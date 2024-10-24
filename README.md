# Face and Coffee Detection Application
This is an application that utilizes real-time face recognition and coffee cup detection. Upon recognizing the user, the application greets them with a personalized "Good morning" message, providing the current date, time, and weather information through the OpenWeatherMap API. 
After the greeting, the user is asked whether they want to create a daily agenda. If the user wishes to create it, they can give commands verbally, and it will be saved to a .txt file. 
If a coffee cup is detected on the user's desk or in their hands using YOLO technology, the application asks if they would like to hear the latest news headlines. If the user agrees, it reads the headlines aloud, keeping them informed while they enjoy their coffee.
## Features

- **Face Recognition**: Utilizes dlib and machine learning to accurately recognize the user's face, greeting them with a personalized morning message along with the current date, time, and weather information.
- **Coffee Cup Detection**: Identifies if a coffee cup is present on the user's desk or in their hands using YOLO (You Only Look Once) object detection.
- **Daily Agenda Creation**: Takes voice commands from the user and saves them to a .txt file.
- **Weather Information**: Displays current weather data, including temperature and conditions.
- **News Headlines**: Asks the user if they want to hear the latest headlines, reading them aloud if the user agrees.

## Technologies

This application is built using the following technologies:

- **Python**: The primary programming language for the application.
- **OpenCV**: A computer vision library used for image processing.
- **Dlib**: A toolkit for machine learning that includes face recognition capabilities.
- **YOLO (You Only Look Once)**: A real-time object detection system used for identifying coffee cups.
- **Text-to-Speech**: Enables the application to speak out loud using the `pyttsx3` library.
- **Speech Recognition**: Allows the application to understand voice commands.
- **APIs**: Provides real-time weather data and news headlines for the user.
  
## APIs Used

- **OpenWeatherMap API**: 
  - **Purpose**: Provides current weather data for the user's location.
  - **Documentation**: [OpenWeatherMap API](https://openweathermap.org/api)
  - **Features**: Current temperature, weather conditions, humidity, and more.
  
- **NewsAPI**: 
  - **Purpose**: Fetches the latest news headlines from various sources, including BBC.
  - **Documentation**: [NewsAPI](https://newsapi.org/)
  - **Features**: Provides news headlines and articles based on user preferences.
 
## Installation

### Requirements
- Python (version 3.6 or higher)
- OpenCV: For image processing
- Dlib: For face recognition capabilities
- YOLO (You Only Look Once): For real-time object detection
- Pyttsx3: For text-to-speech capabilities
- SpeechRecognition: For voice command recognition
- Requests: To make API calls for weather and news
- Numpy: For numerical operations

### Download Model Files

#### Dlib Model Files:
- `dlib_face_recognition_resnet_model_v1.dat`
- `shape_predictor_68_face_landmarks.dat`

#### YOLO Model Files:
- `yolov4.weights`
- `yolov4.cfg`
- `coco.names`

### Steps
To set up the application, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/ibrk92/faceObjectDetection.git
   cd faceObjectDetection
2. **Install Requirements**:
   ```bash
   pip install -r requirements.txt
   
4. **Run the Application**
   ```bash
   python main.py

### Note
Ensure you upload your own photos for the face recognition feature to work effectively.

