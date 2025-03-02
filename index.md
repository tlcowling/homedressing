---
layout: default
title: "Homedressing"
---

<div class="home-content">
    <div class="carousel-container">
        <div class="carousel">
            <a href="#" data-lightbox="home-gallery">
                <img src="/assets/images/image1.png" alt="Home Design 1" class="active">
            </a>
            <a href="#" data-lightbox="home-gallery">
                <img src="/assets/images/image2.png" alt="Home Design 2">
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

<script>
    let images = document.querySelectorAll('.carousel img');
    let currentIndex = 0;

    function showNextImage() {
        images[currentIndex].classList.remove('active');
        currentIndex = (currentIndex + 1) % images.length;
        images[currentIndex].classList.add('active');
    }

    setInterval(showNextImage, 4000);
</script>

