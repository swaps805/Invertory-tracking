# Electronic Components Detection with YOLOv8 and Roboflow

This project leverages YOLOv8 and Roboflow to detect various electronic components in images. The goal is to accurately identify and and keep track of thses componenets in a confined space in realtime like (Arduino, DC motor, Servo motor, jumper wires, Ultrasound Sensor, etc)

## Features

- **Real-Time Detection**: Detect and classify electronic components in images and video streams.

- **YOLOv8**: A custom dataset was used  train YOLO v8 and leverage its state of the art capabilities

- **Roboflow Integration**: Easily manage datasets and training through Roboflow.

## Progress

- The model has been trained on around 800 images of various components. Components/Classes include:
  - Arduino UNO board
  - HW battery
  - Breadboard
  - DC motor
  - Jumper wires
  - LCD screen
  - Servo motor
  - Ultrasound sensor

- One major problem faced during real-time detection was **false positives** (such as faces and walls being identified as “battery” and “breadboard”, respectively).

- A potential solution for which is to increase the confidence threshold for such classes.
