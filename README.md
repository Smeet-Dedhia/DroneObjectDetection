# Project DronAid
https://dronaid.in/about.html <br>
Project DronAid is a one-of-a-kind student project set in Manipal, India. We are making an effort to make healthcare more accessible and hassle-free. This will be achieved by creating an intelligent network of UAV systems that specialize in medical applications. By integrating Artificial Intelligence in Unmanned Aerial Vehicles and app development, we hope to bring about practical clinical applications and emergency services at a community level. We are a unique collaboration between the students and faculty of Manipal Institute of Technology (MIT) and Kasturba Medical College (KMC).

## AI Project for 2022-2023
Modern drones are equipped with cameras and are very prospective for a variety of commercial uses such as aerial 
photography, surveillance, etc. In order to massively deploy drones and further reduce their costs, it’s necessary to 
power drones with smart computer vision and autopilot. In the application of aerial photography, object detection 
and tracking are essential to capturing key objects in a scene.There are significant challenges with drones due to topdown view angles and real-time constraints. Additionally,The strong weight and area constraint of embedded 
hardware that limits the drones to run computation intensive algorithms, such as deep learning, with limited 
hardware resource

## Existing Models
Generally, we use Object Detection Models like YOLO, SSD Mobilenet & RetinaNet to detect objects.
When we Directly apply previous models to tackle object detection task on drone-captured scenarios we majorly 
face three problems.
1. First, the object scale varies violently because the flight altitude of drones change greatly.
2. Second, drone-captured images contain objects with high density, which brings in blockage between objects.
3. Third, drone-captured images always contain confusing geographic elements because of covering large area. 
These problems make the object detection of drone-captured images very challenging.

## Our Solution
We will train the existing Models using object-detection datasets (visDrone Dataset) that are specific to drones so 
that we can improve the accuracy of these models.

## Steps & Workflow:
1. Load & Preprocess the VisDrone dataset.
2. Load existing weights for SSD MobileNet, YOLO and RetinaNet.
3. Train these 3 models on the visDrone dataset.
4. Evaluate performance of all models on actual drone footage
5. Compare the models in terms of accuracy, speed and memory.

## Conlusion
While all models fail to detect all the objects, we can see that:
1. YOLO model has the maximum mAP score and hence has the best performance
2. RetinaNet model has middling mAP. It needs to trained on much more epochs which is not possible on colab.
3. SSD model has the least mAP. This is apparently becuase proper training of SSD requires 200+ hrs.
### Classwise MAP
![image](https://github.com/user-attachments/assets/494250f4-119f-46b0-8d7a-e04da4d8f0bf)
![image](https://github.com/user-attachments/assets/dc85936f-41c4-4243-b0a8-c01369d99a44)

