---
layout: default
title: Home
---

<style>
  /* Basic custom CSS to mimic the layout. You might need to adjust based on your chosen theme. */
  .profile-section {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    gap: 30px; /* Space between image and text */
    margin-bottom: 50px;
    padding: 20px;
    border-radius: 8px;
    background-color: #f8f8f8; /* Light background for the section */
  }
  .profile-image {
    flex: 0 0 200px; /* Fixed width for the image container */
    height: 200px; /* Fixed height to make it a circle */
    border-radius: 50%;
    overflow: hidden;
    box-shadow: 0 4px 8px rgba(0,0,0,0.1);
  }
  .profile-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  .profile-text {
    flex: 1; /* Takes remaining space */
    min-width: 300px; /* Ensures text doesn't get too narrow */
  }
  .social-links a {
    margin-right: 15px;
    text-decoration: none;
    color: #007bff; /* Example link color */
  }
  .featured-work-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); /* Responsive grid */
    gap: 25px;
    margin-top: 40px;
  }
  .work-item {
    border: 1px solid #ddd;
    border-radius: 8px;
    overflow: hidden;
    box-shadow: 0 2px 5px rgba(0,0,0,0.05);
    text-align: center;
  }
  .work-item img {
    width: 100%;
    height: 180px; /* Consistent height for images */
    object-fit: cover;
    display: block;
  }
  .work-item-content {
    padding: 15px;
  }
  .work-item-content h3 {
    margin-top: 0;
    font-size: 1.1em;
    color: #333;
  }
  .work-item-content p {
    font-size: 0.9em;
    color: #666;
    margin-bottom: 10px;
  }
  .work-item-content .icon-link {
    display: inline-block;
    margin: 0 10px;
    color: #555;
    font-size: 1.2em;
  }
  .footer-info {
    text-align: center;
    margin-top: 60px;
    padding-top: 20px;
    border-top: 1px solid #eee;
    color: #777;
    font-size: 0.9em;
  }
</style>

<div class="profile-section">
  <div class="profile-image">
    <img src="/assets/profile.jpg" alt="Aris Thorne Profile Photo">
  </div>
  <div class="profile-text">
    <h1>Hello! I'm Ryan McCune</h1>
    <p>I am a PhD Student in Civil Engineering at North Carolina State University, focusing in Coastal Engineering. My research combines machine learning, numerical modeling, and in-situ data collection to address chronic coastal flooding.</p>
    <p class="social-links">
      <a href="mailto:rmccune@ncsu.edu">aris.thorne@westeros.edu</a>
      <a href="https://linkedin.com/in/ryan-mccune" target="_blank" rel="noopener noreferrer">LinkedIn</a>
      <a href="https://scholar.google.com/citations?user=CnYIFHQAAAAJ&hl=en&oi=ao" target="_blank" rel="noopener noreferrer">Google Scholar</a>
    </p>
  </div>
</div>

<h2>Featured Work:</h2>
<div class="featured-work-grid">
  <div class="work-item">
    <img src="/assets/sensor_prototype.jpg" alt="Antibiotic-Resistance Sensor">
    <div class="work-item-content">
      <h3>Antibiotic-Resistance Sensor</h3>
      <p>Development of a novel portable sensor for rapid detection of antibiotic-resistant genes in water samples.</p>
      <a href="/sensordev/#project-antibiotic" class="icon-link">➡️</a>
    </div>
  </div>

  <div class="work-item">
    <img src="/assets/publication_graph.jpg" alt="Latest Publication">
    <div class="work-item-content">
      <h3>Latest Publication: "Microplastics in Rivers"</h3>
      <p>Published in Environmental Science & Technology. Explores microplastic distribution patterns using drone imagery.</p>
      <a href="/publications/#microplastics" class="icon-link">📖</a>
    </div>
  </div>

  <div class="work-item">
    <img src="/assets/field_work_drone.jpg" alt="Upcoming Field Work">
    <div class="work-item-content">
      <h3>Upcoming: Field Work in the Amazon</h3>
      <p>Deploying autonomous drones for atmospheric composition analysis in collaboration with the Institute of Amazonian Research.</p>
      <a href="/research/#amazon-fieldwork" class="icon-link">✈️</a>
    </div>
  </div>
</div>

<div class="footer-info">
  <p>&copy; {{ site.time | date: "%Y" }} {{ site.title }} | Powered by GitHub Pages & Jekyll</p>
</div>
