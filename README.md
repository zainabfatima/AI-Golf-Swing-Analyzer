# AI-Golf-Swing-Analyzer
This project uses Google’s Mediapipe to estimate human body keypoints from golf swing videos and calculates angles of movement for performance analysis. It processes video frames, extracts landmarks, computes angles, and stores results for further review.

📁 File Structure & Purpose
app.py
Main entry point — coordinates video reading, pose detection, angle calculations, and result storage.

calculate_and_append_angle.py
Computes angles between joints (e.g., elbow, shoulder) from Mediapipe keypoints and appends results to a dataset.

calculate_and_print_average_angle.py
Calculates the average of angles over the video duration and prints it for analysis.

compute.py
Contains core mathematical calculations for pose angle detection.

create_dataframe.py
Converts computed results into a structured DataFrame for CSV export.

get_video_length.py
Retrieves video duration, possibly to synchronize processing.

save_images.py
Saves annotated frames (pose landmarks drawn) for visual review.

show_angle.py
Displays the calculated angles on the video frame in real-time.

writeDataframe.py
Saves DataFrame data (angles, timestamps) to CSV or Excel.

requirements.txt
Python dependencies (Mediapipe, OpenCV, Pandas, NumPy, etc.).

__pycache__/
Compiled Python bytecode files (not manually edited).

🚀 Features
Detects golfer’s pose in each video frame using Mediapipe.

Calculates specific body joint angles for performance metrics.

Displays and saves annotated video frames with angles.

Stores computed angles in CSV format for deeper analysis.

▶️ How It Works
Video Input – Load a golf swing video into app.py.

Pose Estimation – Mediapipe detects 33 body landmarks per frame.

Angle Computation – Calculate joint angles (e.g., arm bend) using trigonometry.

Data Storage – Save results as CSV and annotated images.

Analysis – View average angles or visual swing metrics.

📤 Input
A golf swing video file (.mp4, .avi).

📈 Output
Annotated images/video with joint angles.

CSV file containing per-frame angle measurements.

Average angle statistics printed in console.
