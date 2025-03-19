Real-Time Animal Sound Detection and Classification using Arduino Nano 33 BLE Sense

Overview

This project implements real-time animal sound detection and classification using the Arduino Nano 33 BLE Sense. It utilizes TensorFlow Lite models trained with Edge Impulse to classify animal sounds and make real-time decisions based on the detected class.

Features

Real-time sound classification using the onboard microphone.

Edge AI deployment with TensorFlow Lite for low-power inference.

Edge Impulse integration for model training and deployment.

Arduino Nano 33 BLE Sense for embedded processing.

Hardware Requirements

Arduino Nano 33 BLE Sense

Micro-USB cable for power and data transfer

Speaker or Buzzer (optional, for audible alerts)

LEDs (optional, for visual classification output)

Software Requirements

Arduino IDE (with necessary board packages and libraries)

Edge Impulse Studio (for training and exporting TensorFlow Lite models)

TensorFlow Lite for Microcontrollers

Arduino TensorFlow Lite Library

Project Structure

|-- EdgeImpulse_TFLite_Model/     # TensorFlow Lite model files
|-- Arduino_Code/                 # Arduino firmware
|-- Docs/                         # Documentation and references
|-- README.md                     # Project documentation

Getting Started

1. Clone the Repository

git clone https://github.com/codeshark304/Real-Time-Animal-sound-Detection-and-Classification-using-Arduino-Nano-33-BLE-Sense.git

2. Install Required Libraries

Ensure you have the following libraries installed in the Arduino IDE:

TensorFlow Lite for Microcontrollers

PDM (Pulse Density Modulation) Library (for microphone input)

3. Upload the Code to Arduino

Open Arduino_Code/animal_sound_classification.ino in the Arduino IDE.

Select the board Arduino Nano 33 BLE Sense.

Upload the sketch to the microcontroller.

4. Deploy the TensorFlow Lite Model

Train your custom model using Edge Impulse.

Download the TensorFlow Lite model (.tflite) and place it in the EdgeImpulse_TFLite_Model/ directory.

Convert and integrate it into the Arduino firmware.

Model Training (Edge Impulse)

Data Collection: Collect and upload animal sound samples to Edge Impulse.

Feature Engineering: Use the MFCC (Mel Frequency Cepstral Coefficients) processing block.

Model Training: Train a classification model using Edge Impulse’s AI pipeline.

Deployment: Export the trained model as TensorFlow Lite for Microcontrollers and integrate it into the Arduino code.

Usage

Power the Arduino Nano 33 BLE Sense.

Start real-time sound classification.

Observe results via Serial Monitor or LEDs/Buzzer.

Future Enhancements

Integrate BLE communication for remote monitoring.

Expand dataset for improved classification accuracy.

Deploy the model on different hardware platforms.

License

This project is open-source under the MIT License.

Acknowledgments

Edge Impulse for providing an easy-to-use AI training platform.

TensorFlow Lite for Microcontrollers for efficient AI inference.

Contact

For queries or contributions, feel free to raise an issue or submit a pull request in this repository.
