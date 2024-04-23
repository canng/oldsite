---
layout: page
title: Contact me
permalink: /contact
#comments: true
---

<h2>Leave me a message </h2>

<!-- modify this form HTML and place wherever you want your form 
https://formspree.io/forms/xyyrlbba/integration
-->
<form action="https://formspree.io/f/xyyrlbba" method="POST">

  <div>
    <label for="email" style="font-size: 18px;">Your email:</label><br>
    <input type="email" id="email" name="email" style="width: 650px; height: 50px;" ><br>
    <br>
  </div>
  <div>
    <label for="message" style="font-size: 18px;">Your message:</label><br>
    <textarea id="message" name="message" rows="10" cols="80"></textarea><br>
  </div>
  <!-- your other form fields go here -->
  <div>
    <br>
    <button type="submit" style="font-size: 18px;">Send</button>
  </div>
</form>
