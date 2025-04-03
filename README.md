# Motion Detection System
Description-

This project implements a real-time motion detection system using OpenCV and Python. It processes video streams from a specified video file (or webcam) to detect significant movement, highlights detected motion with green bounding boxes, saves snapshots, and provides console alerts. The system is suitable for applications like security monitoring or activity tracking.

Features-

- Real-time video processing from a video file.

- Motion detection using frame differencing and contour analysis

- Visual feedback with green bounding boxes around detected motion

- Automatic snapshot saving with timestamps when motion is detected

- Console alerts for motion detection events


Requirements-

- Python 3.7+

- OpenCV ('pip install opencv-python')

- NumPy ('pip install numpy')

- Jupyter Notebook ('pip install notebook')

Installation-

1- Clone the repository- 
git clone https://github.com/Jetfire-dev/motion-detection-system.git

2- Navigate to the project directory-
cd motion-detection-system

3- Install the required dependencies-
pip install -r requirements.txt

## Usage
1. Launch Jupyter Notebook: jupyter notebook
2. Open `motion_detection.ipynb` in your browser.
3. Update the `video_file_path` variable in the notebook to point to your video file (e.g., `"path/to/your/video.mp4"`).
4. Run all cells:
- Green boxes will appear around detected motion in the video feed.
- Snapshots are saved in the project directory with timestamps (e.g., `snapshot_2025-04-03_12-00-00.jpg`).
- Press `q` in the video window to stop execution (you may need to interrupt the kernel if it doesn’t close automatically).

## Notes
- Adjust the `buffer_size`, threshold values, or contour area in the notebook to fine-tune motion sensitivity.
- The current setup uses a video file (`tennis_sample.mp4`). To use a webcam, replace `cv2.VideoCapture(video_file_path)` with `cv2.VideoCapture(0)` in the notebook.
- Running in Jupyter may require interrupting the kernel (via the stop button) to exit the video loop cleanly.

## Resources
- **Video File**: The video used in this project (`tennis_sample.mp4`) was renamed and sourced from Pixabay, a platform for royalty-free media. Original file: [Tennis Match Sample Video](https://pixabay.com/videos/tennis-match-sport-ball-game-50109/).


## License
MIT License

