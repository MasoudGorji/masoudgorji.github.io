---

title: "Master's Project"
excerpt: "Master's Project"
author_profile: true
redirect_from: 
  - /grad
---


<style>

.container {
  display: flex;
  flex-wrap: wrap; 
  padding: 0px;
}

.text {
  width: 50%;
  text-align: justify;
  
  padding-right: 20px; /* Add right padding to create space */
}

.image {
  width: 50%;
}

@media (max-width: 600px) {
  .text, .image {
    width: 100%;
    
    padding-right: 0; /* Remove padding on smaller screens */
  }
}

/* other CSS */

</style> 




<div style="text-align: justify">For my master's thesis project, I chose to research human-robot object handovers. Since there were no human-safe robots available at our university, I had to design and build one myself. </div>



<div class="container">

  <div class="text">
    <p>I developed a low-cost 5-DOF robotic arm for the research. The first 4 joints use brushless DC motors and the last joint uses a stepper motor.
The final result will look like this:</p> 
  </div>

  <div class="image">
    <img src="images/robotshow.png" alt="Robot image"> 
  </div>

</div>

<div class="container">

  <div class="text">
    <p>For all of the joints, I used cycloidal gearboxes to have a high efficiency and a low backlash with 3d printed parts.
This is a simulation of how the first joint's gearbox works:</p> 
  </div>

  <div class="image">
    <img src="images/cyclovid.gif" alt="gearbox"> 
  </div>
</div>

<div style="text-align: justify">So far, I have built and tested the first 2 joints. The backlash on the first joint is just 2 arcmin (0.0344°), which meets the requirements for this project.to prevent the plastic parts from deforming, I am using thermistors to monitor the motor temperatures. I am using Hall effect sensors for homing the arm. I have also designed a parallel gripper with soft silicone pads in a grid pattern to gently grasp a variety of objects.</div>
<div style="text-align: justify"> '</div>
<div style="text-align: justify">On the software side, I trained a YOLOv8 model on the Egohands dataset to segment human hands. The model provides reliable hand detection for the robot so the gripper can avoid grasping the human fingers holding the object.</div>

<div style="text-align: justify">Overall, I have made significant progress in designing and prototyping a custom robot for my human-robot interaction research. Once completed, this platform will enable me to conduct novel experiments for my master's thesis. </div>


Here is a gif of the hand segmentation on a live webcam feed:
  <div class="image">
    <img src="images/Segmentationgif.gif" alt="handseggif"> 
  </div>


