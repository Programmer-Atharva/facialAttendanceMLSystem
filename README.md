# Intelligent Attendance System with Face Recognition

## Project Description
The **Intelligent Attendance System** is an advanced Python application designed to streamline attendance tracking using facial recognition technology. This project uses OpenCV for real-time face detection and recognition, coupled with a user-friendly graphical interface built using Tkinter. The system supports both automated and manual attendance entry, making it versatile for various use cases.

---

## Key Features
- **Facial Recognition**: Identify individuals automatically through face recognition and mark their attendance.
- **Photo Capture**: Capture high-quality face images for training.
- **Hybrid Attendance**: Allows both automatic and manual attendance entry.
- **Data Export**: Generate detailed attendance records in CSV format.
- **Database Support**: Utilize MySQL for robust and secure data storage.

---

## Technology Stack
- **Programming Language**: Python
- **Libraries**: OpenCV, Tkinter, NumPy, Pandas, Pillow
- **Database**: MySQL

---

## Getting Started

### Step 1: Clone the Repository
```bash
git clone https://github.com/Programmer-Atharva/facialAttendanceMLSystem.git
cd facialAttendanceMLSystem
```

### 2. Install Required Packages
Ensure Python is installed on your system (I did my project in conda environment), then install the necessary dependencies:
```bash
pip install -r requirements.txt
```

### 3. Set Up MySQL Database
- Create a MySQL database to store attendance records.
- Update the database connection details in the code as needed.
- You can create another user instead of root user 

### 4. Download Haarcascade
Download the Haarcascade XML file for face detection from the [OpenCV GitHub repository](https://github.com/opencv/opencv) and place it in the project directory.

---

## Usage

### 1. Run app
- Make changes in app.py file to update path of files as per your machine 
- Run `app.py` to open the Tkinter GUI.
- Enter the student's enrollment number and name.

### 2. Take Images
- Click on **"Take Images"** to capture face images.

### 3. Train the Model
- Click on **"Train Images"** to train the face recognition model.

### 4.1 Automatic Attendance
- Select **"Automatic Attendance"** to start the face recognition process using the webcam.

### 4.2 Manual Attendance
- Use the **"Manually Fill Attendance"** option to manually fill attendance records.

### 5. View Registered Students
- Access the admin panel to view the list of registered students and their details.
- The username and password is in app.py file

---

## Directory Structure
```plaintext
facialAttendanceMLSystem/
│
├── TrainingImage/               # Directory to store training images
├── TrainingImageLabel/          # Directory to save trained model
├── StudentDetails/              # Directory to save student details CSV
├── Attendance/                  # Directory to save attendance records
├── haarcascade_frontalface_default.xml  # Haarcascade file for face detection
├── requirements.txt             # Required Python packages
├── main_Run.py                  # Main application file
└── README.md                    # Project documentation
```

---
### Note :  
- my system is linux so some syntax is different than windows like, for windows users it will be for example : 
```python
ubprocess.Popen(r'explorer /select,"C:\Users\path_to_project\facialAttendanceMLSystem\Attendance\-------Check atttendance------"')
```
instead of linux syntax : 
```python
subprocess.Popen(['xdg-open','path-to_project/Attendance/-------Check atttendance-------'])
```

