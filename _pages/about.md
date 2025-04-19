---
permalink: /
#title: "About me"
#excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
<style>
/* Color Palette - Luxurious Tech Theme */
:root {
  --primary: #1E3A8A; /* Deep Navy Blue */
  --secondary: #3563E9; /* Bright Blue */
  --accent: #60A5FA; /* Light Blue */
  --accent-gold: #F59E0B; /* Gold */
  --accent-soft: #DBEAFE; /* Very Light Blue */
  --light: #F8FAFC; /* Off-White */
  --dark: #0F172A; /* Very Dark Blue */
  --text: #334155; /* Slate Gray */
  --success: #10B981; /* Emerald */
  --info: #0EA5E9; /* Sky Blue */
  --warning: #F59E0B; /* Amber */
  --danger: #EF4444; /* Red */
  --shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
  --shadow-lg: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
  --shadow-inner: inset 0 2px 4px 0 rgba(0, 0, 0, 0.06);
  --border-radius: 8px;
  --border-radius-lg: 12px;
  --transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
  --font-heading: 'Poppins', sans-serif;
  --font-body: 'Inter', sans-serif;
}

@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Poppins:wght@400;500;600;700&display=swap');

.page__content {
  font-family: var(--font-body);
  line-height: 1.7;
  color: var(--text);
}

h1, h2, h3, h4, h5, h6 {
  font-family: var(--font-heading);
  font-weight: 600;
  line-height: 1.3;
  color: var(--dark);
}

p {
  margin-bottom: 1.2rem;
}

.btn {
  display: inline-block;
  padding: 12px 24px;
  background-color: var(--primary);
  color: white;
  border-radius: var(--border-radius);
  text-decoration: none;
  font-weight: 500;
  transition: var(--transition);
  border: none;
  cursor: pointer;
  box-shadow: var(--shadow);
  font-family: var(--font-heading);
  text-align: center;
  margin: 10px 5px;
}

.btn:hover {
  transform: translateY(-2px);
  box-shadow: var(--shadow-lg);
  background-color: var(--secondary);
}

.btn-outline {
  background-color: transparent;
  border: 2px solid var(--primary);
  color: var(--primary)!important;
}

.btn-outline:hover {
  background-color: var(--primary);
  color: white !important;
}

/* Hero Section */
.hero {
  position: relative;
  background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
  border-radius: var(--border-radius-lg);
  color: white;
  padding: 60px 40px;
  margin-bottom: 40px;
  overflow: hidden;
  box-shadow: var(--shadow-lg);
}

.hero::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-image: url("data:image/svg+xml,%3Csvg width='100' height='100' viewBox='0 0 100 100' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M11 18c3.866 0 7-3.134 7-7s-3.134-7-7-7-7 3.134-7 7 3.134 7 7 7zm48 25c3.866 0 7-3.134 7-7s-3.134-7-7-7-7 3.134-7 7 3.134 7 7 7zm-43-7c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zm63 31c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zM34 90c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zm56-76c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zM12 86c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm28-65c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm23-11c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm-6 60c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm29 22c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zM32 63c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm57-13c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm-9-21c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM60 91c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM35 41c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM12 60c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2z' fill='%23ffffff' fill-opacity='0.05' fill-rule='evenodd'/%3E%3C/svg%3E");
  opacity: 0.8;
}

.hero-content {
  position: relative;
  z-index: 2;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 40px;
}

.hero-text {
  flex: 1;
}

.hero-image {
  flex: 1;
  text-align: center;
}

.hero-image img {
  max-width: 260px;
  border-radius: 50%;
  border: 4px solid white;
  box-shadow: var(--shadow-lg);
  transition: var(--transition);
}

.hero-image img:hover {
  transform: scale(1.03);
}

.hero h1 {
  font-size: 2.6rem;
  color: white;
  margin-bottom: 15px;
  font-weight: 700;
}

.hero p {
  font-size: 1.1rem;
  opacity: 0.9;
  margin-bottom: 25px;
}

.hero-badges {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin-top: 20px;
}

.badge {
  display: inline-block;
  padding: 6px 14px;
  border-radius: 30px;
  font-size: 0.85rem;
  font-weight: 600;
  color: white;
  box-shadow: var(--shadow);
  transition: var(--transition);
}

.badge:hover {
  transform: translateY(-2px);
  box-shadow: var(--shadow-lg);
}

.badge-primary { background-color: var(--primary); }
.badge-secondary { background-color: var(--secondary); }
.badge-success { background-color: var(--success); }
.badge-info { background-color: var(--info); }
.badge-warning { background-color: var(--warning); color: var(--dark); }
.badge-danger { background-color: var(--danger); }
.badge-gold { background-color: var(--accent-gold); color: var(--dark); }

/* Section Styles */
.section {
  background: white;
  border-radius: var(--border-radius-lg);
  box-shadow: var(--shadow);
  padding: 35px;
  margin-bottom: 30px;
  transition: var(--transition);
  position: relative;
  overflow: hidden;
}

.section:hover {
  box-shadow: var(--shadow-lg);
  transform: translateY(-5px);
}

.section::before {
  content: '';
  position: absolute;
  top: 0;
  right: 0;
  width: 150px;
  height: 150px;
  background: linear-gradient(135deg, var(--accent-soft) 0%, rgba(255,255,255,0) 100%);
  border-radius: 0 0 0 100%;
  opacity: 0.6;
  z-index: 0;
}

.section-title {
  position: relative;
  padding-bottom: 15px;
  margin-bottom: 25px;
  color: var(--primary);
  font-size: 1.8rem;
  z-index: 1;
}

.section-title::after {
  content: '';
  position: absolute;
  left: 0;
  bottom: 0;
  height: 4px;
  width: 60px;
  background: linear-gradient(to right, var(--accent-gold), var(--accent));
  border-radius: 2px;
}

.section-content {
  position: relative;
  z-index: 1;
}

/* Two Column Layout */
.two-column {
  display: flex;
  gap: 30px;
  margin: 40px 0;
}

.column {
  flex: 1;
  min-width: 250px;
}

/* Skills Section */
.skills-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(160px, 1fr));
  gap: 15px;
  margin-top: 25px;
}

.skill-item {
  background-color: var(--light);
  border-radius: var(--border-radius);
  padding: 15px;
  text-align: center;
  transition: var(--transition);
  border-bottom: 3px solid var(--accent);
}

.skill-item:hover {
  transform: translateY(-3px);
  box-shadow: var(--shadow);
  border-bottom-color: var(--accent-gold);
}

.skill-icon {
  font-size: 1.8rem;
  color: var(--primary);
  margin-bottom: 10px;
}

.skill-name {
  font-weight: 500;
}

/* Education Cards */
.education-cards {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 20px;
  margin-top: 30px;
}

.education-card {
  background: var(--light);
  border-radius: var(--border-radius);
  padding: 25px;
  transition: var(--transition);
  position: relative;
  overflow: hidden;
  border-left: 4px solid var(--accent);
}

.education-card:hover {
  transform: translateY(-5px);
  box-shadow: var(--shadow);
}

.education-date {
  display: inline-block;
  background: var(--accent-soft);
  color: var(--primary);
  padding: 5px 12px;
  border-radius: 20px;
  font-size: 0.85rem;
  font-weight: 500;
  margin-bottom: 15px;
}

.education-degree {
  font-weight: 600;
  color: var(--dark);
  margin-bottom: 5px;
  font-size: 1.1rem;
}

.education-institution {
  color: var(--text);
  margin-bottom: 15px;
  font-style: italic;
}

/* Project Cards */
.project-cards {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
  gap: 25px;
  margin-top: 30px;
}

.project-card {
  background: white;
  border-radius: var(--border-radius);
  overflow: hidden;
  box-shadow: var(--shadow);
  transition: var(--transition);
}

.project-card:hover {
  transform: translateY(-5px);
  box-shadow: var(--shadow-lg);
}

.project-image {
  width: 100%;
  height: 180px;
  object-fit: cover;
  border-bottom: 3px solid var(--accent);
  transition: var(--transition);
}

.project-card:hover .project-image {
  border-bottom-color: var(--accent-gold);
}

.project-content {
  padding: 20px;
}

.project-title {
  font-weight: 600;
  color: var(--primary);
  margin-bottom: 10px;
  font-size: 1.2rem;
}

.project-description {
  margin-bottom: 15px;
  font-size: 0.95rem;
}

.project-badges {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin-bottom: 15px;
}

.project-badge {
  font-size: 0.75rem;
  padding: 4px 10px;
}

/* Highlight Box */
.highlight-box {
  background-color: var(--accent-soft);
  border-left: 4px solid var(--accent);
  padding: 20px;
  margin: 25px 0;
  border-radius: 0 var(--border-radius) var(--border-radius) 0;
  box-shadow: var(--shadow-inner);
}

/* Lists */
.feature-list {
  list-style: none;
  padding-left: 5px;
  margin: 20px 0;
}

.feature-list li {
  position: relative;
  padding-left: 28px;
  margin-bottom: 12px;
}

.feature-list li::before {
  content: '\f00c';
  font-family: 'Font Awesome 6 Free';
  font-weight: 900;
  position: absolute;
  left: 0;
  color: var(--success);
}

/* Contact Buttons */
.contact-buttons {
  display: flex;
  flex-wrap: wrap;
  gap: 15px;
  margin-top: 30px;
}

.contact-btn {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 10px;
  background: white;
  color: var(--primary);
  padding: 12px 20px;
  border-radius: var(--border-radius);
  box-shadow: var(--shadow);
  transition: var(--transition);
  text-decoration: none;
  font-weight: 500;
}

.contact-btn:hover {
  transform: translateY(-3px);
  box-shadow: var(--shadow-lg);
  background: var(--primary);
  color: white;
}

.contact-btn i {
  font-size: 1.2rem;
}

/* Responsive Styles */
@media screen and (max-width: 992px) {
  .hero-content {
    flex-direction: column-reverse;
    text-align: center;
    gap: 30px;
  }
  
  .hero-image img {
    max-width: 220px;
  }
  
  .hero h1 {
    font-size: 2.2rem;
  }
  
  .hero-badges {
    justify-content: center;
  }
  
  .section-title::after {
    left: 50%;
    transform: translateX(-50%);
  }
  
  .section-title {
    text-align: center;
  }
}

@media screen and (max-width: 768px) {
  .hero {
    padding: 40px 30px;
  }
  
  .two-column {
    flex-direction: column;
  }
  
  .section {
    padding: 25px;
  }
  
  .hero h1 {
    font-size: 1.8rem;
  }
  
  .contact-buttons {
    justify-content: center;
  }
}

@media screen and (max-width: 576px) {
  .skills-grid {
    grid-template-columns: repeat(2, 1fr);
  }
  
  .education-cards, .project-cards {
    grid-template-columns: 1fr;
  }
  
  .hero-image img {
    max-width: 180px;
  }
}
</style>
</head>
<body>




<!-- About Me Section -->
<div class="section">
  <h2 class="section-title">About Me</h2>
  <div class="section-content">
    <p>I recently completed my Master’s in Mechatronics Engineering at Amirkabir University of Technology.
    For my master's research project I designed and built a 5-DOF robotic arm and used it for human to robot object handovers. My undergraduate research project was about "implementation of a haptic exoskeleton for teleoperation and virtual reality purposes".</p>
    
    
    <p>I am passionate about creating robotic systems that can interact safely and effectively with humans. My academic and research journey has equipped me with a unique blend of mechanical design, electronics, and programming skills.</p>
    
    <p>I have hands-on experience bringing a robot from conception to reality by developing both the hardware and software components. I enjoy the design process and creating robotic systems that can work in harmony with humans.</p>
    
    <div class="highlight-box">
      <p><strong>My Vision:</strong> To develop accessible robotic systems that enhance human capabilities through intuitive interaction and safe collaboration.</p>
    </div>
    
    <h3 style="margin-top: 30px; color: var(--secondary);">Key Research Interests</h3>
    
    <li><strong>Human-Robot Interaction, Robotic Manipulation, Robot Perception</strong> </li>
      
      
    
  </div>
</div>

<!-- Projects Showcase -->
<div class="section">
  <h2 class="section-title">Featured Projects</h2>
  <div class="section-content">
    <div class="project-cards">
      <div class="project-card">
        <img class="project-image" src="/graduate/images/robotarmhandover500300.png?text=5-DOF Robotic Arm" alt="5-DOF Robotic Arm">
        <div class="project-content">
          <div class="project-title">Interactive Robotic Arm for HRI</div>
          <div class="project-badges">
            <span class="badge project-badge badge-info">Computer Vision</span>
            <span class="badge project-badge badge-primary">Mechanical Design</span>
            <span class="badge project-badge badge-warning">Manipulation</span>
          </div>
          <div class="project-description">Designed and built a custom 5-DOF robotic arm for human to robot object handover interactions, incorporating computer vision and safety features.</div>
          <a href="/graduate/" class="btn btn-outline">View Project</a>
        </div>
      </div>
      
      <div class="project-card">
        <img class="project-image" src="/_pages/ugrad/images/exoskeleton500300.png?text=Haptic Exoskeleton" alt="Haptic Exoskeleton">
        <div class="project-content">
          <div class="project-title">Haptic Exoskeleton</div>
          <div class="project-badges">
            <span class="badge project-badge badge-secondary">Teleoperation</span>
            <span class="badge project-badge badge-danger">Haptics</span>
            <span class="badge project-badge badge-success">Virtual Reality</span>
          </div>
          <div class="project-description">Implemented a haptic exoskeleton for teleoperation and virtual reality applications, providing tactile feedback to users.</div>
          <a href="/_pages/ugrad" class="btn btn-outline">View Project</a>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- Skills Section -->
<div class="section">
  <h2 class="section-title">Technical Skills</h2>
  <div class="section-content">
    <div class="skills-grid">
      <div class="skill-item">
        <div class="skill-icon"><i class="fas fa-robot"></i></div>
        <div class="skill-name">Robotics</div>
      </div>
      <div class="skill-item">
        <div class="skill-icon"><i class="fas fa-code"></i></div>
        <div class="skill-name">Programming</div>
      </div>
      <div class="skill-item">
        <div class="skill-icon"><i class="fas fa-microchip"></i></div>
        <div class="skill-name">Electronics</div>
      </div>
      <div class="skill-item">
        <div class="skill-icon"><i class="fas fa-cogs"></i></div>
        <div class="skill-name">Mechanical Design</div>
      </div>
      <div class="skill-item">
        <div class="skill-icon"><i class="fas fa-eye"></i></div>
        <div class="skill-name">Computer Vision</div>
      </div>
      <div class="skill-item">
        <div class="skill-icon"><i class="fas fa-cubes"></i></div>
        <div class="skill-name">Prototyping</div>
      </div>
      <div class="skill-item">
        <div class="skill-icon"><i class="fas fa-brain"></i></div>
        <div class="skill-name">Machine Learning</div>
      </div>
      <div class="skill-item">
        <div class="skill-icon"><i class="fas fa-project-diagram"></i></div>
        <div class="skill-name">System Integration</div>
      </div>
    </div>
  </div>
</div>

<!-- Contact Section -->
<div class="section">
  <h2 class="section-title">Get In Touch</h2>
  <div class="section-content">
    <p>I'm always open to discussing robotics research, potential collaborations, or new opportunities. Feel free to reach out through any of the following channels:</p>
    
    <div class="contact-buttons">
      <a href="mailto:masoud.rahimi38@gmail.com" class="contact-btn">
        <i class="fas fa-envelope"></i>
        <span>Email</span>
      </a>
      <a href="https://www.linkedin.com/in/masoud-gorji/" class="contact-btn">
        <i class="fab fa-linkedin"></i>
        <span>LinkedIn</span>
      </a>

    </div>
  </div>
</div>

<script>
  // Add any JavaScript functionality you might need here
  document.addEventListener('DOMContentLoaded', function() {
    // Example: Animate elements on scroll
    // Add functionality as needed
  });
</script>

</body>
</html>