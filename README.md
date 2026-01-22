# 🎓 Face Recognition Attendance System

A modern web-based **Face Recognition Attendance System** using **Flask, OpenCV, and face_recognition**, built for both Admins and Students. This system allows automatic student attendance using facial recognition with full dashboard functionality.


## 📸 Project Overview

This system uses a webcam to capture and recognize student faces and log attendance. Admins can register students, manage credentials, and generate attendance reports. Students can view their personal attendance data with calendar visualization, stats, and download options.


## 🔑 Features

### 🧑‍🎓 Student Registration Module

- Admin registers students with Full Name, Register Number & Room

- Facial data captured via webcam

- Encodings stored using face_recognition library

### 📸 Real-Time Face Recognition Attendance

- Auto camera activation

- Recognizes faces using deep learning encodings

- Marks attendance without duplicates

- Stores records in attendance.csv

### 🖥️ Admin Dashboard

- Register new students

- Capture & store face data

- Create student login credentials

- View, filter & export attendance

- Delete students

- Beautiful cards & modern UI

### 🎓 Student Dashboard

- Personalized dashboard

- Total present/absent stats

- Attendance percentage

- Calendar view

- PDF report download

- Month filter

- Alerts for <75% attendance

### 📂 CSV-Based Data System

- Lightweight & portable

- No database setup required

- Easy to debug

- Good for small-to-medium projects

## 🧰 Technologies Used

| Component            | Technology       |
|---------------------|------------------|
| Backend             | Flask (Python)   |
| Face Detection      | OpenCV, face_recognition |
| Frontend UI         | HTML, CSS, JavaScript |
| Data Storage        | CSV files        |
| PDF Export          | jsPDF            |

## 🚀 Installation & Setup

### 1️. Clone the Repo

    git clone <repository-url>
    cd face-attendance-system
### 2. Install Requirements

    pip install -r requirements.txt
### 3. Install Face Recognition Dependencies
    
    pip install face_recognition
    pip install opencv-python
### 4. Run Flask App
    python app.py
## 📸 How Attendance Works

- Camera opens → captures real-time video

- Face detected → converted to encoding

- Compared with known encodings

- If matched → attendance marked

- Attendance saved in:

        attendance.csv
  Format:

      register_number,name,Time
      99220042009,Vamsi Araveti,2025-07-03 17:54:15
 ## 🧠 System Architecture
 
     project/
    │── app.py                  # Flask backend
    │── register.py             # Face registration
    │── face_attendance.py      # Real-time attendance
    │── encodings.pkl           # Face encodings
    │── users.csv               # Login credentials
    │── students.csv            # Student details
    │── attendance.csv          # Attendance log
    │── templates/
    │   ├── admin_dashboard.html
    │   ├── student_dashboard.html
    │   ├── create_credentials.html
    │   ├── add_student.html
    │   ├── profile pages...
    │── static/
        ├── dashboard.css
        ├── admin.css
        ├── student.css
    
## requirements.tx

    Flask==3.0.2
    Werkzeug==3.0.1
    Jinja2==3.1.3
    
    opencv-python==4.9.0.80
    face_recognition==1.3.0
    cmake==3.29.2
    
    numpy==1.26.4
    click==8.1.7
    itsdangerous==2.1.2
    MarkupSafe==2.1.5
    
    pandas==2.2.1
    python-dateutil==2.8.2
    
    Pillow==10.2.0
    dlib==19.24.2
## 🔥 Notes (Important)

### face_recognition requires dlib
 - Both are included above.
 - If your PC is slow, use:
   
         pip install face_recognition --no-cache-dir
### CMake is required to build dlib
- Already included.
- If error occurs:

      pip install cmake
### Make sure you install Visual Studio Build Tools on Windows
- Needed for dlib.
### For webcam support: opencv-python
- Already added.

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.


Version: 2.0.0

Last Updated: July 2025 

Python: 3.8+ 

Dependencies: See requirements.txt


For questions, suggestions, or issues, please contact. 
