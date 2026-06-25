---
layout: about
title: Home
permalink: /
subtitle: <i class="fa-solid fa-location-dot"></i> SUSTech, Shenzhen

profile:
  align: right
  image: bing.jpeg
  image_circular: false # crops the image to make it circular

selected_papers: false # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page

announcements:
  enabled: false # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

<link rel="stylesheet" href="{{ '/assets/css/site.css' | relative_url }}">

<section class="home-section home-about">

  <p>I am a final-year Ph.D. student in the Department of Electrical and Electronic Engineering at Southern University of Science and Technology (SUSTech). I am working at the intersection of robotics & AI, supervised by Prof. <a href="https://scholar.google.com/citations?user=DxDCU7AAAAAJ&hl=zh-CN">Max Q.-H. Meng</a> and Prof. <a href="https://jkwang1992.github.io/">Jiankun Wang</a>. Before that, I received my B.Eng. degree from the same department at SUSTech in 2020, where I worked on flexible electronic sensors with Prof. <a href="https://sse.cuhk.edu.cn/en/faculty/terrytaoye">Terry Tao Ye</a>.</p>

  <p>My recent research focuses on autonomous navigation and human-robot interaction, particularly developing robot mobility and navigation capabilities for dynamic environments beyond the laboratory and human-centered field applications.
</p>

</section>

<section class="home-section home-news">
  <h1>News</h1>
  <ul class="news-list">
    <li>
      <span class="news-date">2025/03</span>
      <span class="news-text">NAMR-RRT was published in IEEE Transactions on Automation Science and Engineering.</span>
    </li>
    <li>
      <span class="news-date">2025/01</span>
      <span class="news-text">Autonomous multiple-trolley collection work appeared in Journal of Field Robotics.</span>
    </li>
    <li>
      <span class="news-date">2024/09</span>
      <span class="news-text">Smart mobility with agent-based foundation models was published in IEEE Transactions on Intelligent Vehicles.</span>
    </li>
  </ul>
</section>

<section class="home-section home-projects">
  <h1>Research</h1>

  <h2>Social Navigation</h2>
  <div class="project-list">
    <div class="project-item">
      <div class="project-media"></div>
      <div class="project-content">
        <h3>Intention-Aware Crowd Navigation</h3>
        <p>Learning robot visual navigation in crowds via intention-aware scene representations for socially aware motion in human environments.</p>
        <div class="project-links">
          <a href="{{ '/publications/#bao2026learning' | relative_url }}">RA-L 2026</a>
        </div>
      </div>
    </div>
    <div class="project-item">
      <div class="project-media"></div>
      <div class="project-content">
        <h3>Person-Following Navigation</h3>
        <p>Field-based search for robot person following in unknown dynamic environments.</p>
        <div class="project-links">
          <a href="{{ '/publications/#ye2026rpf' | relative_url }}">T-MECH 2025</a>
        </div>
      </div>
    </div>
    <div class="project-item">
      <div class="project-media"></div>
      <div class="project-content">
        <h3>Neural Adaptive Motion Planning</h3>
        <p>Neural adaptive motion planning for mobile robots in dynamic environments.</p>
        <div class="project-links">
          <a href="{{ '/publications/#sun2025namr' | relative_url }}">T-ASE 2025</a>
        </div>
      </div>
    </div>
  </div>

  <h2>Mobile Manipulation</h2>
  <div class="project-list">
    <div class="project-item">
      <div class="project-media"></div>
      <div class="project-content">
        <h3>Collaborative Trolley Transportation</h3>
        <p>Multi-robot planning and control for autonomous nonholonomic robots transporting luggage trolleys in structured service environments.</p>
        <div class="project-links">
          <a href="{{ '/publications/#xia2023collaborative' | relative_url }}">IROS 2023</a>
          <a href="{{ '/publications/#xie2025autonomous' | relative_url }}">JFR 2025</a>
        </div>
      </div>
    </div>
    <div class="project-item">
      <div class="project-media"></div>
      <div class="project-content">
        <h3>Robot Cart-Pushing</h3>
        <p>Integrating maneuverable planning and adaptive control for robot cart-pushing under disturbances.</p>
        <div class="project-links">
          <a href="{{ '/publications/#zhang2026integrating' | relative_url }}">arXiv 2026</a>
        </div>
      </div>
    </div>
    <div class="project-item">
      <div class="project-media"></div>
      <div class="project-content">
        <h3>Autonomous Trolley Collection</h3>
        <p>System design, prescribed-performance control, and implementation for multiple-trolley collection with mobile robots.</p>
        <div class="project-links">
          <a href="{{ '/publications/#pang2026davpc' | relative_url }}">arXiv 2026</a>
          <a href="{{ '/publications/#xie2025autonomous' | relative_url }}">JFR 2025</a>
          <a href="{{ '/publications/#xi2024disturbance' | relative_url }}">PCS 2024</a>
        </div>
      </div>
    </div>
  </div>
</section>
