---
layout: page
title: Get In Touch
description: I'd love to hear from you. Let's start a conversation!
permalink: /contact/
---

<div class="grid" style="max-width: 900px; margin: 0 auto;">

<div class="card">
<div class="card-content">
<h3>Email</h3>
<p>For general inquiries and collaboration opportunities.</p>
<a href="mailto:{{ site.author.email }}" class="card-link">{{ site.author.email }}</a>
</div>
</div>

<div class="card">
<div class="card-content">
<h3>Social Media</h3>
<p>Connect with me on social platforms.</p>
<div style="margin-top: 1rem;">
{% if site.author.github %}
<a href="https://github.com/{{ site.author.github }}" target="_blank" rel="noopener" class="card-link" style="display: block; margin-bottom: 0.5rem;">GitHub</a>
{% endif %}
{% if site.author.linkedin %}
<a href="https://linkedin.com/in/{{ site.author.linkedin }}" target="_blank" rel="noopener" class="card-link" style="display: block; margin-bottom: 0.5rem;">LinkedIn</a>
{% endif %}
{% if site.author.twitter %}
<a href="https://twitter.com/{{ site.author.twitter }}" target="_blank" rel="noopener" class="card-link" style="display: block;">Twitter</a>
{% endif %}
</div>
</div>
</div>

</div>

<form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
    <h2 style="text-align: center; margin-bottom: 2rem;">Send Me a Message</h2>
    
    <div class="form-group">
        <label for="name">Name *</label>
        <input type="text" id="name" name="name" required>
    </div>

    <div class="form-group">
        <label for="email">Email *</label>
        <input type="email" id="email" name="_replyto" required>
    </div>

    <div class="form-group">
        <label for="subject">Subject</label>
        <input type="text" id="subject" name="subject">
    </div>

    <div class="form-group">
        <label for="message">Message *</label>
        <textarea id="message" name="message" required></textarea>
    </div>

    <button type="submit" class="button button-primary" style="width: 100%;">Send Message</button>
    
    <p style="text-align: center; margin-top: 1rem; color: var(--text-secondary); font-size: 0.875rem;">
        To make this form work, sign up for free at <a href="https://formspree.io" target="_blank">Formspree</a> and replace YOUR_FORM_ID with your actual form ID.
    </p>
</form>

<div class="secondary-bg" style="padding: 3rem 2rem; border-radius: 0.5rem; margin-top: 3rem; text-align: center;">
    <h2>Let's Build Something Together</h2>
    <p style="max-width: 600px; margin: 0 auto 2rem;">
        Whether you have a project in mind, want to collaborate, or just want to say hello, 
        I'm always open to new connections and opportunities.
    </p>
    <div style="display: flex; gap: 1rem; justify-content: center; flex-wrap: wrap;">
        <a href="{{ '/projects' | relative_url }}" class="button button-secondary">View My Work</a>
        <a href="{{ '/about' | relative_url }}" class="button button-secondary">Learn More About Me</a>
    </div>
</div>