---
layout: archive
#title: "Master's Project"
#excerpt: "Master's Project"
author_profile: true
redirect_from:
  - /graduate
---

<!-- Styles specific to this page -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
<style>
    /* Import fonts at the top of stylesheet */
    @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Poppins:wght@400;500;600;700&display=swap');

    /* Color Palette - Luxurious Tech Theme */
    :root {
        --primary: #1E3A8A;         /* Deep Navy Blue */
        --secondary: #3563E9;       /* Bright Blue */
        --accent: #60A5FA;          /* Light Blue */
        --accent-gold: #F59E0B;     /* Gold */
        --accent-soft: #DBEAFE;     /* Very Light Blue */
        --light: #F8FAFC;           /* Off-White */
        --dark: #0F172A;            /* Very Dark Blue */
        --text: #334155;            /* Slate Gray */
        --success: #10B981;         /* Emerald */
        --info: #0EA5E9;            /* Sky Blue */
        --warning: #F59E0B;         /* Amber */
        --danger: #EF4444;          /* Red */
        --shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
        --shadow-lg: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
        --shadow-inner: inset 0 2px 4px 0 rgba(0, 0, 0, 0.06);
        --border-radius: 8px;
        --border-radius-lg: 12px;
        --transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        --font-heading: 'Poppins', sans-serif;
        --font-body: 'Inter', sans-serif;
    }

    /* Reset and Base Styles (Apply within the scope of this page content if needed,
       but ideally, base styles should be in the main site CSS) */
    .project-page-wrapper * { /* Scope styles to avoid conflicts if necessary */
        box-sizing: border-box;
        /* Avoid resetting margin/padding globally here if layout handles it */
    }

    .project-page-wrapper { /* Add a wrapper div around your content */
        font-family: var(--font-body);
        line-height: 1.7;
        color: var(--text);
        /* background-color: var(--light); Let layout handle background */
        max-width: 1800px; /* Or control width via layout */
        margin: 0 auto;
        padding: 0 20px; /* Adjust padding as needed */
        overflow-x: hidden;
    }

    .project-page-wrapper h1,
    .project-page-wrapper h2,
    .project-page-wrapper h3,
    .project-page-wrapper h4,
    .project-page-wrapper h5,
    .project-page-wrapper h6 {
        font-family: var(--font-heading);
        font-weight: 600;
        line-height: 1.3;
        color: var(--dark);
    }

    .project-page-wrapper p {
        margin-bottom: 1rem;
    }

    .project-page-wrapper .btn {
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
    }

    .project-page-wrapper .btn:hover {
        transform: translateY(-2px);
        box-shadow: var(--shadow-lg);
        background-color: var(--secondary);
    }

    .project-page-wrapper .btn-outline {
        background-color: transparent;
        border: 2px solid var(--primary);
        color: var(--primary);
    }

    .project-page-wrapper .btn-outline:hover {
        background-color: var(--primary);
        color: white;
    }

    /* Header Styles */
    .project-page-wrapper .header {
        position: relative;
        padding: 80px 0 60px;
        text-align: center;
        overflow: hidden;
        background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
        color: white;
        border-radius: 0 0 var(--border-radius-lg) var(--border-radius-lg);
        margin-bottom: 60px;
        box-shadow: var(--shadow-lg);
    }

    .project-page-wrapper .header::before {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-image: url("data:image/svg+xml,%3Csvg width='100' height='100' viewBox='0 0 100 100' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M11 18c3.866 0 7-3.134 7-7s-3.134-7-7-7-7 3.134-7 7 3.134 7 7 7zm48 25c3.866 0 7-3.134 7-7s-3.134-7-7-7-7 3.134-7 7 3.134 7 7 7zm-43-7c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zm63 31c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zM34 90c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zm56-76c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zM12 86c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm28-65c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm23-11c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm-6 60c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm29 22c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zM32 63c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm57-13c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm-9-21c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM60 91c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM35 41c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM12 60c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2z' fill='%23ffffff' fill-opacity='0.05' fill-rule='evenodd'/%3E%3C/svg%3E");
        opacity: 0.8;
    }

    .project-page-wrapper .header-content {
        position: relative;
        z-index: 2;
        max-width: 900px;
        margin: 0 auto;
    }

    .project-page-wrapper .header h1 {
        font-size: 3rem;
        margin-bottom: 20px;
        color: white;
        text-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        line-height: 1.2;
    }

    .project-page-wrapper .header p {
        font-size: 1.25rem;
        max-width: 800px;
        margin: 0 auto 30px;
        color: rgba(255, 255, 255, 0.9);
    }

    .project-page-wrapper .badge {
        display: inline-block;
        padding: 6px 14px;
        border-radius: 30px;
        font-size: 0.85rem;
        font-weight: 600;
        margin: 8px 5px;
        color: white;
        box-shadow: var(--shadow);
        transition: var(--transition);
    }

    .project-page-wrapper .badge:hover {
        transform: translateY(-2px);
        box-shadow: var(--shadow-lg);
    }

    .project-page-wrapper .badge-primary { background-color: var(--primary); }
    .project-page-wrapper .badge-secondary { background-color: var(--secondary); }
    .project-page-wrapper .badge-success { background-color: var(--success); }
    .project-page-wrapper .badge-info { background-color: var(--info); }
    .project-page-wrapper .badge-warning { background-color: var(--warning); color: var(--dark); }
    .project-page-wrapper .badge-danger { background-color: var(--danger); }
    .project-page-wrapper .badge-gold { background-color: var(--accent-gold); color: var(--dark); }

    .project-page-wrapper .badges-container {
        margin: 20px 0;
        text-align: center;
    }

    /* Card and Section Styles */
    .project-page-wrapper .card {
        background: white;
        border-radius: var(--border-radius-lg);
        box-shadow: var(--shadow);
        overflow: hidden;
        transition: var(--transition);
        margin-bottom: 30px;
    }

    .project-page-wrapper .card:hover {
        box-shadow: var(--shadow-lg);
        transform: translateY(-5px);
    }

    .project-page-wrapper .overview-section {
        display: flex;
        flex-wrap: wrap;
        margin: 60px 0;
        background: white;
        border-radius: var(--border-radius-lg);
        box-shadow: var(--shadow);
        overflow: hidden;
        transition: var(--transition);
    }

    .project-page-wrapper .overview-section:hover {
        box-shadow: var(--shadow-lg);
    }

    .project-page-wrapper .overview-content {
        flex: 1;
        padding: 50px;
        min-width: 300px;
    }

    .project-page-wrapper .overview-image {
        flex: 1;
        min-width: 300px;
        position: relative;
        overflow: hidden;
        display: flex; /* Added for centering */
        align-items: center; /* Added for centering */
        justify-content: center; /* Added for centering */
    }

    .project-page-wrapper .overview-image::before {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: linear-gradient(135deg, var(--accent) 0%, var(--secondary) 100%);
        opacity: 0.1;
        z-index: 1;
    }

    .project-page-wrapper .overview-image img {
        max-width: 100%; /* Use max-width */
        max-height: 100%; /* Use max-height */
        height: auto; /* Maintain aspect ratio */
        object-fit: contain;
        display: block;
        position: relative;
        z-index: 2;
        transition: var(--transition);
    }

    .project-page-wrapper .overview-image:hover img {
        transform: scale(1.05);
    }

    .project-page-wrapper .section-title {
        position: relative;
        padding-bottom: 15px;
        margin-bottom: 40px;
        color: var(--primary);
        font-size: 2.2rem;
    }

    .project-page-wrapper .section-title::after {
        content: '';
        position: absolute;
        left: 0;
        bottom: 0;
        height: 4px;
        width: 80px;
        background: linear-gradient(to right, var(--accent-gold), var(--accent));
        border-radius: 2px;
    }

    .project-page-wrapper .highlight-box {
        background-color: var(--accent-soft);
        border-left: 4px solid var(--accent);
        padding: 20px;
        margin: 25px 0;
        border-radius: 0 var(--border-radius) var(--border-radius) 0;
        box-shadow: var(--shadow-inner);
    }

    /* Timeline Styles */
    .project-page-wrapper .timeline-section {
        padding: 60px 0;
        position: relative;
    }

    .project-page-wrapper .timeline-container {
        position: relative;
        max-width: 1100px;
        margin: 0 auto;
    }

    .project-page-wrapper .timeline {
        position: relative;
    }

    .project-page-wrapper .timeline::before {
        content: '';
        position: absolute;
        width: 6px;
        background: linear-gradient(to bottom, var(--primary), var(--accent));
        top: 0;
        bottom: 0;
        left: 50%;
        margin-left: -3px;
        border-radius: 3px;
        box-shadow: var(--shadow);
    }

    .project-page-wrapper .timeline-item {
        padding: 15px 40px;
        position: relative;
        background-color: inherit;
        width: 50%;
        margin-bottom: 40px;
    }

    .project-page-wrapper .timeline-item::after {
        content: '';
        position: absolute;
        width: 28px;
        height: 28px;
        right: -14px;
        background-color: white;
        border: 4px solid var(--accent-gold);
        top: 20px;
        border-radius: 50%;
        z-index: 1;
        box-shadow: var(--shadow);
        transition: var(--transition);
    }

    .project-page-wrapper .timeline-item:hover::after {
        background-color: var(--accent-gold);
        transform: scale(1.2);
    }

    .project-page-wrapper .timeline-left {
        left: 0;
    }

    .project-page-wrapper .timeline-right {
        left: 50%;
    }

    .project-page-wrapper .timeline-left::before {
        content: " ";
        height: 0;
        position: absolute;
        top: 22px;
        width: 0;
        z-index: 1;
        right: 30px;
        border: medium solid var(--accent-soft);
        border-width: 10px 0 10px 10px;
        border-color: transparent transparent transparent var(--accent-soft);
    }

    .project-page-wrapper .timeline-right::before {
        content: " ";
        height: 0;
        position: absolute;
        top: 22px;
        width: 0;
        z-index: 1;
        left: 30px;
        border: medium solid var(--accent-soft);
        border-width: 10px 10px 10px 0;
        border-color: transparent var(--accent-soft) transparent transparent;
    }

    .project-page-wrapper .timeline-right::after {
        left: -14px;
    }

    .project-page-wrapper .timeline-content {
        padding: 30px;
        background-color: white;
        position: relative;
        border-radius: var(--border-radius-lg);
        box-shadow: var(--shadow);
        transition: var(--transition);
    }

    .project-page-wrapper .timeline-content:hover {
        box-shadow: var(--shadow-lg);
        transform: translateY(-5px);
    }

    .project-page-wrapper .timeline-content h3 {
        color: var(--primary);
        margin-bottom: 20px;
        font-size: 1.5rem;
        position: relative;
        padding-bottom: 10px;
    }

    .project-page-wrapper .timeline-content h3::after {
        content: '';
        position: absolute;
        left: 0;
        bottom: 0;
        height: 3px;
        width: 50px;
        background-color: var(--accent-gold);
        border-radius: 2px;
    }

    .project-page-wrapper .timeline-content img {
        width: 100%;
        border-radius: var(--border-radius);
        margin-top: 20px;
        box-shadow: var(--shadow);
        transition: var(--transition);
    }

    .project-page-wrapper .timeline-content img:hover {
        transform: scale(1.02);
    }

    /* Skills Grid Styles */
    .project-page-wrapper .skills-section {
        padding: 60px 0;
    }

    .project-page-wrapper .skills-grid {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
        gap: 25px;
        margin: 40px 0;
    }

    .project-page-wrapper .skill-card {
        background: white;
        border-radius: var(--border-radius-lg);
        box-shadow: var(--shadow);
        overflow: hidden;
        transition: var(--transition);
    }

    /* No hover effect needed if click toggles */
    /* .project-page-wrapper .skill-card:hover {
        transform: translateY(-5px);
        box-shadow: var(--shadow-lg);
    } */

    .project-page-wrapper .skill-header {
        background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
        color: white;
        padding: 20px 25px;
        cursor: pointer;
        position: relative;
        transition: var(--transition);
    }

    .project-page-wrapper .skill-header h3 {
        margin: 0;
        font-size: 1.3rem;
        color: white;
        display: flex; /* Align icon and text */
        align-items: center; /* Align icon and text */
    }
    .project-page-wrapper .skill-header h3 i {
        margin-right: 10px; /* Space between icon and text */
    }

    .project-page-wrapper .skill-header::after {
        content: '\f107'; /* Down arrow */
        font-family: 'Font Awesome 6 Free';
        font-weight: 900;
        position: absolute;
        right: 20px;
        top: 50%;
        transform: translateY(-50%);
        font-size: 1.2rem;
        transition: var(--transition);
    }

    .project-page-wrapper .skill-card.active .skill-header::after {
        transform: translateY(-50%) rotate(180deg); /* Up arrow */
    }

    .project-page-wrapper .skill-content {
        padding: 0 25px; /* Keep horizontal padding for transition */
        max-height: 0;
        overflow: hidden;
        transition: max-height 0.5s ease, padding-top 0.5s ease, padding-bottom 0.5s ease;
    }

    .project-page-wrapper .skill-card.active .skill-content {
        padding-top: 25px; /* Add padding back when active */
        padding-bottom: 25px;
        max-height: 1000px; /* Adjust if content is taller */
    }

    .project-page-wrapper .skill-list {
        list-style-type: none;
        padding-left: 0; /* Remove default padding */
    }

    .project-page-wrapper .skill-list li {
        margin-bottom: 12px;
        padding-left: 28px;
        position: relative;
    }

    .project-page-wrapper .skill-list li::before {
        content: '\f00c'; /* Checkmark */
        font-family: 'Font Awesome 6 Free';
        font-weight: 900;
        position: absolute;
        left: 0;
        color: var(--success);
    }

    /* Technical Specs Styles */
    .project-page-wrapper .technical-specs {
        margin: 60px 0;
        background: white;
        border-radius: var(--border-radius-lg);
        box-shadow: var(--shadow);
        padding: 40px;
        position: relative;
        overflow: hidden;
    }

    .project-page-wrapper .technical-specs::before {
        content: '';
        position: absolute;
        top: 0;
        right: 0;
        width: 200px;
        height: 200px;
        background: linear-gradient(135deg, var(--accent-soft) 0%, rgba(255,255,255,0) 100%);
        border-radius: 0 0 0 100%;
        opacity: 0.8;
        z-index: 0;
    }

    .project-page-wrapper .specs-grid {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
        gap: 30px;
        margin-top: 40px;
        position: relative;
        z-index: 1;
    }

    .project-page-wrapper .spec-item {
        background-color: var(--light);
        border-radius: var(--border-radius);
        padding: 25px;
        transition: var(--transition);
        border-top: 4px solid var(--accent);
    }

    .project-page-wrapper .spec-item:hover {
        transform: translateY(-5px);
        box-shadow: var(--shadow);
    }

    .project-page-wrapper .spec-title {
        font-weight: 600;
        color: var(--primary);
        margin-bottom: 15px;
        font-size: 1.2rem;
        display: flex;
        align-items: center;
    }

    .project-page-wrapper .spec-title i {
        margin-right: 10px;
        color: var(--accent-gold);
    }

    .project-page-wrapper .spec-item ul {
        list-style: none;
        padding-left: 0;
    }

    .project-page-wrapper .spec-item ul li {
        position: relative;
        padding-left: 20px;
        margin-bottom: 10px;
        line-height: 1.5;
    }

    .project-page-wrapper .spec-item ul li::before {
        content: '→';
        position: absolute;
        left: 0;
        color: var(--secondary);
    }

    /* Contributions Section Styles */
    .project-page-wrapper .contributions-section {
        background: white;
        padding: 50px;
        margin: 60px 0;
        border-radius: var(--border-radius-lg);
        box-shadow: var(--shadow);
        position: relative;
        overflow: hidden;
    }

    .project-page-wrapper .contributions-section::before {
        content: '';
        position: absolute;
        bottom: 0;
        left: 0;
        width: 200px;
        height: 200px;
        background: linear-gradient(135deg, var(--accent-soft) 0%, rgba(255,255,255,0) 100%);
        border-radius: 0 100% 0 0;
        opacity: 0.8;
        z-index: 0;
    }

    .project-page-wrapper .contributions-list {
        list-style-type: none;
        counter-reset: contrib-counter;
        position: relative;
        z-index: 1;
        padding-left: 0; /* Remove default padding */
    }

    .project-page-wrapper .contributions-list li {
        position: relative;
        padding: 25px 30px 25px 80px;
        margin-bottom: 25px;
        background-color: var(--light);
        border-radius: var(--border-radius);
        box-shadow: var(--shadow);
        transition: var(--transition);
    }

    .project-page-wrapper .contributions-list li:hover {
        transform: translateY(-5px);
        box-shadow: var(--shadow-lg);
    }

    .project-page-wrapper .contributions-list li::before {
        counter-increment: contrib-counter;
        content: counter(contrib-counter);
        position: absolute;
        left: 20px;
        top: 50%;
        transform: translateY(-50%);
        width: 45px;
        height: 45px;
        border-radius: 50%;
        background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
        color: white;
        text-align: center;
        line-height: 45px;
        font-weight: bold;
        font-size: 1.2rem;
        box-shadow: var(--shadow);
    }

    /* Final Demo Styles */
    .project-page-wrapper .final-demo {
        background: white;
        border-radius: var(--border-radius-lg);
        box-shadow: var(--shadow);
        padding: 50px;
        margin: 60px 0;
        text-align: center;
        position: relative;
        overflow: hidden;
    }

    .project-page-wrapper .final-demo::before {
        content: '';
        position: absolute;
        top: -50px;
        right: -50px;
        width: 200px;
        height: 200px;
        background: linear-gradient(135deg, var(--accent-soft) 0%, rgba(255,255,255,0) 100%);
        border-radius: 0 0 0 100%;
        opacity: 0.8;
        z-index: 0;
    }

    .project-page-wrapper .final-demo h2 {
        color: var(--primary);
        margin-bottom: 30px;
        position: relative;
        display: inline-block;
        padding-bottom: 15px;
        z-index: 1;
    }

    .project-page-wrapper .final-demo h2::after {
        content: '';
        position: absolute;
        bottom: 0;
        left: 50%;
        transform: translateX(-50%);
        width: 80px;
        height: 4px;
        background: linear-gradient(to right, var(--accent-gold), var(--accent));
        border-radius: 2px;
    }

    .project-page-wrapper .final-demo p {
        margin-bottom: 30px;
        max-width: 800px;
        margin-left: auto;
        margin-right: auto;
        position: relative;
        z-index: 1;
    }

    .project-page-wrapper .demo-video {
        max-width: 100%;
        border-radius: var(--border-radius);
        box-shadow: var(--shadow-lg);
        position: relative;
        z-index: 1;
        transition: var(--transition);
        display: block; /* Ensure it behaves like a block */
        margin: 0 auto; /* Center if needed */
    }

    .project-page-wrapper .demo-video:hover {
        transform: scale(1.02);
    }

    /* Footer Styles - Consider if layout handles this */
    .project-page-wrapper .footer {
        text-align: center;
        margin: 80px 0 40px;
        color: var(--text);
        position: relative;
        padding-top: 40px;
    }

    .project-page-wrapper .footer::before {
        content: '';
        position: absolute;
        top: 0;
        left: 50%;
        transform: translateX(-50%);
        width: 100px;
        height: 3px;
        background: linear-gradient(to right, var(--primary), var(--accent));
        border-radius: 2px;
    }

    .project-page-wrapper .footer a {
        color: var(--primary);
        text-decoration: none;
        transition: var(--transition);
        font-weight: 500;
        margin: 0 10px;
    }

    .project-page-wrapper .footer a:hover {
        color: var(--secondary);
    }

    .project-page-wrapper .social-links {
        margin: 20px 0;
    }

    .project-page-wrapper .social-links a {
        display: inline-flex;
        align-items: center;
        justify-content: center;
        width: 40px;
        height: 40px;
        border-radius: 50%;
        background-color: var(--accent-soft);
        color: var(--primary);
        margin: 0 5px;
        transition: var(--transition);
    }

    .project-page-wrapper .social-links a:hover {
        background-color: var(--primary);
        color: white;
        transform: translateY(-3px);
    }

    /* Collapsible Section Styles */
    .project-page-wrapper .collapsible-section {
        background: white;
        border-radius: var(--border-radius-lg);
        box-shadow: var(--shadow);
        margin: 60px 0;
        overflow: hidden; /* Important for max-height transition */
    }

    .project-page-wrapper .collapsible-header {
        background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
        color: white;
        padding: 20px 30px;
        cursor: pointer;
        position: relative;
        transition: var(--transition);
        display: flex; /* Ensure header takes full width */
        justify-content: space-between; /* Push icon to the right */
        align-items: center; /* Vertically center content */
    }

    .project-page-wrapper .collapsible-header h2 {
        margin: 0;
        color: white;
        display: flex;
        align-items: center;
    }

    .project-page-wrapper .collapsible-header h2 i {
        margin-right: 15px;
    }

    .project-page-wrapper .collapsible-header::after {
        content: '\f107'; /* Down arrow */
        font-family: 'Font Awesome 6 Free';
        font-weight: 900;
        /* position: absolute; Removed */
        /* right: 30px; Removed */
        /* top: 50%; Removed */
        /* transform: translateY(-50%); Removed */
        font-size: 1.5rem;
        transition: transform 0.3s ease; /* Only transition transform */
        flex-shrink: 0; /* Prevent icon from shrinking */
        margin-left: 15px; /* Space between title and icon */
    }

    .project-page-wrapper .collapsible-section.active .collapsible-header::after {
        transform: rotate(180deg); /* Up arrow */
    }

    .project-page-wrapper .collapsible-content {
        padding: 0 40px; /* Keep horizontal padding */
        max-height: 0;
        overflow: hidden;
        transition: max-height 0.5s ease, padding-top 0.5s ease, padding-bottom 0.5s ease;
    }

    .project-page-wrapper .collapsible-section.active .collapsible-content {
        padding-top: 40px; /* Add vertical padding back */
        padding-bottom: 40px;
        max-height: 5000px; /* Set a large enough max-height */
        /* height: auto; Avoid height: auto with transitions */
    }

    /* Responsive Styles */
    @media screen and (max-width: 992px) {
        .project-page-wrapper .header h1 {
            font-size: 2.5rem;
        }

        .project-page-wrapper .overview-content {
            padding: 40px;
        }

        .project-page-wrapper .skills-grid {
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
        }
    }

    @media screen and (max-width: 768px) {
        .project-page-wrapper .header {
            padding: 60px 0 40px;
        }

        .project-page-wrapper .header h1 {
            font-size: 2rem;
        }

        .project-page-wrapper .header p {
            font-size: 1.1rem;
        }

        .project-page-wrapper .section-title {
            font-size: 1.8rem;
        }

        .project-page-wrapper .timeline::before {
            left: 31px;
        }

        .project-page-wrapper .timeline-item {
            width: 100%;
            padding-left: 70px;
            padding-right: 25px;
            margin-bottom: 30px;
            left: 0 !important; /* Override inline style */
        }

         .project-page-wrapper .timeline-left::after,
         .project-page-wrapper .timeline-right::after {
            left: 18px;
        }

        /* .project-page-wrapper .timeline-right {
            left: 0%; Removed, handled by timeline-item override
        } */

        .project-page-wrapper .timeline-left::before,
        .project-page-wrapper .timeline-right::before {
            left: 60px;
            border-width: 10px 10px 10px 0;
            border-color: transparent var(--accent-soft) transparent transparent;
        }

        .project-page-wrapper .overview-content,
        .project-page-wrapper .overview-image {
            flex: 1 1 100%; /* Ensure they stack */
        }
         .project-page-wrapper .overview-image {
            margin-top: 30px; /* Add space when stacked */
         }


        .project-page-wrapper .contributions-section,
        .project-page-wrapper .technical-specs,
        .project-page-wrapper .final-demo {
            padding: 30px;
        }

        .project-page-wrapper .contributions-list li {
            padding: 20px 20px 20px 70px;
        }

        .project-page-wrapper .collapsible-section.active .collapsible-content {
            padding: 30px;
        }
        .project-page-wrapper .collapsible-content {
             padding: 0 30px; /* Match active horizontal padding */
        }
    }

    @media screen and (max-width: 576px) {
        .project-page-wrapper .header h1 {
            font-size: 1.8rem;
        }

        .project-page-wrapper .badge {
            padding: 5px 10px;
            font-size: 0.8rem;
            margin: 5px 3px;
        }

        .project-page-wrapper .specs-grid,
        .project-page-wrapper .skills-grid {
            grid-template-columns: 1fr;
        }

        .project-page-wrapper .skill-header h3,
        .project-page-wrapper .spec-title {
            font-size: 1.1rem;
        }

        .project-page-wrapper .contributions-list li::before {
            width: 35px;
            height: 35px;
            line-height: 35px;
            font-size: 1rem;
            left: 15px; /* Adjust position */
        }

        .project-page-wrapper .contributions-list li {
            padding-left: 60px; /* Adjust padding */
        }
         .project-page-wrapper .overview-content,
         .project-page-wrapper .collapsible-section.active .collapsible-content,
         .project-page-wrapper .technical-specs,
         .project-page-wrapper .final-demo,
         .project-page-wrapper .contributions-section {
            padding: 20px; /* Reduce padding on small screens */
         }
         .project-page-wrapper .collapsible-content {
             padding: 0 20px; /* Match active horizontal padding */
         }
         .project-page-wrapper .collapsible-header {
             padding: 15px 20px;
         }
    }
</style>

<!-- Wrap all your page content in a div for better CSS scoping -->
<div class="project-page-wrapper">

    <!-- Header Section -->
    <div class="header">
        <div class="header-content">
            <h1>Interactive Robotic Arm for Safe Human-Robot Handover</h1>
            <p>My master's thesis project demonstrating the design, fabrication, and implementation of a low-cost 5-DOF robotic arm with advanced perception and safety features</p>

            <div class="badges-container">
                <span class="badge badge-primary">Robotics</span>
                <span class="badge badge-secondary">Human-Robot Interaction</span>
                <span class="badge badge-info">Computer Vision</span>
                <span class="badge badge-success">Deep Learning</span>
                <span class="badge badge-warning">Mechanical Design</span>
                <span class="badge badge-danger">Prototyping</span>
                <span class="badge badge-gold">Object Perception</span>
            </div>
        </div>
    </div>

    <!-- Overview Section -->
    <div class="overview-section">
        <div class="overview-content">
            <h2 class="section-title">Project Overview</h2>
            <p>I successfully designed, built, and tested a complete low-cost 5-DOF robotic arm system specifically designed for safe human-robot object handover interactions. This project addressed the challenge of creating affordable yet capable robotic assistants for collaborative environments.</p>

            <div class="highlight-box">
                <p><strong>Key Innovation:</strong> Combining custom 3D-printed hardware with advanced perception systems to create a safe, interactive robotic platform at a fraction of the cost of commercial solutions.</p>
            </div>

            <p>The final system leverages custom cycloidal gearboxes, a hybrid motor approach, and deep learning-based perception to enable safe and reliable object handover from a human user, demonstrating that affordable robotics can achieve meaningful human-robot interaction.</p>

            <a href="#final-demo" class="btn">See Final Demonstration <i class="fas fa-arrow-right"></i></a>
        </div>
        <div class="overview-image">
            <!-- Make sure the image path is correct relative to your site root -->
            <img src="{{ '/graduate/images/hrhotrans.png' | relative_url }}" alt="Final Robot System">
        </div>
    </div>

    <!-- Technical Specs Section -->
    <div class="technical-specs">
        <h2 class="section-title">System Specifications</h2>
        <div class="specs-grid">
            <div class="spec-item">
                <div class="spec-title"><i class="fas fa-cogs"></i> Mechanical</div>
                <ul>
                    <li>5 Degrees of Freedom</li>
                    <li>Custom 3D-printed structure</li>
                    <li>Cycloidal gearboxes (2 arcmin backlash)</li>
                    <li>Parallel jaw gripper with silicone pads</li>
                    <li>Max payload: 2kg</li>
                    <li>Max reach: 74 cm (with gripper attached)</li>
                </ul>
            </div>
            <div class="spec-item">
                <div class="spec-title"><i class="fas fa-bolt"></i> Actuation</div>
                <ul>
                    <li>Brushless DC motors (Joints 1-4)</li>
                    <li>Stepper motor (Joint 5)</li>
                    <li>DC servo for gripper</li>
                    <li>ODrive controllers with FOC</li>
                    <li>Hall effect sensors for homing</li>
                </ul>
            </div>
            <div class="spec-item">
                <div class="spec-title"><i class="fas fa-eye"></i> Perception</div>
                <ul>
                    <li>Microsoft Kinect RGB-D camera</li>
                    <li>YOLOv8 hand segmentation model</li>
                    <li>GR-ConvNet grasp detection</li>
                    <li>Current sensing for object contact</li>
                </ul>
            </div>
            <div class="spec-item">
                <div class="spec-title"><i class="fas fa-code"></i> Software</div>
                <ul>
                    <li>Python-based control system</li>
                    <li>Deep learning-based perception</li>
                    <li>ikpy for inverse kinematics</li>
                    <li>URDF model for trajectory planning</li>
                </ul>
            </div>
        </div>
    </div>

    <!-- Development Journey Section (Collapsible) -->
    <!-- REMOVED 'active' class - let JS handle the initial state if needed, or keep it if it should always start open -->
    <div class="collapsible-section" id="development-journey">
        <div class="collapsible-header">
            <h2><i class="fas fa-tasks"></i> Development Journey</h2>
            <!-- The ::after pseudo-element will add the icon -->
        </div>
        <div class="collapsible-content">
            <div class="timeline-section"> <!-- Added wrapper for consistent padding -->
                <div class="timeline-container">
                    <div class="timeline">
                        <div class="timeline-item timeline-left">
                            <div class="timeline-content">
                                <h3>Project Inception</h3>
                                <p>Identifying the need for an affordable, safe robot for human-robot interaction research at my university.</p>
                                <div class="highlight-box">
                                    <p>"Since there were no human-safe robots available at our university, I had to design and build one myself."</p>
                                </div>
                            </div>
                        </div>
                        <div class="timeline-item timeline-right">
                            <div class="timeline-content">
                                <h3>Transmission System Design</h3>
                                <p>Designing and implementing custom cycloidal gearboxes for high efficiency and low backlash using 3D printed parts.</p>
                                <img src="{{ '/graduate/images/cyclovid.gif' | relative_url }}" alt="Cycloidal Gearbox Simulation">
                            </div>
                        </div>
                        <div class="timeline-item timeline-left">
                            <div class="timeline-content">
                                <h3>Initial Hardware Validation</h3>
                                <p>Building and testing the first two joints with verified backlash of just 2 arcmin (0.0344°), implementing thermal monitoring, and designing a parallel gripper with soft silicone pads.</p>
                                <p>After the tests were successful, the complete robot arm was designed as shown in the image below:</p>
                                <img src="{{ '/graduate/images/RobotDesign.png' | relative_url }}" alt="Hardware Testing">
                            </div>
                        </div>
                        <div class="timeline-item timeline-right">
                            <div class="timeline-content">
                                <h3>Hand Detection System</h3>
                                <p>Training a YOLOv8 model on the Egohands dataset to provide reliable hand segmentation, ensuring the robot can avoid grasping human fingers during handover.</p>
                                <img src="{{ '/graduate/images/Segmentationgif.gif' | relative_url }}" alt="Hand Segmentation">
                            </div>
                        </div>
                        <div class="timeline-item timeline-left">
                            <div class="timeline-content">
                                <h3>Grasp Detection System</h3>
                                <p>Implementing a robotic grasp detection system using GR-ConvNet, adapted to work with Kinect camera input for finding optimal grasp points on objects.</p>
                                <p>The hand mask from the segmentation was used to ensure no grasps are generated on the user's hand.</p>
                                <img src="{{ '/graduate/images/graspestimationpic.png' | relative_url }}" alt="Grasp Estimation">
                            </div>
                        </div>
                        <div class="timeline-item timeline-right">
                            <div class="timeline-content">
                                <h3>System Integration</h3>
                                <p>Integrating all hardware and software components into a complete, functional system capable of safely handling objects from humans.</p>
                                <img src="{{ '/graduate/images/robotarmhandovergpage.png' | relative_url }}" alt="System Integration">
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Skills Section -->
    <div class="skills-section">
        <h2 class="section-title">Skills & Competencies Demonstrated</h2>
        <div class="skills-grid">
            <!-- Skill cards remain the same, e.g.: -->
            <div class="skill-card">
                <div class="skill-header">
                    <h3><i class="fas fa-project-diagram"></i> Project Management</h3>
                </div>
                <div class="skill-content">
                    <ul class="skill-list">
                        <li><strong>Project Planning:</strong> Defining scope, objectives, milestones, and tasks</li>
                        <li><strong>Time Management:</strong> Scheduling tasks and ensuring timely completion</li>
                        <li><strong>Resource Management:</strong> Identifying required hardware, software, and materials</li>
                        <li><strong>Budget Management:</strong> Operating within financial constraints</li>
                        <li><strong>Problem Solving:</strong> Overcoming unforeseen challenges</li>
                    </ul>
                </div>
            </div>
            <div class="skill-card">
                <div class="skill-header">
                    <h3><i class="fas fa-dolly-flatbed"></i> Supply Chain & Logistics</h3>
                </div>
                <div class="skill-content">
                    <ul class="skill-list">
                        <li><strong>Component Sourcing:</strong> Identifying and selecting appropriate parts</li>
                        <li><strong>Vendor Negotiation:</strong> Securing favorable pricing and terms</li>
                        <li><strong>Procurement:</strong> Managing ordering and delivery of components</li>
                    </ul>
                </div>
            </div>
            <div class="skill-card">
                <div class="skill-header">
                    <h3><i class="fas fa-drafting-compass"></i> Mechanical Design</h3>
                </div>
                <div class="skill-content">
                    <ul class="skill-list">
                        <li>Robotic Arm Kinematics (DOF selection, DH parameters)</li>
                        <li>Mechanism Design (Gripper mechanism)</li>
                        <li>Gearbox Design (Cycloidal profile generation)</li>
                        <li>Design for Additive Manufacturing</li>
                        <li>CAD Modeling for 3D printing and URDF generation</li>
                    </ul>
                </div>
            </div>
            <div class="skill-card">
                <div class="skill-header">
                    <h3><i class="fas fa-chart-line"></i> Analysis & Simulation</h3>
                </div>
                <div class="skill-content">
                    <ul class="skill-list">
                        <li>Kinematic Analysis (Forward/inverse kinematics)</li>
                        <li>Dynamic Analysis (Newton-Euler method)</li>
                        <li>Stress Analysis for gearbox design</li>
                        <li>Tolerance Analysis for performance and fit</li>
                        <li>Workspace Analysis</li>
                    </ul>
                </div>
            </div>
            <div class="skill-card">
                <div class="skill-header">
                    <h3><i class="fas fa-cubes"></i> Fabrication & Testing</h3>
                </div>
                <div class="skill-content">
                    <ul class="skill-list">
                        <li>Additive Manufacturing / 3D Printing</li>
                        <li>Prototyping and iteration</li>
                        <li>Experimental Validation</li>
                        <li>Metrology and measurement</li>
                    </ul>
                </div>
            </div>
            <div class="skill-card">
                <div class="skill-header">
                    <h3><i class="fas fa-microchip"></i> Electronics & Control</h3>
                </div>
                <div class="skill-content">
                    <ul class="skill-list">
                        <li>Motor Selection and integration</li>
                        <li>Field-Oriented Control implementation</li>
                        <li>Sensor Integration (Kinect, Hall effect, encoders)</li>
                        <li>Current sensing for grasp detection</li>
                    </ul>
                </div>
            </div>
            <div class="skill-card">
                <div class="skill-header">
                    <h3><i class="fas fa-laptop-code"></i> Software & Algorithms</h3>
                </div>
                <div class="skill-content">
                    <ul class="skill-list">
                        <li>Computer Vision and image processing</li>
                        <li>Deep Learning model training and adaptation</li>
                        <li>Python-based robotics control</li>
                        <li>Algorithm design for safe grasp planning</li>
                    </ul>
                </div>
            </div>
            <div class="skill-card">
                <div class="skill-header">
                    <h3><i class="fas fa-sitemap"></i> Systems Engineering</h3>
                </div>
                <div class="skill-content">
                    <ul class="skill-list">
                        <li>System Integration across domains</li>
                        <li>Human-Robot Interaction principles</li>
                        <li>Safety Engineering for collaborative robots</li>
                    </ul>
                </div>
            </div>
        </div> <!-- End skills-grid -->
    </div> <!-- End skills-section -->


    <!-- Final Demo Section -->
    <div class="final-demo" id="final-demo">
        <h2>Final System Demonstration</h2>
        <p>The complete system successfully integrates custom hardware with perception and control software to enable safe object handover from a human user. The system detects both graspable objects and human hands, creates a safety mask to avoid grasping the user's hand, and calculates optimal grasp points and robot trajectories.</p>
        <!-- Use relative_url filter for Jekyll paths -->
        <img class="demo-video" src="{{ '/api/placeholder/800/450?text=System+Demonstration' | relative_url }}" alt="Final Handover Demonstration">

        <div style="margin-top: 40px;">
            <!-- Update links if they point to actual files/repos -->
            <a href="#" class="btn">Download Full Report <i class="fas fa-file-pdf"></i></a>
            <a href="#" class="btn btn-outline" style="margin-left: 15px;">View Source Code <i class="fab fa-github"></i></a>
        </div>
    </div>

    <!-- Contributions Section -->
    <div class="contributions-section">
        <h2 class="section-title">Key Contributions</h2>
        <ul class="contributions-list">
            <li>
                <strong>Low-Cost Interactive Robotic Arm System:</strong> Designed, built, and demonstrated a complete 5-DOF robotic arm capable of human-robot object handover at a significantly lower cost than commercial alternatives.
            </li>
            <li>
                <strong>Custom 3D-Printed Cycloidal Gearboxes:</strong> Successfully designed and fabricated custom cycloidal gearboxes with low backlash (2 arcmin), validating their suitability for precision robotics applications.
            </li>
            <li>
                <strong>Integrated Vision System for Safe Handover:</strong> Developed a perception system combining deep learning-based grasp detection and hand segmentation for ensuring safe human-robot interaction.
            </li>
            <li>
                <strong>Demonstration of Feasibility:</strong> Provided proof that affordable hardware combined with advanced software can yield a functional and safe interactive robot for collaborative tasks.
            </li>
            <li>
                <strong>Proxy Force Sensing Implementation:</strong> Showcased motor current sensing as a cost-effective alternative to direct tactile sensing for object contact detection.
            </li>
        </ul>
    </div>

    <!-- Footer Section - Consider moving to layout if it's site-wide -->
    <div class="footer">
         <div class="social-links">
            <!-- Add actual links -->
            <a href="#" aria-label="GitHub"><i class="fab fa-github"></i></a>
            <a href="#" aria-label="LinkedIn"><i class="fab fa-linkedin"></i></a>
            <a href="#" aria-label="Email"><i class="fas fa-envelope"></i></a>
        </div>
        <p>&copy; <span id="current-year"></span> Masoud Rahimi Gorji. All rights reserved.</p>
        <p>
            <a href="#">Home</a> |
            <a href="#">About</a> |
            <a href="#">Projects</a>
        </p>
    </div>

</div> <!-- End project-page-wrapper -->

<!-- JavaScript should be placed at the end, ideally loaded via the layout -->
<script>
    // Wait for the DOM to be fully loaded before running scripts
    document.addEventListener('DOMContentLoaded', function() {

        // --- Collapsible Section Logic ---
        const collapsibleHeaders = document.querySelectorAll('.collapsible-header');
        collapsibleHeaders.forEach(function(header) {
            header.addEventListener('click', function() {
                // Find the parent .collapsible-section and toggle the 'active' class
                const parentSection = this.closest('.collapsible-section');
                if (parentSection) {
                    parentSection.classList.toggle('active');
                } else {
                    console.error("Could not find parent .collapsible-section for", this);
                }
            });
        });

        // --- Skill Card Logic ---
        const skillHeaders = document.querySelectorAll('.skill-header');
        skillHeaders.forEach(function(header) {
            header.addEventListener('click', function() {
                // Find the parent .skill-card and toggle the 'active' class
                const parentCard = this.closest('.skill-card');
                if (parentCard) {
                    parentCard.classList.toggle('active');
                } else {
                     console.error("Could not find parent .skill-card for", this);
                }
            });
        });

        // --- Initial State Logic (Optional - Keep or Remove) ---

        // Development Journey: Decide if it should start open or closed.
        // If it should start open, add the 'active' class here or back in the HTML.
        // If it should start closed, ensure the 'active' class is NOT in the HTML and not added here.
        const devJourney = document.getElementById('development-journey');
        if (devJourney) {
             // Example: Start Development Journey open by default
             devJourney.classList.add('active');
             // Example: Start Development Journey closed by default (ensure HTML class is also removed)
             // devJourney.classList.remove('active');
        }


        // Skill Cards: Decide if some should start open based on screen width, or all start closed.

        // Option A: All skill cards start closed (remove the logic below)

        // Option B: Open first N skill cards based on screen width (Keep/Adapt the logic below)
        const skillCards = document.querySelectorAll('.skill-card');

        function setInitialSkillCardsState() {
            const screenWidth = window.innerWidth;
            let cardsToShow = 0; // Start with 0 open by default

            // Define how many cards to show based on screen width
            // Adjust these breakpoints and numbers as needed
            if (screenWidth >= 1200) {
                cardsToShow = 4; // Example: Open first 4 on large screens
            } else if (screenWidth >= 992) {
                cardsToShow = 3; // Example: Open first 3 on medium-large screens
            } else if (screenWidth >= 768) {
                 cardsToShow = 2; // Example: Open first 2 on medium screens
            } else {
                 cardsToShow = 1; // Example: Open first 1 on small screens
            }

            // Apply the 'active' class
            skillCards.forEach((card, index) => {
                if (index < cardsToShow) {
                    card.classList.add('active');
                } else {
                    card.classList.remove('active'); // Ensure others are closed
                }
            });
        }

        // Set initial state on load
        // setInitialSkillCardsState(); // Uncomment this line to enable Option B

        // Optional: Update on resize (can cause layout shifts, use with caution)
        // window.addEventListener('resize', setInitialSkillCardsState); // Uncomment this line to enable Option B resize updates


        // --- Footer Year ---
        const yearSpan = document.getElementById('current-year');
        if (yearSpan) {
            yearSpan.textContent = new Date().getFullYear();
        }

    }); // End DOMContentLoaded
</script>