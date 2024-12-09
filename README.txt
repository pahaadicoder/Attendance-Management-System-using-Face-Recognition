# README.txt for Attendance Management System Using Face Recognition

## Project Title
**Attendance Management System Using Face Recognition**

## Description
This project implements an automated attendance management system that utilizes facial recognition technology to streamline the process of marking attendance. The system captures images of students through a webcam, recognizes their faces, and records their attendance in a structured manner. The user interface is built using Tkinter, providing a simple and intuitive experience for users.

## Features
- **Facial Recognition**: Automatically recognizes student faces and marks attendance.
- **Image Capture**: Allows users to capture images for training the recognition model.
- **Manual Attendance Entry**: Provides functionality for manual entry of attendance if needed.
- **Data Storage**: Saves student details and attendance records in CSV format.
- **Database Integration**: Supports storing attendance data in a MySQL database.
- **User-Friendly Interface**: Built with Tkinter for easy navigation and interaction.

## Requirements
To run this project, ensure you have the following installed:
- Python 3.x
- OpenCV (opencv-python and opencv-contrib-python)
- NumPy
- Pandas
- Tkinter (usually included with Python installations)
- MySQL or any other database for storing attendance records

## Installation Steps
1. Clone this repository to your local machine:
   ```
   git clone https://github.com/yourusername/AttendanceManagementSystem.git
   ```

2. Navigate to the project directory:
   ```
   cd AttendanceManagementSystem
   ```

3. Install the required Python packages:
   ```bash
   pip install opencv-python opencv-contrib-python numpy pandas pymysql
   ```

4. Ensure that the following directories exist:
   - `TrainingImage/` for storing training images.
   - `StudentDetails/` for storing student details.
   - `Attendance/` for saving attendance records.

5. Download the Haar Cascade file for face detection (`haarcascade_frontalface_default.xml`) and place it in the project directory.

## Usage Instructions
1. Run the main script:
   ```bash
   python main.py
   ```

2. Follow the prompts to either capture images for new students or fill attendance using facial recognition.

3. For manual attendance entry, navigate to the corresponding section in the GUI.

4. Generated CSV files can be found in the `Attendance/` directory.

## How It Works
1. **Image Capture**: Users can enter their enrollment number and name to capture their images using a webcam.
2. **Model Training**: The captured images are used to train a facial recognition model saved as `Trainner.yml`.
3. **Filling Attendance**: When filling attendance, the system captures live video from the webcam, recognizes faces, and logs attendance based on recognized identities.
4. **Data Management**: Attendance records are stored in both CSV files and a MySQL database for future reference.

## Contributing
Contributions are welcome! If you would like to contribute to this project, please fork the repository and submit a pull request with your changes.


