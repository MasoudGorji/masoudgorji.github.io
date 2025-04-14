---
layout: archive
#title: "BSc Project"
#excerpt: "BSc Project"
author_profile: true
redirect_from: 
  - /ugrad/
---
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Masoud Rahimi Gorji | Haptic Exoskeleton for VR & Teleoperation</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        /* Color Palette - Immersive Haptics Theme */
        :root {
            --primary: #2E3192;         /* Deep Purple Blue */
            --secondary: #6A5ACD;       /* Slate Blue */
            --accent: #9370DB;          /* Medium Purple */
            --accent-teal: #20B2AA;     /* Light Sea Green */
            --accent-soft: #E6E6FA;     /* Lavender */
            --light: #F8F9FF;           /* Off-White with slight blue tint */
            --dark: #1A1A2E;            /* Very Dark Blue Purple */
            --text: #2F3640;            /* Dark Slate */
            --success: #27AE60;         /* Green */
            --info: #3498DB;            /* Blue */
            --warning: #F39C12;         /* Orange */
            --danger: #E74C3C;          /* Red */
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

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: var(--font-body);
            line-height: 1.7;
            color: var(--text);
            background-color: var(--light);
            max-width: 1800px;
            margin: 0 auto;
            padding: 0 20px;
            overflow-x: hidden;
        }

        h1, h2, h3, h4, h5, h6 {
            font-family: var(--font-heading);
            font-weight: 600;
            line-height: 1.3;
            color: var(--dark);
        }

        p {
            margin-bottom: 1rem;
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
        }

        .btn:hover {
            transform: translateY(-2px);
            box-shadow: var(--shadow-lg);
            background-color: var(--secondary);
        }

        .btn-outline {
            background-color: transparent;
            border: 2px solid var(--primary);
            color: var(--primary);
        }

        .btn-outline:hover {
            background-color: var(--primary);
            color: white;
        }

        /* Header Styles */
        .header {
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

        .header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: url("data:image/svg+xml,%3Csvg width='100' height='100' viewBox='0 0 100 100' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M11 18c3.866 0 7-3.134 7-7s-3.134-7-7-7-7 3.134-7 7 3.134 7 7 7zm48 25c3.866 0 7-3.134 7-7s-3.134-7-7-7-7 3.134-7 7 3.134 7 7 7zm-43-7c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zm63 31c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zM34 90c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zm56-76c1.657 0 3-1.343 3-3s-1.343-3-3-3-3 1.343-3 3 1.343 3 3 3zM12 86c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm28-65c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm23-11c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm-6 60c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm29 22c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zM32 63c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm57-13c2.76 0 5-2.24 5-5s-2.24-5-5-5-5 2.24-5 5 2.24 5 5 5zm-9-21c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM60 91c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM35 41c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2zM12 60c1.105 0 2-.895 2-2s-.895-2-2-2-2 .895-2 2 .895 2 2 2z' fill='%23ffffff' fill-opacity='0.05' fill-rule='evenodd'/%3E%3C/svg%3E");
            opacity: 0.8;
        }

        .header-content {
            position: relative;
            z-index: 2;
            max-width: 900px;
            margin: 0 auto;
        }

        .header h1 {
            font-size: 3rem;
            margin-bottom: 20px;
            color: white;
            text-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            line-height: 1.2;
        }

        .header p {
            font-size: 1.25rem;
            max-width: 800px;
            margin: 0 auto 30px;
            color: rgba(255, 255, 255, 0.9);
        }

        .badge {
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
        .badge-teal { background-color: var(--accent-teal); }

        .badges-container {
            margin: 20px 0;
            text-align: center;
        }

        /* Card and Section Styles */
        .card {
            background: white;
            border-radius: var(--border-radius-lg);
            box-shadow: var(--shadow);
            overflow: hidden;
            transition: var(--transition);
            margin-bottom: 30px;
        }

        .card:hover {
            box-shadow: var(--shadow-lg);
            transform: translateY(-5px);
        }

        .overview-section {
            display: flex;
            flex-wrap: wrap;
            margin: 60px 0;
            background: white;
            border-radius: var(--border-radius-lg);
            box-shadow: var(--shadow);
            overflow: hidden;
            transition: var(--transition);
        }

        .overview-section:hover {
            box-shadow: var(--shadow-lg);
        }

        .overview-content {
            flex: 1;
            padding: 50px;
            min-width: 300px;
        }

        .overview-image {
            flex: 1;
            min-width: 300px;
            position: relative;
            overflow: hidden;
        }

        .overview-image::before {
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

        .overview-image img {
            width: 100%;
            height: 100%;
            object-fit: contain; /* Changed from 'cover' to 'contain' */
            display: block;
            position: relative;
            z-index: 2;
            transition: var(--transition);
        }

        .overview-image:hover img {
            transform: scale(1.05);
        }

        .section-title {
            position: relative;
            padding-bottom: 15px;
            margin-bottom: 40px;
            color: var(--primary);
            font-size: 2.2rem;
        }

        .section-title::after {
            content: '';
            position: absolute;
            left: 0;
            bottom: 0;
            height: 4px;
            width: 80px;
            background: linear-gradient(to right, var(--accent-teal), var(--accent));
            border-radius: 2px;
        }

        .highlight-box {
            background-color: var(--accent-soft);
            border-left: 4px solid var(--accent);
            padding: 20px;
            margin: 25px 0;
            border-radius: 0 var(--border-radius) var(--border-radius) 0;
            box-shadow: var(--shadow-inner);
        }

        /* Technical Specs Styles */
        .technical-specs {
            margin: 60px 0;
            background: white;
            border-radius: var(--border-radius-lg);
            box-shadow: var(--shadow);
            padding: 40px;
            position: relative;
            overflow: hidden;
        }

        .technical-specs::before {
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

        .specs-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 30px;
            margin-top: 40px;
            position: relative;
            z-index: 1;
        }

        .spec-item {
            background-color: var(--light);
            border-radius: var(--border-radius);
            padding: 25px;
            transition: var(--transition);
            border-top: 4px solid var(--accent);
        }

        .spec-item:hover {
            transform: translateY(-5px);
            box-shadow: var(--shadow);
        }

        .spec-title {
            font-weight: 600;
            color: var(--primary);
            margin-bottom: 15px;
            font-size: 1.2rem;
            display: flex;
            align-items: center;
        }

        .spec-title i {
            margin-right: 10px;
            color: var(--accent-teal);
        }

        .spec-item ul {
            list-style: none;
            padding-left: 0;
        }

        .spec-item ul li {
            position: relative;
            padding-left: 20px;
            margin-bottom: 10px;
            line-height: 1.5;
        }

        .spec-item ul li::before {
            content: '→';
            position: absolute;
            left: 0;
            color: var(--secondary);
        }

        /* Feature Grid Styles */
        .features-section {
            padding: 60px 0;
        }

        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin: 40px 0;
        }

        .feature-card {
            background: white;
            border-radius: var(--border-radius-lg);
            box-shadow: var(--shadow);
            overflow: hidden;
            transition: var(--transition);
        }

        .feature-card:hover {
            transform: translateY(-5px);
            box-shadow: var(--shadow-lg);
        }

        .feature-image {
            height: 200px;
            overflow: hidden;
            position: relative;
        }

        .feature-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: var(--transition);
        }

        .feature-card:hover .feature-image img {
            transform: scale(1.05);
        }

        .feature-content {
            padding: 25px;
        }

        .feature-content h3 {
            font-size: 1.5rem;
            margin-bottom: 15px;
            color: var(--primary);
        }

        /* Applications Section Styles */
        .applications-section {
            background: white;
            padding: 50px;
            margin: 60px 0;
            border-radius: var(--border-radius-lg);
            box-shadow: var(--shadow);
            position: relative;
            overflow: hidden;
        }

        .applications-section::before {
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

        .applications-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            position: relative;
            z-index: 1;
        }

        .application-item {
            position: relative;
            background-color: var(--light);
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
            transition: var(--transition);
            overflow: hidden;
        }

        .application-item:hover {
            transform: translateY(-5px);
            box-shadow: var(--shadow-lg);
        }

        .application-image {
            height: 200px;
            overflow: hidden;
        }

        .application-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: var(--transition);
        }

        .application-item:hover .application-image img {
            transform: scale(1.05);
        }

        .application-content {
            padding: 25px;
        }

        .application-content h3 {
            color: var(--primary);
            margin-bottom: 15px;
            font-size: 1.3rem;
        }

        /* Video Section Styles */
        .video-section {
            background: white;
            border-radius: var(--border-radius-lg);
            box-shadow: var(--shadow);
            padding: 50px;
            margin: 60px 0;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .video-section::before {
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

        .video-section h2 {
            color: var(--primary);
            margin-bottom: 30px;
            position: relative;
            display: inline-block;
            padding-bottom: 15px;
            z-index: 1;
        }

        .video-section h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: linear-gradient(to right, var(--accent-teal), var(--accent));
            border-radius: 2px;
        }

        .video-section p {
            margin-bottom: 30px;
            max-width: 800px;
            margin-left: auto;
            margin-right: auto;
            position: relative;
            z-index: 1;
        }

        .video-container {
            max-width: 800px;
            position: relative;
            padding-bottom: 56.25%;
            height: 0;
            overflow: hidden;
            margin: 0 auto;
            border-radius: var(--border-radius);
            box-shadow: var(--shadow-lg);
            z-index: 1;
        }

        .video-container iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            border: none;
        }

        /* Results Section Styles */
        .results-section {
            background: white;
            border-radius: var(--border-radius-lg);
            box-shadow: var(--shadow);
            padding: 50px;
            margin: 60px 0;
            position: relative;
            overflow: hidden;
        }

        .results-section::before {
            content: '';
            position: absolute;
            bottom: 0;
            right: 0;
            width: 200px;
            height: 200px;
            background: linear-gradient(135deg, var(--accent-soft) 0%, rgba(255,255,255,0) 100%);
            border-radius: 100% 0 0 0;
            opacity: 0.8;
            z-index: 0;
        }

        .results-list {
            list-style-type: none;
            position: relative;
            z-index: 1;
        }

        .results-list li {
            position: relative;
            padding: 20px 25px;
            margin-bottom: 20px;
            background-color: var(--light);
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
            transition: var(--transition);
            display: flex;
            align-items: center;
        }

        .results-list li:hover {
            transform: translateY(-5px);
            box-shadow: var(--shadow-lg);
        }

        .results-list li i {
            font-size: 1.5rem;
            color: var(--accent-teal);
            margin-right: 15px;
        }

        /* Skills Section */
        .skills-section {
            margin: 60px 0;
        }

        .skills-cols {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .skills-col {
            background: white;
            border-radius: var(--border-radius-lg);
            box-shadow: var(--shadow);
            padding: 30px;
            transition: var(--transition);
        }

        .skills-col:hover {
            transform: translateY(-5px);
            box-shadow: var(--shadow-lg);
        }

        .skills-col h3 {
            color: var(--primary);
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 3px solid var(--accent-soft);
            display: inline-block;
        }

        .skills-list {
            list-style: none;
            padding: 0;
        }

        .skills-list li {
            margin-bottom: 12px;
            padding-left: 25px;
            position: relative;
        }

        .skills-list li::before {
            content: '\f00c';
            font-family: 'Font Awesome 6 Free';
            font-weight: 900;
            position: absolute;
            left: 0;
            color: var(--accent-teal);
        }

        /* Responsive Styles */
        @media screen and (max-width: 992px) {
            .header h1 {
                font-size: 2.5rem;
            }
            
            .overview-content {
                padding: 40px;
            }
        }

        @media screen and (max-width: 768px) {
            .header {
                padding: 60px 0 40px;
            }
            
            .header h1 {
                font-size: 2rem;
            }
            
            .header p {
                font-size: 1.1rem;
            }
            
            .section-title {
                font-size: 1.8rem;
            }
            
            .overview-content, .overview-image {
                flex: 100%;
            }
            
            .applications-section, .technical-specs, .video-section, .results-section {
                padding: 30px;
            }
        }

        @media screen and (max-width: 576px) {
            .header h1 {
                font-size: 1.8rem;
            }
            
            .badge {
                padding: 5px 10px;
                font-size: 0.8rem;
                margin: 5px 3px;
            }
            
            .specs-grid {
                grid-template-columns: 1fr;
            }
            
            .skill-header h3, .spec-title {
                font-size: 1.1rem;
            }
        }
    </style>
</head>
<body>
    <!-- Header Section -->
    <div class="header">
        <div class="header-content">
            <h1>HEXON: A Two-Finger Haptic Exoskeleton for Teleoperation & VR</h1>
            <p>My undergraduate thesis project that combines mechatronics, haptic feedback, and virtual reality to create immersive human-machine interaction experiences</p>
            
            <div class="badges-container">
                <span class="badge badge-primary">Haptic Feedback</span>
                <span class="badge badge-secondary">Virtual Reality</span>
                <span class="badge badge-info">Teleoperation</span>
                <span class="badge badge-success">Mechatronics</span>
                <span class="badge badge-warning">Motion Tracking</span>
                <span class="badge badge-danger">Human-Robot Interaction</span>
                <span class="badge badge-teal">Force Sensing</span>
            </div>
        </div>
    </div>

    <!-- Overview Section -->
    <div class="overview-section">
        <div class="overview-content">
            <h2 class="section-title">Project Overview</h2>
            <p>For my undergraduate thesis, I developed HEXON, a two-fingered haptic exoskeleton integrated with a force-sensitive robotic gripper. This dual-purpose system was designed to enable intuitive teleoperation of a robotic arm and enhance immersion in virtual reality environments.</p>
            
            <div class="highlight-box">
                <p><strong>Key Innovation:</strong> Creating a bi-directional haptic interface that allows users to not only control robotic or virtual hands but also feel realistic feedback when interacting with objects.</p>
            </div>
            
            <p>Through this project, I gained extensive experience in mechatronic design, motion tracking, force feedback systems, and human-computer interaction. The completed system demonstrated successful integration of multiple sensing modalities and real-time haptic rendering algorithms.</p>
            
            <a href="#video-section" class="btn">Watch Demonstration <i class="fas fa-arrow-right"></i></a>
        </div>
        <div class="overview-image">
            <img src="images/EmbeddedImage3.png" alt="HEXON Exoskeleton">
        </div>
    </div>

    <!-- Technical Specs Section -->
    <div class="technical-specs">
        <h2 class="section-title">System Components</h2>
        <div class="specs-grid">
            <div class="spec-item">
                <div class="spec-title"><i class="fas fa-hand-paper"></i> Haptic Exoskeleton</div>
                <ul>
                    <li>Linkage-based design for thumb and index finger</li>
                    <li>Dynamixel AX-12+ servo motors for force feedback</li>
                    <li>GY-25 IMUs for finger angle sensing</li>
                    <li>Lightweight, ergonomic design</li>
                    <li>Active force feedback capability</li>
                </ul>
            </div>
            <div class="spec-item">
                <div class="spec-title"><i class="fas fa-robot"></i> Force-Sensitive Gripper</div>
                <ul>
                    <li>Parallel-jaw mechanism</li>
                    <li>Four-bar linkage design</li>
                    <li>Force Sensing Resistors (FSRs)</li>
                    <li>Polynomial force calibration</li>
                    <li>Real-time force measurement</li>
                </ul>
            </div>
            <div class="spec-item">
                <div class="spec-title"><i class="fas fa-camera"></i> Sensing Systems</div>
                <ul>
                    <li>Microsoft Kinect v2 for body tracking</li>
                    <li>Oculus Rift for VR visualization</li>
                    <li>IMU-based joint angle measurement</li>
                    <li>FSRs for contact force detection</li>
                    <li>Kalman filtering for position data</li>
                </ul>
            </div>
            <div class="spec-item">
                <div class="spec-title"><i class="fas fa-code"></i> Software Architecture</div>
                <ul>
                    <li>Unity3D for VR environment</li>
                    <li>C# for Kinect SDK integration</li>
                    <li>Robot Operating System (ROS)</li>
                    <li>Arduino for sensor acquisition</li>
                    <li>Custom haptic rendering algorithms</li>
                </ul>
            </div>
        </div>
    </div>

    <!-- Features Section -->
    <div class="features-section">
        <h2 class="section-title">Key System Features</h2>
        <div class="features-grid">
            <div class="feature-card">
                <div class="feature-image">
                    <img src="images/EmbeddedImage.png" alt="Teleoperation System">
                </div>
                <div class="feature-content">
                    <h3>Intuitive Teleoperation</h3>
                    <p>The system allows users to remotely control a 4-DOF robotic arm using natural hand movements tracked by the Kinect sensor, while the exoskeleton provides tactile feedback of interaction forces experienced by the gripper.</p>
                </div>
            </div>
            <div class="feature-card">
                <div class="feature-image">
                    <img src="images/EmbeddedImage123.png" alt="VR Interaction">
                </div>
                <div class="feature-content">
                    <h3>Virtual Reality Integration</h3>
                    <p>Users can interact with virtual objects in Unity3D while receiving haptic feedback through the exoskeleton. The system supports different object types including stiff, soft, breakable, and explosive objects, each with unique haptic profiles.</p>
                </div>
            </div>
            <div class="feature-card">
                <div class="feature-image">
                    <img src="images/EmbeddedImage1.jpg" alt="Force Sensing">
                </div>
                <div class="feature-content">
                    <h3>Calibrated Force Sensing</h3>
                    <p>The robotic gripper incorporates FSRs that were carefully calibrated using physical scales to create accurate force mapping. This enables precise measurement of grasping forces for realistic haptic rendering.</p>
                </div>
            </div>
        </div>
    </div>

    <!-- Applications Section -->
    <div class="applications-section">
        <h2 class="section-title">Application Domains</h2>
        <div class="applications-grid">
            <div class="application-item">
                <div class="application-image">
                    <img src="images/Annotation 2020-10-27 190614.png" alt="VR Training">
                </div>
                <div class="application-content">
                    <h3>Immersive VR Training</h3>
                    <p>The system demonstrates potential for training applications where physical feel of objects is important, such as medical training, manufacturing, or hazardous operations.</p>
                </div>
            </div>
            <div class="application-item">
                <div class="application-image">
                    <img src="images/teleoperationfigure.png" alt="Remote Operation">
                </div>
                <div class="application-content">
                    <h3>Remote Robot Operation</h3>
                    <p>The teleoperation capability allows for intuitive control of robotic manipulators in environments that are dangerous, inaccessible, or require precision handling with force feedback.</p>
                </div>
            </div>
            <div class="application-item">
                <div class="application-image">
                    <img src="images/exoskeleton500300.png" alt="Rehabilitation">
                </div>
                <div class="application-content">
                    <h3>Rehabilitation Technology</h3>
                    <p>The exoskeleton and VR system could be adapted for physical therapy and rehabilitation applications (Serious Games), providing guided movements and resistance training.</p>
                </div>
            </div>
        </div>
    </div>

    <!-- Video Section -->
    <div class="video-section" id="video-section">
        <h2>System Demonstration</h2>
        <p>Watch how the HEXON exoskeleton provides haptic feedback as users interact with objects in the virtual reality environment, creating a truly immersive experience that engages both visual and tactile senses.</p>
        <div class="video-container">
            <iframe src="https://www.youtube.com/embed/vwxGTvljvsQ" title="HEXON - a two-finger haptic exoskeleton" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
        </div>
    </div>

    <!-- Results Section -->
    <div class="results-section">
        <h2 class="section-title">Project Outcomes</h2>
        <ul class="results-list">
            <li>
                <i class="fas fa-file-alt"></i>
                <div>
                    <strong>Published Research:</strong> The project resulted in three academic papers on haptic feedback and teleoperation systems.
                </div>
            </li>
            <li>
                <i class="fas fa-award"></i>
                <div>
                    <strong>Recognition:</strong> Received three awards for innovation and technical achievement in undergraduate research.
                </div>
            </li>
            <li>
                <i class="fas fa-check-circle"></i>
                <div>
                    <strong>Proof of Concept:</strong> Successfully demonstrated that affordable haptic systems can provide meaningful feedback for both virtual reality and teleoperation applications.
                </div>
            </li>
            <li>
                <i class="fas fa-lightbulb"></i>
                <div>
                    <strong>System Integration:</strong> Created a unique system that combined multiple sensing technologies (Kinect, Oculus, Leap Motion, IMUs, FSRs) into a cohesive user experience.
                </div>
            </li>
        </ul>
    </div>

    <!-- Skills Section -->
    <div class="skills-section">
        <h2 class="section-title">Skills & Competencies Demonstrated</h2>
        <div class="skills-cols">
            <div class="skills-col">
                <h3>Design & Fabrication</h3>
                <ul class="skills-list">
                    <li>Exoskeleton mechanism design</li>
                    <li>Parallel-jaw gripper design</li>
                    <li>Sensor integration design</li>
                    <li>Prototyping (cardboard, wood, 3D printing)</li>
                    <li>CAD modeling for mechanical components</li>
                </ul>
            </div>
            <div class="skills-col">
                <h3>Electronics & Control</h3>
                <ul class="skills-list">
                    <li>Sensor integration (Kinect, Leap Motion, Oculus, IMUs, FSRs)</li>
                    <li>Actuator control (Dynamixel servos)</li>
                    <li>Microcontroller programming (Arduino)</li>
                    <li>Force sensor calibration</li>
                    <li>Robotic arm control</li>
                </ul>
            </div>
            <div class="skills-col">
                <h3>Software Development</h3>
                <ul class="skills-list">
                    <li>VR development in Unity3D</li>
                    <li>Computer vision with Kinect SDK</li>
                    <li>Robot Operating System (ROS)</li>
                    <li>Data filtering and sensor fusion</li>
                    <li>Haptic rendering algorithms</li>
                </ul>
            </div>
        </div>
    </div>

    <script>
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>