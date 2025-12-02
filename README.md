# face recognition attendance system (python + opencv)

a real-time face recognition attendance system built with python that detects faces through a webcam, matches them against known images, and automatically logs attendance into a csv file with timestamps.

## why?

this project demonstrates real-world use of computer vision, facial recognition, image processing, and automation using python and opencv.

---

## features

- real-time webcam face detection  
- face recognition using trained encodings  
- automatic attendance tracking  
- csv file logging with time stamps  
- image dataset integration for known faces  
- fast matching using numpy  
- works on macOS (apple silicon supported)  

---

## functionality

1. images of known individuals are stored in the `ImageAttendance/` folder  
2. the program encodes each face using the `face_recognition` library  
3. a webcam feed is captured using opencv  
4. detected faces are compared against known encodings  
5. when a match is found:  
   - the person’s name is displayed on screen  
   - their attendance is recorded into `Attendance.csv`  
   - time is automatically logged  

---

## tech stack

- python 3.10+  
- opencv (`cv2`)  
- numpy  
- face-recognition  
- dlib  
- csv file handling  

---

## project structure

AttendanceProjecto/
│
├── AttendanceProject.py
├── Basics.py
├── Attendance.csv
├── ImageAttendance/
│   ├── elon musk.jpg
│   ├── bill gates.jpg
│   └── Jack Ma.jpg
└── ImageBasic/

---

## installation

install required dependencies:

pip install opencv-python face-recognition numpy

note: face-recognition depends on dlib which may take several minutes to build on macOS.

---

## how to run

python AttendanceProject.py

---

## output example

the program automatically updates `Attendance.csv` like this:

Name,Time  
Elon Musk,14:32:10  
Bill Gates,14:33:01  

---

## known setup notes

- webcam access is required  
- macOS users may be prompted for camera permission  
- first run may take longer due to face encoding  









