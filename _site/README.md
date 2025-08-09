<style>
    .main-content {
        max-width: 1200px;
        margin: 0 auto;
    }
    .project-card {
        width: 1000px;
        border: 2px solid #ccc;
        border-radius: 10px;
        padding: 20px;
        margin: 30px auto;
        background-color: #f9f9f9;
        box-shadow: 0px 4px 10px rgba(0,0,0,0.05);
    }
    .project-header {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .project-header h2 {
        font-size: 24px;
        margin: 0;
    }
    .project-date {
        font-size: 14px;
        color: #666;
    }
    .project-images {
        display: flex;
        justify-content: center;       /* Center images horizontally */
        gap: 20px;                      /* Space between images */
        margin: 15px 0;
        flex-wrap: wrap;               /* Allows images to stack on small screens */
    }

    .project-images img {
        max-width: 45%;
        height: auto;
        border-radius: 5px;
        object-fit: contain;
    }
    .project-images-large {
        text-align: center;
        margin: 15px 0;
    }

    .project-images-large img {
        max-width: 90%;
        height: auto;
        border-radius: 5px;
    }
    table {
        width: 100%;
        border-collapse: collapse;
        margin-bottom: 2em;
    }

    th, td {
    padding: 10px;
    text-align: left;
    border-bottom: 1px solid #ccc;
    }

    th {
    background-color: #f5f5f5;
    }

    tr:hover {
    background-color: #f9f9f9;
    }
</style>



<body>
    <div class="container">
        <div>
            <p>I am currently a Robotics Engineer in the Autonomy team at Bgarage. I work on deploying software to drone hardware and QA simulation testing. <br><br>
            I graduated with a Masters in Mechanical Engineering from the University of Illinois at Urbana Champaign. I was a graduate research assistant in the Reliable Autonomy Group @ UIUC, focusing on mobile robotics with perception applications. I enjoy full stack robotics projects, working with both software and hardware.<br><br>
            In my free time I love to build and ride bikes. </p>
        </div>
    </div>
</body>

---

<h2>News</h2>

<table>
  <thead>
    <tr>
      <th>Date</th>
      <th>Update</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>2025-02-28</td>
      <td>Paper 'Lyapunov Perception Contracts for Operating Design Domain' accepted to L4DC 2025.</td>
    </tr>
    <tr>
      <td>2025-09-12</td>
      <td>Started Robotics Engineer position at Bgarage AI.</td>
    </tr>
    <tr>
      <td>2024-04-10</td>
      <td><a href="https://youtu.be/hpIQ-ZyIRGA" target="_blank">Video presentation</a> uploaded for ICRA 2024.</td>
    </tr>
    <tr>
      <td>2024-01-29</td>
      <td>Paper 'Learning-Based Perception Contracts and Applications' accepted to ICRA 2024.</td>
    </tr>
  </tbody>
</table>


<p style="text-align: center; font-size: 36px"> Past Projects</p>


<div class="project-card">
  <div class="project-header">
    <h2>Visual Tracking with Intermittent Visibility</h2>
    <span class="project-date">Fall 2024</span>
  </div>

  <div class="project-images">
    <img src="{{ 'images/agi_real.JPG' | relative_url }}" alt="drone_hardware" />
    <img src="{{ 'images/target_tracker_diagram.png' | relative_url }}" alt="figure1" />
  </div>

  <p>
    <br>
    <span style="font-size: 0.9em; color: #555;">
      <strong>
        “Visual Tracking with Intermittent Visibility: Switched Control Design and Implementation”
      </strong>
      <br>
      Yangge Li, Benjamin C Yang, and Sayan Mitra
      <br>
      <a href="https://arxiv.org/abs/2411.08144" target="_blank">arxiv link</a>
    </span>
    <br>
        Designed a Switched Visual Tracker (SVT) for drones that alternates between tracking and recovery modes to maintain target proximity and visibility despite intermittent vision loss. Using switched systems theory, we proved stability and optimized parameters for performance, achieving up to 45% lower tracking error and longer visibility than baseline methods on our custom 5inch quadcopters.
  </p>
</div>


<div class="project-card">
  <div class="project-header">
    <h2>UAV Simulation: Vision-based Closed Loop Navigation</h2>
    <span class="project-date">Fall 2023</span>
  </div>

<div class="project-images">
  <img src="{{ 'images/NeRF_decreasingLight.gif' | relative_url }}" alt="Decreasing Light GIF" />
  <img src="{{ 'images/NeRF_increasingFog.gif' | relative_url }}" alt="Increasing Fog GIF" />
</div>

  <p>
    <br>
    <span style="font-size: 0.9em; color: #555;">
      <strong>“Lyapunov Perception Contracts for Operating Design Domain”</strong> <br>
      Yangge Li, Chenxi Ji, Jai Anchalia, Yixuan Jia, Benjamin C Yang, Daniel Zhuang and Sayan Mitra
      <br>
      <em>L4DC 2025 </em> <br>
      <a href="https://mitras.ece.illinois.edu/research/2025/LPC_L4DC25.pdf" target="_blank">paper link</a>
    </span>
    <br>
        This work introduces Lyapunov Perception Contracts (LPC), a framework for specifying and verifying the stability of visual control systems that rely on deep learning for perception and state estimation. LPCs bridge the gap between complex environmental effects (e.g., lighting, weather) and the lack of formal specifications for neural networks. The method synthesizes stability guarantees from data and system models, and identifies safe operating domains for visual controllers. We demonstrated the use of the contract for automated landing system using both simulated and Google Earth imagery.
  </p>
</div>

<div class="project-card">
  <div class="project-header">
    <h2>UAV Landing Using Perception Contracts</h2>
    <span class="project-date">Spring 2023</span>
  </div>

<div class="project-images-large">
  <img src="{{ 'images/RAL_lighting.JPG' | relative_url }}" alt="UAV Landing Image" />
</div>


  <p>
    <br>
    <span style="font-size: 0.9em; color: #555;">
      <strong>“Learning-Based Perception Contracts and Applications”</strong>
      Dawei Sun, Benjamin C. Yang, Sayan Mitra<br>
      <em>ICRA 2024 </em> <br>
      <a href="https://arxiv.org/abs/2309.13515" target="_blank">arXiv link</a>
    </span>
    <br>
        Developed an Inverse Perception Contract (IPC) framework that learns to bound perception errors from data and uses these bounds for safe control. We applied this to a quadcopter vision-based-landing pipeline, the IPC-enabled controller achieved reliable autonomous landings despite perception inaccuracies, outperforming a baseline that failed under the same conditions.
  </p>
</div>


<div class="project-card">
    <div class="project-header"><h2>ME446 Project: 6DOF Manipulator Scripting</h2><span class="project-date">Spring 2023</span></div>
    <div class="project-images-large">
        <img src="{{ 'images/ME446_robotpath.gif' | relative_url }}" alt="zigzag" />
    </div>
    <p>Created C++ scripting for 6 DOF manipulator using task space PD and feed forward control tracking, force control, and impedance control.</p>
</div>

<!-- <div class="project-card">
    <div class="project-header"><h2>Automated Needle Insertion Mechanism for Needle Tribology</h2><span class="project-date">Fall 2022</span></div>
    <div class="project-images"><img src="images/needle_tribology_assembly.png" alt="Image 1" /> <img src="images/needle_closeup.png" alt="Image 2" /></div>
    <p>Designed setup for controlled and repeatable study of needle insertion forces. Commissioned by Dr. Alison Dunn for research use.</p>
</div> -->

<div class="project-card">
    <div class="project-header"><h2>ECE484 Project: Carla Simulator</h2><span class="project-date">Fall 2022</span></div>
    <div class="project-images"><img src="{{ "images/ECE484_evasion.gif" | prepend: site.baseurl | prepend: site.url}}" alt="zigzag" /> <img src="{{ "images/ECE484_track.gif" | prepend: site.baseurl | prepend: site.url}}" alt="zigzag" /></div>
    <p>Developed python-based aggressive and real-time controller for autonomous racing in Carla simulator using PD control. Created custom PRM-variant for dynamic obstacle avoidance.</p>
</div>

<div class="project-card">
    <div class="project-header"><h2>ME461 Project: Segbot</h2><span class="project-date">Fall 2024</span></div>
    <div class="project-images"><img src="{{ "images/segbot.gif" | prepend: site.baseurl | prepend: site.url}}" alt="zigzag" /></div>
    <p>C program implementation of balancing segbot on Texas Instruments LAUNCHXL-F28379D.<br><a href="https://www.hackster.io/513006/me-461-final-project-self-erecting-and-navigating-robot-9fbbdc">Detail Build</a> | <a href="https://github.com/JFiore31/ME461_repo/tree/e65d09bec3acffd1f8a8c2669753008c1a189d73/workspace/Final%20Project">GitHub Link</a></p>
</div>

<!-- <div class="project-card">
    <div class="project-header"><h2>Design and Clinical Validation of a Robotic Ankle-Foot Simulator for Ankle Clonus</h2><span class="project-date">Spring 2020</span></div>
    <div class="project-images"><img src="{{ "images/ankle_clonus_assembly.png" | prepend: site.baseurl | prepend: site.url}}" alt="zigzag" /></div>
    <p>Designed robotic ankle-foot simulator for consistent training of clinicians in neurological disease assessment.</p>
</div> -->
<!-- 
<div class="project-card">
    <div class="project-header"><h2>Passive Hydraulic Simulator for Biceps Spasticity</h2><span class="project-date">Fall 2019</span></div>
    <div class="project-images"><img src="{{ "images/bicep_spasticity_assembly.png" | prepend: site.baseurl | prepend: site.url}}" alt="zigzag" /></div>
    <p>Developed unpowered simulator replicating biceps spasticity response through adjustable hydraulic piston for clinician training.</p>
</div> -->

