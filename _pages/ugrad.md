---

title: "BSc Project"
excerpt: "BSc Project"
author_profile: true
redirect_from: 
  - /ugrad/
---
<style>
.video-container {
  max-width: 800px; /* constrain max width */
  position: relative;
  padding-bottom: 56.25%; /* 16:9 aspect ratio (9 / 16 = 0.5625 or 56.25%) */
  height: 0;
  overflow: hidden;
}

.video-container iframe {
  position: absolute;

  top: 0; 
  left: 0;
  right: 0;
  margin: auto;
  width: 70%;
  height: 70%;
}
</style>


<style>

.container {
  display: flex;
  flex-wrap: wrap; 
  padding: 0px;
}

.text {
  width: 60%;
  text-align: justify;
  
  padding-right: 20px; /* Add right padding to create space */
}

.image {
  width: 40%;
}
.image222 {
  width: 100%;
}
@media (max-width: 600px) {
  .text, .image {
    width: 100%;
    
    padding-right: 0; /* Remove padding on smaller screens */
  }
}
</style>



<div style="text-align: justify">For my undergraduate thesis, I worked on developing a two-fingered haptic exoskeleton along with a force-sensitive robotic gripper. The goal was to control a robotic arm in teleoperation applications. I also used it to enhance immersion in virtual environments.  </div>
<div class="text">
    <p> </p> 
  </div>


<div class="container">

  <div class="text">
    <p>The gripper was a 2-jaw parallel mechanism integrated with force sensitive resistors to measure contact forces during grasping.</p> 
  </div>

  <div class="image">
    <img src="images/EmbeddedImage1.jpg" alt="gripper image"> 
  </div>

</div>


<div class="container">

  <div class="text">
    <p>The exoskeleton was designed to be worn on the hand and relay forces experienced by the robotic gripper back to the user's fingertips. </p> 
  </div>

  <div class="image">
    <img src="images/EmbeddedImage2.png" alt="exo"> 
  </div>

</div>



<div class="container">

  <div class="text">
    <p>For teleoperation, a Kinect sensor (V2) tracked the user's hand position which was mapped to control the 4-DOF robotic arm. The exoskeleton allowed the user to control the gripper's movement and feel the forces applied by the gripper to the object it was grasping.</p> 
  </div>

  <div class="image">
    <img src="images/EmbeddedImage.png" alt="Robot image"> 
  </div>

</div>

<div class="text">
    <p> </p> 
  </div>

<div class="container">

  <div class="text">
    <p>Using Oculus Rift, Leap motion sensor, Kinect V2, and the exoskeleton, I made a virtual environment in Unity3D. As the user interacted with objects in the Unity simulation, the exoskeleton provided corresponding haptic feedback, enhancing immersion.</p> 
  </div>

  <div class="image">
    <img src="images/EmbeddedImage123.png" alt="vr hand image"> 
  </div>

</div>

<div class="image222">
    <img src="images/Annotation 2020-10-27 190614.png" alt="vr image"> 
</div>


Through this project, I gained valuable experience in mechatronic design, motion tracking, force feedback systems, and human-computer interaction. In the end, we published three papers and won three awards from this project.


Here is a video that shows how we used the exoskeleton to interact with objects in the VR environment:
<div class="video-container">
  <iframe src="https://www.youtube.com/embed/vwxGTvljvsQ" title="HEXON - a two-finger haptic exoskeleton" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div>