# Face Recognition + Attendance Project

## Overview

This project is an automated attendance system that leverages face recognition technology to mark and manage attendance. Built entirely in Python, it uses modern computer vision techniques to identify individuals and record their presence efficiently and accurately.

## Features

- **Automated Face Recognition:** Detects and recognizes faces using a webcam or pre-recorded images.
- **Attendance Recording:** Automatically marks attendance for recognized individuals.
- **User-Friendly Interface:** Simple to operate, making it suitable for classrooms, offices, and events.
- **Attendance Logging:** Saves attendance data to a file (CSV or similar) for easy review.
- **Scalability:** Easily add or remove individuals from the system’s database.

## Technologies Used

- Python 3.x
- OpenCV (for image processing)
- face_recognition library (based on dlib)
- NumPy
- Pandas (for data handling)
- Tkinter (if GUI is included; otherwise, remove)
- CSV (for attendance logs)

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/KaranSatish15/Face-Recognition-Attendance-Project.git
   cd Face-Recognition-Attendance-Project
   ```

2. **Install required packages:**
   ```bash
   pip install -r requirements.txt
   ```
   If `requirements.txt` is not available, install manually:
   ```bash
   pip install opencv-python face_recognition numpy pandas
   ```

3. **(Optional) Install dlib prerequisites:**
   - On Ubuntu: `sudo apt-get install build-essential cmake`
   - On Windows: [See the dlib installation guide](https://pypi.org/project/dlib/)

## Usage

1. **Add known faces:**
   - Place images of individuals to be recognized in the `known_faces/` directory (or your designated folder).
   - Rename the images to match the person's name (e.g., `Alice.jpg`, `Bob.jpg`).

2. **Run the attendance script:**
   ```bash
   python attendance.py
   ```
   - The script will start the webcam, detect faces, and mark attendance.
   - Attendance is logged to `attendance.csv` (or configured file).

3. **Review attendance:**
   - Open the CSV log file to view attendance records.

## Sample Directory Structure

```
Face-Recognition-Attendance-Project/
│
├── attendance.py
├── known_faces/
│   ├── Alice.jpg
│   └── Bob.jpg
├── attendance.csv
├── requirements.txt
└── README.md
```

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License.

## Acknowledgements

- [face_recognition](https://github.com/ageitgey/face_recognition) for the core recognition technology.
- [OpenCV](https://opencv.org/) for image processing utilities.

