# Node-RED and Phidgets Experiments

This repository contains a collection of experiments using Node-RED to interface with various Phidgets devices.

## Folder Structure

- `documentation/`: General guides, manuals, and notes on Node-RED and Phidgets.
- `experiments/`: Individual, self-contained projects, each in its own subfolder.
    - `01-SONAR-DST1200_DISTANCE_SENSOR/`: Sonar sensor experiment.
    - `02-SPATIAL- MOT1101_0/`: Spatial sensor experiment.
    - `03-ENCODERS/`: Encoder experiment.
- `shared_flows/`: Reusable Node-RED flows and subflows.

## Getting Started

Each experiment folder contains a `flows/` directory with the Node-RED JSON file, and a `README.md` with instructions on how to set it up and run it.

## Hardware Used

- Phidgets VINT HUB0000_0
- Phidgets DST1200_0 Sonar Sensor
- Phidgets MOT1101_0 Spatial Sensor
- Phidgets Encoder
- ...

## Experiments

- **01-Sonar-DST1200_Distance_Sensor**: Reads distance data from a DST1200_0 sonar sensor and cleans the output for easy use.
    - [Flow File](experiments/01-SONAR-DST1200_DISTANCE_SENSOR/flows/basic_flow.json)
    - [Learn more](experiments/01-SONAR-DST1200_DISTANCE_SENSOR/README.md)

- **02-Spatial-MOT1101_0**: Captures acceleration data from a MOT1101_0 spatial sensor and visualizes X, Y, Z axes.
    - [Flow File](experiments/02-SPATIAL- MOT1101_0/flows/basic_flow.json)
    - [Learn more](experiments/02-SPATIAL- MOT1101_0/README.md)

- **03-Encoders**: Monitors position changes from Phidgets encoders, filtering out small movements.
    - [Flow File](experiments/03-ENCODERS/flows/Flow-1.json)
    - [Learn more](experiments/03-ENCODERS/README.md)

## Shared Flows

Reusable flows and subflows for Node-RED are stored in [shared_flows/](shared_flows/).

## Notes

- Node-RED modules used: `node-red-contrib-phidget22`, `node-red-node-smooth`, `node-red-dashboard`, `node-red-contrib-osc`.
- See each experiment’s folder for specific