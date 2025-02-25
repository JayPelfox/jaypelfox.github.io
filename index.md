---
layout: default
title: "Home"
---

<!-- ========== Services Section ========== -->
<section id="services" class="container">
  <h2>Our Services</h2>
  <p>We provide easy-to-follow DIY tutorials, in-depth product reviews, and step-by-step automation guides to help you transform your home on a budget.</p>

  <div style="display: flex; gap: 2rem; flex-wrap: wrap; margin-top: 1.5rem;">
    <div style="flex: 1; min-width: 280px; background: #fff; padding: 1rem; border-radius: 5px; box-shadow: 0 2px 5px rgba(0,0,0,0.1);">
      <h3>Budget Automation</h3>
      <p>Install sensors, voice assistants, and smart switches without breaking the bank.</p>
    </div>
    <div style="flex: 1; min-width: 280px; background: #fff; padding: 1rem; border-radius: 5px; box-shadow: 0 2px 5px rgba(0,0,0,0.1);">
      <h3>Smart Security</h3>
      <p>Secure your home with camera systems, door locks, and motion detectors.</p>
    </div>
    <div style="flex: 1; min-width: 280px; background: #fff; padding: 1rem; border-radius: 5px; box-shadow: 0 2px 5px rgba(0,0,0,0.1);">
      <h3>Home Entertainment</h3>
      <p>Optimize your media center with streaming devices and smart TVs.</p>
    </div>
  </div>
</section>

<!-- ========== Blog Section ========== -->
<section id="blog" class="container">
  <h2>Latest Blog Posts</h2>
  <div class="post-listing">
    {% for post in site.posts limit:4 %}
      <div class="post-item">
        <h2><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
        <p><small>Published on {{ post.date | date: "%B %d, %Y" }}</small></p>
        <p>{{ post.excerpt }}</p>
        <a class="read-more" href="{{ post.url | prepend: site.baseurl }}">Read More</a>
      </div>
    {% endfor %}
  </div>
  <p style="margin-top: 1.5rem;">
    <a href="{{ '/blog' | prepend: site.baseurl }}" class="read-more">View All Posts</a>
  </p>
</section>

<!-- ========== Contact Section ========== -->
<section id="contact" class="container">
  <h2>Contact Us</h2>
  <p>Questions about a project? Want to request a new tutorial? Reach out!</p>
  <p>Email: <a href="mailto:example@diy-smart-home.com">example@diy-smart-home.com</a></p>
</section>
