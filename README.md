 Face Recognition Attendance System
This Google Colab notebook implements a simple face recognition-based attendance system. It uses the face-recognition library along with opencv-python for image processing.

Features:
Install Libraries: Installs necessary Python packages (face-recognition, opencv-python).
Setup Known Faces and Attendance Logic: Defines directories for known faces and captured faces, and a function mark_attendance to record attendance in attendance.csv.
Encode Known Faces: A load_known_faces() function is provided to load images from the known_faces directory, encode them, and store their names. You need to upload images of known individuals to the known_faces folder and then uncomment and run load_known_faces().
Recognition and Attendance Loop: The process_attendance_frame(frame) function takes an image frame, detects faces, compares them against known encodings, marks attendance for recognized individuals, and saves captured face images.
Store Captured Faces: Defines a directory and function save_captured_face to store images of detected faces for review.
Test with Webcam (Colab Specific): Provides a utility to capture a photo using your webcam within the Colab environment and then processes it for attendance.
View Attendance Log: A view_attendance() function to display the attendance.csv file, showing who was marked present and at what time.
How to Use:
Run all cells sequentially.
Upload images of individuals you want to recognize into the known_faces folder. Each image filename (e.g., John_Doe.jpg) will be used as the person's name.
Uncomment and run the load_known_faces() call in the "Encode Known Faces" section.
Run the Webcam Test cell to capture your photo and check for recognition.
View the Attendance Log to see if your attendance was recorded.
Note: If you encounter a Webcam Error, ensure your browser has camera permissions enabled for Google Colab.
