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
  {% assign home_news = site.news | sort: "date" | reverse %}
  <ul class="news-list">
    {% for item in home_news limit: 3 %}
      <li>
        <span class="news-date">{{ item.date | date: "%Y/%m" }}</span>
        <span class="news-text">{{ item.content | markdownify | remove: '<p>' | remove: '</p>' | strip }}</span>
      </li>
    {% endfor %}
  </ul>
</section>

<section class="home-section home-projects">
  <h1>Research</h1>

  <h2>Social Navigation</h2>
  <p class="research-intro">
  Social navigation aims to enable robots to move safely, efficiently, and naturally in environments shared with humans. My research mainly addresses point-to-point navigation in crowded and dynamic environments through learning-based methods, covering data collection, global path planning, and RL-based navigation policies. Beyond general navigation tasks, I also explore person following as a special form of social navigation.
  </p>
  <div class="project-list">
    <div class="project-item">
      <div class="project-media">
        <video autoplay muted loop playsinline preload="metadata" poster="{{ '/assets/img/publication_preview/navisaaclab_web.jpg' | relative_url }}">
          <source src="{{ '/assets/video/navisaaclab_web.mp4' | relative_url }}" type="video/mp4">
        </video>
      </div>
      <div class="project-content">
        <h3>Human-Aware Navigation Simulation and Benchmark</h3>
        <p>NavIsaacLab builds photo-realistic, physics-based crowd simulation on Isaac Lab, using data-driven pedestrian generation for providing richer visual feedback and GPU-parallel environments to accelerate data collection and training human-aware navigation policies.</p>
        <div class="project-links">
          <a href="{{ '/publications/#xia2026navisaaclab' | relative_url }}">arXiv 2026</a>
        </div>
      </div>
    </div>
    <div class="project-item">
      <div class="project-media">
        <video autoplay muted loop playsinline preload="metadata" poster="{{ '/assets/img/publication_preview/bev_web.jpg' | relative_url }}">
          <source src="{{ '/assets/video/bev_web.mp4' | relative_url }}" type="video/mp4">
        </video>
      </div>
      <div class="project-content">
        <h3>Intention-Aware Crowd Navigation</h3>
        <p>iCrowdNav learns RL-based crowd navigation policies from RGB-D observations by combining occupancy features with human pose cues, enabling the robot to infer pedestrian intentions and navigate more safely in dense crowds.</p>
        <div class="project-links">
          <a href="{{ '/publications/#bao2026learning' | relative_url }}">RA-L 2026</a>
        </div>
      </div>
    </div>
    <div class="project-item">
      <div class="project-media">
        <img src="{{ '/assets/img/publication_preview/rpf_search.gif' | relative_url }}" alt="Person-following navigation preview">
      </div>
      <div class="project-content">
        <h3>Person-Following</h3>
        <p>RPF-Search addresses target loss in unknown and dynamic environments, using belief-guided fields for topographic occlusions and adaptive search strategies for moving pedestrian occluders.</p>
        <div class="project-links">
          <a href="{{ '/publications/#ye2026rpf' | relative_url }}">T-MECH 2025</a>
        </div>
      </div>
    </div>
    <div class="project-item">
      <div class="project-media">
        <img src="{{ '/assets/img/publication_preview/namr.gif' | relative_url }}" alt="Neural adaptive motion planning preview">
      </div>
      <div class="project-content">
        <h3>Neural Adaptive Path Planning</h3>
        <p>NAMR-RRT improves sampling-based planning methods by using neural heuristic regions to focus sampling on promising areas, reducing unnecessary node exploration for real-time computation in dynamic environments.</p>
        <div class="project-links">
          <a href="{{ '/publications/#sun2025namr' | relative_url }}">T-ASE 2025</a>
        </div>
      </div>
    </div>
  </div>

  <h2>Mobile Manipulation: Cart Pushing, Collection, and Transportation</h2>
  <p class="research-intro">
  My research in mobile manipulation focuses on wheeled objects, such as carts, trolleys, and wheelchairs. We develop practical robotic applications built around cart pushing to automate manual trolley collection. We built a full-stack robotic system that integrates localization, perception, manipulation, formation control, and cooperative transportation, enabling two mobile robots to collect scattered carts, arrange them into a queue, and transport them to a target location. The robotic platform was iterated through three versions, evolving from a simple gripper-based mechanism to a dual-arm manipulation system.
  </p>
  <div class="project-list">
    <div class="project-item">
      <div class="project-media">
        <video autoplay muted loop playsinline preload="metadata" poster="{{ '/assets/img/publication_preview/transport_web.jpg' | relative_url }}">
          <source src="{{ '/assets/video/transport_web.mp4' | relative_url }}" type="video/mp4">
        </video>
      </div>
      <div class="project-content">
        <h3>Collaborative Trolley Transportation</h3>
        <p>This work develops an autonomous multi-robot system for transporting long lines of luggage trolleys, with a hierarchical framework for feasible path generation, online motion planning, and feedback control under coupled nonholonomic constraints.</p>
        <div class="project-links">
          <a href="{{ '/publications/#xia2023collaborative' | relative_url }}">IROS 2023</a>
        </div>
      </div>
    </div>
    <div class="project-item">
      <div class="project-media">
        <img src="{{ '/assets/img/publication_preview/cart.png' | relative_url }}" alt="Robot cart-pushing preview">
      </div>
      <div class="project-content">
        <h3>Robot Cart-Pushing</h3>
        <p>This work combines maneuverable push-pose planning with disturbance-rejection control, allowing mobile robots to push carts flexibly and robustly despite payload variation, redundancy, and external disturbances.</p>
        <div class="project-links">
          <a href="{{ '/publications/#zhang2026integrating' | relative_url }}">arXiv 2026</a>
        </div>
      </div>
    </div>
    <div class="project-item">
      <div class="project-media">
        <img src="{{ '/assets/img/publication_preview/vpc.png' | relative_url }}" alt="Autonomous trolley collection preview">
      </div>
      <div class="project-content">
        <h3>Autonomous Trolley Collection</h3>
        <p>This research builds a complete multiple-trolley collection system, including lightweight docking hardware, vision-based control, and disturbance-aware visual predictive control for accurate and stable trolley alignment in real service scenarios.</p>
        <div class="project-links">
          <a href="{{ '/publications/#pang2026davpc' | relative_url }}">arXiv 2026</a>
          <a href="{{ '/publications/#xie2025autonomous' | relative_url }}">JFR 2025</a>
        </div>
      </div>
    </div>
  </div>
</section>
