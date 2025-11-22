---
layout: page
title: Resources
permalink: /resources/
---

<div class="resources-grid">
  <a class="resource-card" href="/resources/physics-equations/">
    <div class="resource-card-title">Physics Equations</div>
    <div class="resource-card-subtitle">
      PHY 2130 / 2140 equation sheets, derivations, examples
    </div>
  </a>
</div>

<hr>

<h2>Contact me</h2>

<form
  class="contact-card"
  action="https://formspree.io/f/xyzveolr"
  method="POST"
>
  <div class="contact-row">
    <label>
      First name
      <input type="text" name="first_name" required>
    </label>

    <label>
      Email
      <input type="email" name="email" required>
    </label>
  </div>

  <label>
    Subject
    <input type="text" name="subject" required>
  </label>

  <label>
    Message
    <textarea name="message" rows="6" required></textarea>
  </label>

  <!-- Anti-spam honeypot (hidden) -->
  <input type="text" name="_gotcha" style="display:none">

  <!-- Optional: redirect back to Resources after submit -->
  <input type="hidden" name="_next" value="https://www.abhishekcp.com/resources/">

  <button class="contact-btn" type="submit">Send</button>
</form>
