---
layout: page
permalink: /experience/
title: Experience
description: "<span style='font-size:1.2rem; font-weight:200;'>My professional work experience - sample (will update later on) </span>"
nav: true
nav_order: 2
---


<style>
/* 🔹 Subtle hover animation for links */
.experience a {
  text-decoration: none;
  color: inherit;
  transition: all 0.2s ease-in-out;
  border-bottom: 1px solid transparent;
}

.experience a:hover {
  color: var(--global-theme-color);
  border-bottom: 1px solid var(--global-theme-color);
}
</style>

<div class="experience">

  <!-- Example 1: Tech Solutions Ltd. -->
  <div class="card mt-3 p-3">
    <div class="row">
      <div class="col-sm-2 text-center">
        <img src="/assets/img/company_a_logo.png" alt="Tech Solutions Logo" class="img-fluid rounded" style="max-width: 100px;">
      </div>

      <div class="col-sm-10 mt-2 mt-md-0">
        <h5 class="title font-weight-bold ml-1 ml-md-4">
          <i class="fa-solid fa-briefcase" style="color: var(--global-theme-color); margin-right: 0.3rem;"></i>
          <a href="https://www.techsolutions.com" target="_blank">Tech Solutions Ltd.</a>
        </h5>

        <h6 class="ml-1 ml-md-4" style="font-size: 0.95rem;">
          <a href="https://www.techsolutions.com" target="_blank">Software Engineer</a>
        </h6>

        <h6 class="ml-1 ml-md-4" style="font-size: 0.95rem; font-style: italic;">
          Full-time | Python & Django Development
        </h6>

        <div class="ml-1 ml-md-4 d-flex justify-content-between align-items-center"
             style="font-size: 0.95rem; margin-top: 0.5rem;">
          <span class="badge badge-secondary">Jan 2022 - Dec 2023</span>
          <span class="text-muted">
            <i class="fa-solid fa-location-dot" style="color: var(--global-theme-color);"></i>
            Dhaka, Bangladesh
          </span>
        </div>

        <div class="ml-1 ml-md-4 mt-3">
          <strong>Key Responsibilities:</strong>
          <ul class="items mt-2" 
              style="display: grid; grid-template-columns: repeat(1, 1fr); row-gap: 0.5rem; padding-left: 1.2rem;">
            <li>Developed web applications using Python and Django framework.</li>
            <li>Improved performance of internal tools by 30% through optimized database queries.</li>
            <li>Collaborated with the frontend team to build responsive user interfaces.</li>
            <li>Maintained CI/CD pipelines using GitHub Actions and Docker.</li>
          </ul>
        </div>
      </div>
    </div>
  </div>

  <!-- Example 2: Internship -->
  <div class="card mt-4 p-3">
    <div class="row">
      <div class="col-sm-2 text-center">
        <img src="/assets/img/intern_logo.png" alt="Internship Logo" class="img-fluid rounded" style="max-width: 100px;">
      </div>

      <div class="col-sm-10 mt-2 mt-md-0">
        <h5 class="title font-weight-bold ml-1 ml-md-4">
          <i class="fa-solid fa-user-graduate" style="color: var(--global-theme-color); margin-right: 0.3rem;"></i>
          <a href="https://www.creativetechhub.com" target="_blank">Creative Tech Hub</a>
        </h5>

        <h6 class="ml-1 ml-md-4" style="font-size: 0.95rem;">
          <a href="https://www.creativetechhub.com" target="_blank">Intern – Web Developer</a>
        </h6>

        <div class="ml-1 ml-md-4 d-flex justify-content-between align-items-center"
             style="font-size: 0.95rem; margin-top: 0.5rem;">
          <span class="badge badge-secondary">Jun 2021 - Aug 2021</span>
          <span class="text-muted">
            <i class="fa-solid fa-location-dot" style="color: var(--global-theme-color);"></i>
            Chattogram, Bangladesh
          </span>
        </div>

        <div class="ml-1 ml-md-4 mt-3">
          <strong>Key Contributions:</strong>
          <ul class="items mt-2" 
              style="display: grid; grid-template-columns: repeat(1, 1fr); row-gap: 0.5rem; padding-left: 1.2rem;">
            <li>Built responsive webpages using HTML, CSS, and JavaScript.</li>
            <li>Assisted in developing backend APIs with Flask.</li>
            <li>Learned version control and teamwork using Git and GitHub.</li>
          </ul>
        </div>
      </div>
    </div>
  </div>

</div>
