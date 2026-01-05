---
layout: page
title: Contact
description: Get in touch with us
permalink: /contact/
full_width: true
---

<div class="container">

<div class="row g-5">

<!-- Contact Form -->
<div class="col-lg-7">
<div class="card border-0 shadow-sm">
<div class="card-body p-4 p-md-5">
<h3 class="mb-4">Send us a Message</h3>
<form action="https://formspree.io/f/xyzgwkpn" method="POST" class="contact-form" id="contactForm">
<input type="hidden" name="_subject" value="New Contact from LHSG Website">
<input type="hidden" name="_next" value="{{ site.url }}{{ site.baseurl }}/contact?success=true">
<div class="row g-3">
<div class="col-md-6">
<label for="name" class="form-label">Your Name *</label>
<input type="text" class="form-control" id="name" name="name" placeholder="John Doe" required>
<div class="invalid-feedback">Please enter your name.</div>
</div>
<div class="col-md-6">
<label for="email" class="form-label">Your Email *</label>
<input type="email" class="form-control" id="email" name="email" placeholder="john@example.com" required>
<div class="invalid-feedback">Please enter a valid email address.</div>
</div>
<div class="col-12">
<label for="subject" class="form-label">Subject *</label>
<select class="form-select" id="subject" name="subject" required>
<option value="">What do you want to tell us about?</option>
<option value="Business Inquiry">Business Inquiry</option>
<option value="Partnership Opportunity">Partnership Opportunity</option>
<option value="Product Support">Product Support</option>
<option value="Career Opportunity">Career Opportunity</option>
<option value="Other">Other</option>
</select>
<div class="invalid-feedback">Please select a subject.</div>
</div>
<div class="col-12">
<label for="message" class="form-label">Your Message *</label>
<textarea class="form-control" id="message" name="message" rows="5" placeholder="Tell us about your project or question..." required></textarea>
<div class="invalid-feedback">Please enter your message.</div>
</div>
<div class="col-12">
<button type="submit" class="btn btn-primary btn-lg">
<i class="fas fa-paper-plane me-2"></i>Send Message
</button>
</div>
</div>
</form>

<!-- Success Message (shown via URL parameter) -->
<div id="successMessage" class="alert alert-success mt-4 d-none" role="alert">
<i class="fas fa-check-circle me-2"></i>
<strong>Thank you!</strong> Your message has been sent successfully. We'll get back to you soon.
</div>

<script>
// Check for success parameter and show message
if (window.location.search.includes('success=true')) {
    document.getElementById('successMessage').classList.remove('d-none');
    document.getElementById('contactForm').reset();
}
</script>
</div>
</div>
</div>

<!-- Contact Info -->
<div class="col-lg-5">
<div class="contact-info">
<h4>Contact Information</h4>

<div class="info-item">
<i class="fas fa-envelope"></i>
<div class="info-content">
<h5>Email</h5>
<p><a href="mailto:contact.lhsg@gmail.com">contact.lhsg@gmail.com</a></p>
</div>
</div>

<div class="info-item">
<i class="fas fa-map-marker-alt"></i>
<div class="info-content">
<h5>Address</h5>
<p>#310, 105 Dong,<br>Seoul National University (SNU),<br>1 Gwanak-ro, Gwanak-gu,<br>Seoul, Korea</p>
</div>
</div>

<div class="info-item">
<i class="fas fa-clock"></i>
<div class="info-content">
<h5>Business Hours</h5>
<p>Monday - Friday: 9:00 AM - 6:00 PM (KST)</p>
</div>
</div>

<hr class="my-4 opacity-25">

<h5 class="text-white mb-3">Follow Us</h5>
<div class="d-flex gap-2">
<a href="https://github.com/lhsg" class="btn btn-outline-light btn-social" target="_blank">
<i class="fab fa-github"></i>
</a>
<a href="https://facebook.com/lhsgfb" class="btn btn-outline-light btn-social" target="_blank">
<i class="fab fa-facebook-f"></i>
</a>
<a href="https://twitter.com/LHSG_" class="btn btn-outline-light btn-social" target="_blank">
<i class="fab fa-twitter"></i>
</a>
</div>
</div>
</div>

</div>

<!-- Map Section -->
<div class="row mt-5">
<div class="col-12">
<div class="card border-0 shadow-sm overflow-hidden">
<iframe
src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3165.4858736776!2d126.95170661531042!3d37.45982397981938!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x357ca1005e3a9c75%3A0xa5d6d05d9c2f6b8!2sSeoul%20National%20University!5e0!3m2!1sen!2skr!4v1640000000000!5m2!1sen!2skr"
width="100%"
height="400"
style="border:0;"
allowfullscreen=""
loading="lazy"
referrerpolicy="no-referrer-when-downgrade">
</iframe>
</div>
</div>
</div>

</div>
