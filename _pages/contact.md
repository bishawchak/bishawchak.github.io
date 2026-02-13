---
layout: page
permalink: /contact/
title: Contact
description: "<span style='font-size:1.2rem; font-weight:200;'>Feel free to reach out to me at LinkedIn or email.</span>"
nav: true
nav_order: 7
---

<div class="contact-container">

  <!-- Top Cards: Social + Email -->
  <div class="contact-top">

    <!-- Social Profiles -->
    <div class="contact-card top-card">
      <i class="fa-solid fa-share-nodes"></i>
      <div>
        <h5 style="color: var(--global-theme-color);">Social Profiles</h5>
        <div class="social-icons">
          <a href="https://github.com/bishawchak" target="_blank"><i class="fab fa-github"></i></a>
          <a href="https://www.linkedin.com/in/bishawkirti" target="_blank"><i class="fab fa-linkedin"></i></a>
          <a href="https://www.facebook.com/bishaw1245" target="_blank"><i class="fab fa-facebook"></i></a>
          <a href="https://www.instagram.com/__bishaw" target="_blank"><i class="fab fa-instagram"></i></a>
        </div>
      </div>
    </div>

    <!-- Email -->
    <div class="contact-card top-card">
      <i class="fa-solid fa-envelope"></i>
      <div>
        <h5 style="color: var(--global-theme-color);">Email</h5>
        <a href="mailto:kuet.bishaw@gmail.com">kuet.bishaw@gmail.com</a>
      </div>
    </div>

  </div>

  <!-- Contact Form -->
  <div class="contact-form">
    <form action="https://getform.io/f/bnlngreb" method="POST">
      <input type="hidden" name="_redirect" value="/thank-you/">

      <!-- Two-column input row -->
      <div class="form-row">
        <div class="form-column">
          <input type="text" name="name" placeholder="Your Name" required>
        </div>
        <div class="form-column">
          <input type="email" name="email" placeholder="Your Email" required>
        </div>
      </div>

      <!-- Subject row -->
      <div class="form-row">
        <div class="form-column">
          <input type="text" name="subject" placeholder="Subject" required>
        </div>
      </div>

      <!-- Message row -->
      <div class="form-row">
        <div class="form-column">
          <textarea name="message" placeholder="Message" required></textarea>
        </div>
      </div>

      <div class="form-button">
        <button type="submit">Send Message</button>
      </div>
    </form>
  </div>

</div>

<style>
/* Contact container */
.contact-container {
  display: flex;
  flex-direction: column;
  gap: 2rem;
  width: 100%;
  max-width: 900px;
  margin: 0 auto;
}

/* Top cards container */
.contact-top {
  display: flex;
  gap: 2rem;
  align-items: stretch;
  flex-wrap: wrap;
}

/* Top cards (Social + Email) */
.top-card {
  flex: 1 1 auto;
  display: flex;
  gap: 1rem;
  border-radius: 0;
  padding: 1.5rem 1.5rem;
  background-color: var(--card-bg);
  border: 1px solid rgb(90, 90, 90);
  align-items: flex-start;
}

[data-theme="dark"] .top-card {
  border-color: rgb(180, 180, 180);
}

/* Main icon on top card (remove circle and align with heading) */
.top-card > i {
  display: inline-flex;
  justify-content: center;
  align-items: center;
  width: 1.6rem;
  height: 1.6rem;
  border-radius: 0;
  background-color: transparent;
  color: var(--global-theme-color);
  font-size: 1.6rem;
  flex-shrink: 0;
}

/* Adjust Email icon specifically */
.top-card:nth-child(2) > i {
  position: relative;
  top: 0.1rem; /* nudges icon up for perfect alignment */
}

/* Text inside card */
.top-card > div {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  gap: 0.25rem;
}

/* Heading and links */
.top-card h5 {
  margin: 0 0 0.5rem 0;
  font-weight: 600;
}

.top-card a {
  color: var(--text-color);
  text-decoration: none;
  transition: all 0.2s ease-in-out;
  border-bottom: 1px solid transparent;
}

.top-card a:hover {
  color: var(--global-theme-color);
  border-bottom: 1px solid var(--global-theme-color);
}

/* Social icons */
.social-icons {
  display: flex;
  gap: 0.5rem;
  margin-top: 0.5rem;
}

.social-icons a {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 32px;
  height: 32px;
  border-radius: 50%;
  background-color: var(--global-theme-color);
  color: #fff;
  font-size: 1rem;
  transition: transform 0.3s ease, filter 0.3s ease, opacity 0.3s ease;
  opacity: 0.85;
}

.social-icons a:hover {
  transform: scale(1.1);           /* enlarge slightly */
  opacity: 1;                       /* fully visible */
  filter: brightness(0.85);         /* automatically darkens background */
  color: #fff;                       /* icon stays white */
}

/* Contact Form */
.contact-form {
  width: 100%;
  background-color: var(--card-bg);
  border: 1px solid rgb(90, 90, 90);
  padding: 1.5rem;
  border-radius: 0;
  transition: border-color 0.3s ease, background-color 0.3s ease;
}

[data-theme="dark"] .contact-form {
  border-color: rgb(180, 180, 180);
}

/* Two-column layout for first row inputs */
.form-row {
  display: flex;
  gap: 0.5rem;
  margin-bottom: 1rem;
}

.form-column {
  flex: 1;
  min-width: 0;
}

/* Input and Textarea */
.contact-form input,
.contact-form textarea {
  width: 100%;
  padding: 0.75rem 1rem;
  margin-bottom: 1rem;
  border-radius: 0;
  border: 1px solid rgb(100, 100, 100);
  box-sizing: border-box;
  color: var(--text-color);
  background-color: var(--input-bg);
  transition: border-color 0.3s ease, background-color 0.3s ease;
}

.contact-form input::placeholder,
.contact-form textarea::placeholder {
  color: var(--text-muted);
}

/* Focus */
.contact-form input:focus,
.contact-form textarea:focus {
  border-color: var(--global-theme-color);
  outline: none;
}

/* Button */
.form-button {
  text-align: center;
  margin-top: 0.5rem;
}

.contact-form button {
  background-color: var(--global-theme-color);
  color: var(--button-text-color, #fff);
  padding: 0.75rem 1.5rem;
  border: none;
  border-radius: 0.5rem;
  cursor: pointer;
  font-weight: 600;
  transition: all 0.2s ease-in-out;
}

.contact-form button:hover {
  background-color: var(--button-hover-bg, #00c853);
  transform: scale(1.05);
}

/* Responsive */
@media (max-width: 600px) {
  .form-row {
    flex-direction: column;
  }

  .form-column {
    width: 100%;
  }

  .top-card {
    flex-direction: row;
    gap: 0.8rem;
  }

  .top-card > i {
    top: 0;
  }

  .top-card:nth-child(2) > i {
    top: 0;
  }
}
</style>
