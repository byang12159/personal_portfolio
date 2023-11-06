# personal_portfolio



<p style="text-align: center;"> ME446 Project Demo</p>
<div style="text-align:center;"> 
    <img src="{{ "images/ME446_robotpath.gif" | prepend: site.baseurl | prepend: site.url}}" alt="zigzag" />
</div>

<!-- add year of project  -->

<p style="text-align: center;"> ECE484 Project: Carla Simulator</p>

<head>
    <style>
        .image-container {
            display: flex;
            justify-content: space-between; /* Adjust this property to control spacing */
        }
        .image-container img {
            max-width: 45%; /* Adjust image width as needed */
        }
    </style>
</head>
<body>
    <div class="image-container">
        <img src="{{ "images/ECE484_evasion.gif" | prepend: site.baseurl | prepend: site.url}}" alt="zigzag" />
        <img src="{{ "images/ECE484_track.gif" | prepend: site.baseurl | prepend: site.url}}" alt="zigzag" />
    </div>
</body>

The simulation is part of the Generalized Racing Intelligence Competition (GRAIC). Given
ground-truth perception information, the focus of the project is on the planning and control of the vehicle. An aggressive and fast
controller is developed to complete the generalized race course in the shortest amount of time and evade the most number of obstacles.

The controller utilizes PRM-variant as its sampling strategy and finds shortest path by performing topological sort in a directed acyclic graph.

Lateral control of the car is based on a PD controller. 
For longditudinal control, the acceleration is based on path curvature. Using the current position of the car and the next two waypoints on our
path, we calculated the radius of the circle generated from those three points. The radius of the circle tells us how much curvature is coming up in our path. We tuned a logarithm relationship between the radius and desired vehicle speed
