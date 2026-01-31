HiveMind Release
Download required files for this beta version: Latest Release V1.0.1

🛡️ Getting Started Guide: HiveMind Tensor Desktop Welcome to the Distributed Artificial Intelligence engine for desktop. This guide will help you set up your processing "swarm" in just a few minutes.

1. 🖥️ Minimum System Requirements
To ensure smooth execution, please make sure your system meets the following:

Disk Space: At least 2 GB of free space for the installed program.

RAM: 8 GB minimum (16 GB recommended for loading large models directly into memory).

Architecture: Windows 10/11 64-bit (x64).

Processor: Intel Core i5 or AMD Ryzen 5 (minimum) to manage gRPC orchestration.

2. 📱 Requirements for Android Nodes
HiveMind leverages the power of your mobile devices to accelerate inference.

Android Version: 8.0 (Oreo) or higher.

Connection: Stable Wi-Fi network (same network as the PC) or USB cable connection (requires enabling USB Debugging).

Signed APK: Install Hivemind-Node-V1.0.1.apk on each device.

3. 📦 SDK Integration (SDK.zip)
If you are a developer, you can create your own AI scripts that utilize the swarm. Inside SDK.zip, you will find the necessary tools.

Included Files:
hivemind.py: Python file containing essential methods. Check the internal summaries for implementation details and purposes.

hivemind_pb2: Required for SDK communication. Do not move this out of the same path as hivemind.py.

hivemind_pb2_grpc: Required for SDK communication. Do not move this out of the same path as hivemind.py.

How to import the SDK into your project:
Extract the contents of SDK.zip into your project's root folder. A folder named hivemind_sdk will be created; this folder contains everything needed to function as a library.

Ensure communication dependencies are installed:

pip install grpcio protobuf numpy

Note: The SDK requires several libraries. A requirements.txt file is included with the necessary names and versions. We recommend creating a virtual environment (venv).

How to import the SDK in your code:
Check the YOLOv8Nano example inside the /Models folder for a brief guide on how to start importing the SDK correctly.

EXTRA NOTE: Currently, the inference application only accepts models converted to TensorFlow Lite (.tflite). The user is responsible for the training process and the target conversion (UINT8, INT8, FLOAT16, FLOAT32). Weights, data types, and responses must match for the project to function correctly.

4. 🚀 Practical Example: YOLOv8Nano (Computer Vision)
I have included a ready-to-use model: YoloV8NanoEjemplo.zip.

Model: yolov8n_float32.tflite.

Usage: Select this model from the HiveMind Desktop interface. Note that the first time you load a model, it may be slow; subsequent uses will be significantly faster.

Connect: Identify an available port (we recommend 50052) and start the Server.

Make Visible: Enable the environment so Android nodes can detect the server.

Configure: The system will show whether you are using your project's venv or global Python libraries. You can also input extra execution parameters as if you were using a terminal.

Execute: The system will perform a "Warming" process to notify nodes that work is coming.

Running: After a brief grace period, the application will execute your selected script in a separate thread.

Fun Fact: This example model can process images in milliseconds when the load is distributed across several phones.

5. Windows Application V1.0.0 (Beta)
Go to Releases > Assets and download the .exe file named HiveMind Core Setup 1.0.0. Install the software in a directory with read/write permissions. We recommend having 2GB of disk space available, as TensorFlow and communication libraries are quite large. We are working on reducing the volume without losing efficiency.

6. Installing the APK on Nodes
Install the signed APK Hivemind-Node-V1.0.1.apk. You must accept the minimum permissions required for operation. Rest assured, we do not share any data with third parties. You can read our Privacy Policy here: Privacy Policy Link.

🔒 Trust and Security
Data Protection: HiveMind operates 100% locally. Your models and data never leave your private network. Communication between the PC and mobile devices is encrypted and protected by unique session tokens.

APP QUICK GUIDE:
![GUIA1](https://github.com/user-attachments/assets/3de522cc-e554-475d-9f79-8d4c53b7d40c)
![GUIA2](https://github.com/user-attachments/assets/7ef571ad-688e-4aeb-85d6-0de1d2121ce1)
![GUIA3](https://github.com/user-attachments/assets/463055b9-2f87-4eac-9923-c9feb1667293)
![GUIA4](https://github.com/user-attachments/assets/32b724ce-5e52-4263-ba12-92e3d3282533)
![GUIA5](https://github.com/user-attachments/assets/5994674d-5b8c-43bb-b589-cb01d1632b2c)
![GUIAPERSONA](https://github.com/user-attachments/assets/96003939-7643-47f6-8545-22ae9040866e)

Examples APP Android with Metrics and info:

![2 - Inferencias ejemplp 1](https://github.com/user-attachments/assets/d8000e14-6c5a-46e5-90db-b3504bb34212)
![1 - Esperando modelo](https://github.com/user-attachments/assets/02ab91fd-45b1-4724-bdc6-eff7ed840bb8)
![4 - Desconectando](https://github.com/user-attachments/assets/5242dc39-bc08-4630-9647-5435469cced7)
![3 - Inferencias ejemplo 2](https://github.com/user-attachments/assets/d3468ea4-ef68-49cc-9d62-8e1e7a1c0511)
