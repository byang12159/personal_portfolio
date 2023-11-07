<head>
    <style>
        .image-container {
            display: flex;
            justify-content: space-between; /*Adjust this property to control spacing */
        }
        .image-container img {
            max-width: 45%; /* Adjust image width as needed*/
        }
    </style>
</head>

<head>
    <style>
        /* Add CSS styles here */
        .container {
            display: flex;
            align-items: center;
        }

        .image {
            flex: 1;
            margin-right: 15px; /* Adjust the margin as needed */
        }
    </style>
</head>

<body>
    <div class="container">
        <img src="{{ "images/IMG_1807.jpg" | prepend: site.baseurl | prepend: site.url}}" alt="zigzag" />
        <div>
            <h1>Benjamin C Yang</h1>
            <p>Hi, i am master in MechSE.</p>
        </div>
    </div>
</body>

<p style="text-align: center; font-size: 36px"> Past Projects</p>

<!-- NeRF Simulation -->
<body>
    <div class="image-container">
        <img src="{{ "images/NeRF_decreasingLight.gif" | prepend: site.baseurl | prepend: site.url}}" alt="zigzag" />
        <img src="{{ "images/NeRF_increasingFog.gif" | prepend: site.baseurl | prepend: site.url}}" alt="zigzag" />
    </div>
</body>

<div style="display: flex; justify-content: space-between;">
  <p style="text-align: center; font-size: 24px;">UAV Simulation: Vision-based Closed Loop Navigation</p>
  <p style="text-align: right;">Fall 2023</p>
</div>

Closed loop vision-based simulation for quadcopter. Images generated from NeRF model of the flying arena. Quadcopter running monte carlo particle filter localization. 

TACAS Submission 2024

<!-- RAL PAPER -->
<div style="text-align:center;">
    <img src="{{ "images/RAL_lighting.JPG" | prepend: site.baseurl | prepend: site.url}}" alt="zigzag" />
</div>

<div style="display: flex; justify-content: space-between;">
  <p style="text-align: center; font-size: 24px;">UAV Landing Using Perception Contracts</p>
  <p style="text-align: right;">Spring 2023</p>
</div>

Demonstrate learning-based approach that can automatically characterize the error of a perception module from data and use this for
safe control. The proposed approach constructs a perception contract (PC), which generates a set that contains the groundtruth
value that is being estimated by the perception module, with high probability.

The PC technique is applied for the vision pipeline in the UAV safe-landing scenario. A PC is trained from ground truth data. A controller is designed to utilize the PC. Experiments show that with the control algorihtm with learned PC can safely land the quadcopter despite error from the perception module, while the baseline algorithm without PC failed to do so.

ICRA Submission 2024


<div style="text-align:center;">
    <img src="{{ "images/ME446_robotpath.gif" | prepend: site.baseurl | prepend: site.url}}" alt="zigzag" />
</div>

<div style="display: flex; justify-content: space-between;">
  <p style="text-align: center; font-size: 24px;">ME446 Project Demo</p>
  <p style="text-align: right;">Spring 2023</p>
</div>

<body>
    <div class="image-container">
        <img src="{{ "images/ECE484_evasion.gif" | prepend: site.baseurl | prepend: site.url}}" alt="zigzag" />
        <img src="{{ "images/ECE484_track.gif" | prepend: site.baseurl | prepend: site.url}}" alt="zigzag" />
    </div>
</body>

<div style="display: flex; justify-content: space-between;">
  <p style="text-align: center; font-size: 24px;">ECE484 Project: Carla Simulator</p>
  <p style="text-align: right;">Fall 2022</p>
</div>

The simulation is part of the Generalized Racing Intelligence Competition (GRAIC). Given
ground-truth perception information, the focus of the project is on the planning and control of the vehicle. An aggressive and fast
controller is developed to complete the generalized race course in the shortest amount of time and evade the most number of obstacles.

The controller utilizes PRM-variant as its sampling strategy and finds shortest path by performing topological sort in a directed acyclic graph.

Lateral control of the car is based on a PD controller.
For longditudinal control, the acceleration is based on path curvature. Using the current position of the car and the next two waypoints on our
path, we calculated the radius of the circle generated from those three points. The radius of the circle tells us how much curvature is coming up in our path. We tuned a logarithm relationship between the radius and desired vehicle speed
