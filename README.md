# Raksha-Kavach-Voice-Analysis-
Project Raksha Kavach: An Intelligent Personal Safety System
Raksha Kavach is a prototype for a personal safety system designed to provide a reliable and intelligent way for an individual to send an SOS alert in a moment of distress. It recognizes that in many real-world emergencies, a person may be unable to use their phone or even speak.

The system is built on a multi-modal approach, combining a physical hardware trigger with an intelligent analysis app, ensuring there is always a path to getting help.

Advantages of the System
Solves the "Noisy Place" Problem: The core of the system is the Raksha Ring, a discreet, wearable device. A simple button press sends a silent alert to the app. This is the primary trigger and works perfectly in loud environments (like a bus or market) or quiet places where speaking would attract unwanted attention. The user's direct, intentional action is the most reliable signal.

Intelligent Voice Analysis: For situations where a user cannot use their hands, the system features an advanced Voice AI Guardian. This isn't just a simple keyword spotter. It uses a multi-layered approach to analyze audio for universal distress signals, such as screams and shouts, making it more accurate and less prone to false alarms from normal conversation.

Robust Failsafe Design: The system is built with redundancy. If the AI detects a potential threat, it enters a "Pre-Alert" mode, asking the user for confirmation. If the user doesn't or can't respond within a short time, the system assumes the worst and automatically sends the full SOS alert. This ensures that even if the user is incapacitated, help is still called.

Privacy-Focused Architecture: The AI analysis is designed to run entirely on the user's device. This means raw audio from the microphone is not constantly being streamed to a cloud server, which is a critical design choice for protecting the user's privacy.

Key Resources Used
AI Models & Datasets:

Sound Event Detection: The system uses Google's pre-trained YAMNet (.tflite model) as the foundation for recognizing universal sounds like screams and crying.

Training Datasets: To create a more accurate custom model, the system is trained on publicly available audio datasets from Kaggle, such as the RAVDESS and UrbanSound8K datasets, to learn the difference between threatening and normal environmental sounds.

Software Libraries & Platforms:

AI Framework: TensorFlow Lite is used to run the machine learning models efficiently on a mobile device.

Audio Processing: Python libraries such as Librosa and Pydub are used to process and standardize the audio files for analysis.

Speech-to-Text: The SpeechRecognition library is used for the keyword spotting layer.

Training Platform: Google Colab is used as the free, cloud-based environment to run the Python script that trains the custom AI model.
