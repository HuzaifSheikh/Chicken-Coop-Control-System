#  Poultry System Enthalpy Optimization
This is an Android application that applies Artificial Neural Networks (ANNs) to monitor and optimize control parameters in chicken coop environments using inverse modeling techniques. Built for educational and experimental use, the app supports training, testing, and optimization workflows in a user-friendly mobile interface.

## Features
- Configure input/output layers, hidden nodes, and activation pipeline.
-  Ingest training and testing datasets for forward propagation and error analysis.
-  Solve inverse problems using ANN outputs to back-calculate optimal environmental inputs (e.g., temperature, humidity).
-  Fully functional Android app supporting data uploads and result exports.

## Requirements
- Android OS 11 or higher for APK-based deployment
- Windows OS with Android Studio for emulator-based execution
- Compatible with phones/tablets supporting file upload/download capability

## Installation Instructions
- Download ```InverseAI.apk``` from the project release.
- Install the APK on your Android 11+ device.
- Grant storage permissions if prompted.
- Windows (via Emulator)
  - Place the ```InverseAI``` folder in:
  - ```\AndroidStudioProjects\```
  - Open Android Studio and build the project.
  - Run the app through an Android Emulator with API level 30+.
- Launch the app and register a new user or login with existing credentials.
- Tap "ANN" to enter the model setup screen.
- Input model parameters
  - Input Nodes
  - Output Nodes
  - Hidden Layer 1 Nodes
  - Hidden Layer 2 Nodes
  - Leave fields empty to use default architecture.
- Upload a file named traindata.txt containing your training dataset.
- Tap "Train" to initiate the ANN training phase.
- Upload testdata.txt containing test samples.
- Tap "Run" to evaluate the ANN model on test data.
- Input inverse parameters
  - Number of Outputs
  - Output Targets (to optimize)
  - Number of Inputs
  - Input Bounds
  - Number of Optimization Runs
- Alternatively, upload a file named ```InverseUpload.txt``` with parameter definitions.
- Tap "Export" to download the optimized results to your device. Ensure the following filenames are used exactly as follows
  - ```traindata.txt``` – training phase
  - ```testdata.txt``` – testing phase
  - ```InverseUpload.txt``` – inverse optimization parameters

## Authors
Sheikh Huzaif
