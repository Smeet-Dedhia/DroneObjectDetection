## Problem Statement
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
1. Load existing weights for SSD MobileNet, YOLO and RetinaNet.
2. Train these 3 models on the visDrone dataset.
3. Evaluate performance of all models on actual drone footage
4. Compare the models in terms of accuracy, speed and memory.
