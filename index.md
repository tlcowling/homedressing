---
layout: default
title: "Homedressing"
---

<div class="carousel-container">
    <div class="carousel">
        <img src="/assets/images/image1.png" class="active" alt="Image 1">
        <img src="/assets/images/image2.png" alt="Image 2">
    </div>
</div>

<div class="text-content">
    <p>
        Úspěšný design se skládá z několika složek: design na míru plus širokodostupný nábytek, zpestřený ikonickými kousky ze světa a osobitými nebo starožitnými detaily.
    </p>
    <p>
        K práci s prostorem přistupuji velice individuálně, ráda řeším zařizování na míru, aby Váš interiér vynikl co nejlépe.
    </p>
    <p>
        Pro inspiraci shlédněte moje <a href="/portfolio">portfolio</a>.
    </p>
</div>

<script>
    let currentIndex = 0;
    const images = document.querySelectorAll('.carousel img');
    
    function showNextImage() {
        images[currentIndex].classList.remove('active');
        currentIndex = (currentIndex + 1) % images.length;
        images[currentIndex].classList.add('active');
    }

    setInterval(showNextImage, 3000);
</script>
