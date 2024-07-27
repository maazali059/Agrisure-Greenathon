# Team Hydra (IRrigaScan)
## Project Overview
IRrigaScan is an innovative system designed to optimize irrigation scheduling and enhance early disease detection in agriculture using infrared (IR) imaging and machine learning (ML). This project aims to address the critical issue of water wastage in agriculture and improve crop health by providing precise and reliable data on plant water stress and early signs of disease.

## Problem Statement
Agriculture consumes 70% of global water resources, yet only 30% is used efficiently, leading to significant water wastage. Traditional methods for irrigation scheduling and disease detection rely on visual estimation and are prone to inaccuracies and late detection. Existing IoT solutions, such as soil moisture sensors, require maintenance and are susceptible to damage.

## Proposed Solution
IRrigaScan leverages IR imaging to estimate the Crop Water Stress Index (CWSI) for accurate irrigation scheduling and utilizes a machine learning model to detect plant diseases early by using thermal camera clubbed with Raspberry Pi and providing all data to farmer on his smartphone.

## Key Benefits
### High Accuracy:
Provides precise data on plant water stress and early disease signs.
### Low Maintenance: 
Eliminates the need for soil-contacting sensors, reducing maintenance and damage risks.
### Efficient and Reliable: 
Ensures timely irrigation and disease management, enhancing crop yield and sustainability.
### Targeted Water Use: 
Focuses on the plant’s water requirement, reducing water waste.
### Machine Learning Model: 
Trains on IR images to detect early signs of plant diseases, enabling timely intervention.

### Automated Monitoring: 
Minimal human intervention needed, allowing for consistent and reliable data collection.
Features

## How it Works
1) The crop image is first masked using Open CV to detect only the plant.

![RGB Mask](https://github.com/maazali059/Agrisure-Greenathon/blob/main/1.jpg?raw=true)

2) The IR image is then masked based on the RGB mask and the CWSI, and Disease is calculated using the ML model.

![IR Mask](https://github.com/maazali059/Agrisure-Greenathon/blob/main/2.jpg?raw=true)

3) This data is then used to trigger events using Raspberry Pi.

## Flow diagram
![Flowchart](https://github.com/maazali059/Agrisure-Greenathon/blob/main/Flowchart.png?raw=true)


