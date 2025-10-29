---
layout: page
title: Projects
permalink: /projects/
description: "<span style='font-size:1.1rem; font-weight:300;'>A showcase of my academic and personal projects.</span>"
nav: true
nav_order: 4
---

<div class="projects-grid">

  <!-- Project 1 -->
  <a href="https://github.com/bishawchak/Student_Attendance_System" target="_blank" class="project-card">
    <img src="/assets/img/homepage.png" alt="Homepage">
    <h3>Student Attendance System</h3>
    <p>A web-based system developed in ASP.NET and C# to automate attendance tracking efficiently.</p>
  </a>

  <!-- Project 2 -->
  <a href="https://github.com/bishawchak/Ping_Pong" target="_blank" class="project-card">
    <img src="/assets/img/demo_game.png" alt="Ping Pong Game">
    <h3>Ping Pong Game</h3>
    <p>A fun and interactive Ping Pong game created in C++ using the Raylib library to simulate real-time ball and paddle movement.</p>
  </a>

  <!-- Project 3 -->
  <a href="https://github.com/bishawchak/Sorting_Algorithm" target="_blank" class="project-card">
    <img src="/assets/img/demo.png" alt="Sorting Algorithm Visualization">
    <h3>Sorting Algorithm Visualization</h3>
    <p>A C++ project that visualizes popular sorting algorithms like Bubble, Insertion, Merge, Quicksort etc  using Raylib.</p>
  </a>

  <!-- Project 4 -->
  <a href="https://github.com/bishawchak/Self_Balancing_Robot" target="_blank" class="project-card">
    <img src="/assets/img/bot.png" alt="Self Balancing Robot">
    <h3>Self Balancing Robot</h3>
    <p>An Arduino project that uses a gyro sensor and PID control to maintain balance on two wheels.</p>
  </a>

  <!-- Project 5 -->
  <a href="https://github.com/bishawchak/DC_Power_Supply/tree/main" target="_blank" class="project-card">
    <img src="/assets/img/circuit_diagram.png" alt="DC Power Supply">
    <h3>DC Power Supply</h3>
    <p>An electronics project that delivers 0–30V DC output with over-voltage, under-voltage, and short-circuit protection.</p>
  </a>

</div>

<style>
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
  margin-top: 2rem;
}

/* Project Card */
.project-card {
  display: block;
  background-color: var(--card-bg); /* match theme */
  border: 1px solid rgb(90, 90, 90);
  padding: 1rem;
  text-align: center;
  transition: all 0.3s ease;
  color: inherit;
  text-decoration: none;
  border-radius: 0; /* square corners like contact page */
}

[data-theme="dark"] .project-card {
  border-color: rgb(180, 180, 180);
}

/* Image */
.project-card img {
  width: 100%;
  height: 220px;
  object-fit: cover;
  border: 1px solid rgba(255, 255, 255, 0.2);
  margin-bottom: 1rem;
  transition: transform 0.3s ease, filter 0.3s ease;
}

/* Title */
.project-card h3 {
  color: var(--global-theme-color);
  font-size: 1.1rem;
  margin-bottom: 0.5rem;
}

/* Description */
.project-card p {
  font-size: 0.9rem;
  color: var(--text-color);
  margin-bottom: 0.8rem;
}

/* Hover Effect – same as contact cards */
.project-card:hover {
  transform: scale(1.03);
  border-color: var(--global-theme-color);
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.4);
  text-decoration: none;
  background-color: rgba(255, 255, 255, 0.03);
}

/* Slight hover change for light mode */
[data-theme="light"] .project-card:hover {
  background-color: rgba(0, 0, 0, 0.03);
}

/* Optional: zoom image a bit when hovering */
.project-card:hover img {
  transform: scale(1.05);
  filter: brightness(0.9);
}
</style>
