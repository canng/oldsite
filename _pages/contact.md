---
layout: page
title: Contact me
permalink: /contact
#comments: true
---

<div style="max-width: 1400px; margin: 0 auto;">

<h2>Leave me a message </h2>

<!-- modify this form HTML and place wherever you want your form 
https://formspree.io/forms/xyyrlbba/integration
-->
<form action="https://formspree.io/f/xyyrlbba" method="POST">

  <div>
    <label for="name" style="font-size: 18px;">Your name:</label><br>
    <input type="name" id="name" name="name" style="width: 650px; height: 25px;" ><br>
    <br>
  </div>
  <div>
    <label for="email" style="font-size: 18px;">Your email:</label><br>
    <input type="email" id="email" name="email" style="width: 650px; height: 25px;" ><br>
    <br>
  </div>
  <div>
    <label for="message" style="font-size: 18px;">Your message:</label><br>
    <textarea id="message" name="message" rows="6" cols="76"></textarea><br>
  </div>
  <!-- your other form fields go here -->
  <div>
    <br>
        <button type="submit" style="font-size: 18px; padding: 10px 20px; background-color: #fa7c1e; color: white; border: none; border-radius: 5px;">Send</button>

  </div>
</form>


</div>