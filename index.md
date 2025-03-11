---
layout: default
title: "Homedressing"
---

<div class="home-content">
    <div class="carousel-container">
        <div class="carousel">
            <a href="#" class="lightbox-trigger">
                <img src="{{ '/assets/images/image1.png' | relative_url }}" alt="Home Design 1" class="active">
            </a>
            <a href="#" class="lightbox-trigger">
                <img src="{{ '/assets/images/image2.png' | relative_url }}" alt="Home Design 2">
            </a>
        </div>
    </div>
    <div class="home-text">
<p>Úspěšný design se skládá z několika složek: design na míru plus širokodostupný nábytek, zpestřený ikonickými kousky ze světa a osobitými nebo starožitnými detaily. Využívám všech těch prostředků pro dosažení interiéru originálního, stylového, ale zároveň útulného a osobitého.</p>

<p>K práci z prostorem přistupuji velice individuálně, ráda řeším zařizování na míru, aby Váš interiér vyzněl co nejlépé, aby se tam dobře bydlelo a vyhovovalo to Vaším individuálním nárokům.</p>

<p>Zabývám se designem soukromého bydleni, dělám návrhy i projektovou činnost pro komplexní rekonstrukce. Zvlaštní složkou mých praci je také staging bytů k pronájmů, kde je efektního výsledku dosaženo za podmínek omezeného rozpočtu.</p>
        <p><a href="/portfolio/">Pro inspiraci shlédněte moje portfolio.</a></p>
    </div>
</div>
<div id="lightbox">
    <span class="close">&times;</span>
    <img id="lightbox-img" src="" alt="">
</div>
<script>
    document.addEventListener("DOMContentLoaded", function () {
        const lightbox = document.getElementById("lightbox");
        const lightboxImg = document.getElementById("lightbox-img");
        const closeBtn = document.querySelector(".close");

        document.querySelectorAll(".lightbox-trigger img").forEach(img => {
            img.addEventListener("click", function (event) {
                event.preventDefault();
                lightboxImg.src = this.src;
                lightbox.classList.add("show");
            });
        });

        closeBtn.addEventListener("click", function () {
            lightbox.classList.remove("show");
        });

        lightbox.addEventListener("click", function (event) {
            if (event.target === lightbox) {
                lightbox.classList.remove("show");
            }
        });
    });
</script>
