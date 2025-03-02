---
layout: default
title: Kontakt
permalink: /contact/
---

<div class="contact-container">
    <div class="contact-image">
        <img src="{{ '/assets/images/m.jpg' | relative_url }}" alt="Maria Shatova">
    </div>
    <div class="contact-info">
        <h1>Kontaktujte</h1>
        <h2>Maria Shatova</h2>
        <p>Praha</p>
        <p><a href="mailto:shatova.mariya@gmail.com">shatova.mariya@gmail.com</a></p>
        <p>Tel: +420 775 076 049</p>
        <p><a href="https://www.homedressing.cz" target="_blank">www.homedressing.cz</a></p>

        <form action="#" method="POST" class="contact-form">
            <input type="text" name="name" placeholder="Jméno Příjmení *" required>
            <input type="email" name="email" placeholder="Email *" required>
            <input type="text" name="subject" placeholder="Téma">
            <textarea name="message" placeholder="Vzkaz"></textarea>
            <button type="submit">Odeslat</button>
        </form>
    </div>
</div>

