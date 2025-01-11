---
title: "AIMM ICC"
date: 2024-05-10T20:28:35-04:00
draft: false
---
You can see Trine Universities overview of the project here: [Artificial Intelligence Maritime Manuever Intercollegiate Challenge](https://www.trine.edu/innovation-one/aimm/index.aspx). This project, as the name states, is a competition between Purdue Main Campus, Purdue Fort Wayne, Indiana University, Trine University, Rose-Hulman Institute of Technology, and Notre Dame. Every team got a completely hollowed out 12ft wooden boat along with a grant to transform the boat into an autonomous agent that could navigate an obstacle course. This was a (relatively) large project with around 15 active undergrads, 2 graduate students, and 2 professors on the team. The team was divided into 3 teams: computer vision, mechanical/electrical, and navigation. Computer vision team, which I led, was responsible for creating a system to detect buoys, rings, and a floating baby doll that was a part of the obstacle course. The mechanical electrical team was responsible for the physical mountings on the boat and making sure all systems had power to run. Lastly, the navigation team was responsible for navigating based off the computer vision detections (which had distance), GPS, and as a last resort remote control. 

<!--more-->

## Role
2023-2024: Computer Vision Team Lead

## Tech Stack
- Computer Vision
    - Python
    - Yolov8
    - Roboflow
    - Pytorch
    - Docker
    - CUDA 

## Pipeline
![CV Pipeline](/images/aimm_cv_pipeline.png)

## Results 
We published a technical report about our process as part of the judging for the AIMM competition. You can view the document [here](https://docs.google.com/document/d/e/2PACX-1vTYsToDpUohFNKVdY4i7hteEkqEoGSFKjM2ApVTrtP4zEd6Y9sWk9BbXpVzlFmIGOf4SvqyG4mYLFIM/pub). Due to Purdue getting a late start on the competiton (and extremely bad weather) we weren't able to score as well as we wanted in the competition. Despite this, we were able to get a fully remote controlled boat and a working computer vision system that was able to detect buoys, and based off their distance from the camera, calculate their GPS coordinates for our navigation system to use. We also placed 3rd in the presentation section of the competition which was based off our report and on-site presentation given to the judges. 

## Future
This was just the first year of the competition and we didn't really start until February for a competition that took place in April. This coming year we have almost half our team back and get to start in August for the competition. We have learned quite a bit and I am actually working with [Dr. Newell](https://www.purdue.edu/aatl/people/dr-brittany-newell/), one of the professors on the project, over the summer working on setting up the project for the coming year and doing research in the realm of reinforcement learning on the autonomous boat. As this project progresses, more updates will be added here. 


Jan 2024 - Current
