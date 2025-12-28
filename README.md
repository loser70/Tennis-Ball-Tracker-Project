Tennis-Tracker
A computer vision application for tennis ball tracking and speed analysis.

Overview
This project uses computer vision and machine learning techniques to:

Detect and track tennis balls in video footage
Identify tennis court lines and transform the perspective
Calculate and display the ball speed
Generate output videos with tracking visualization
Features
Tennis ball detection using YOLO
Court line detection using a custom ResNet50-based model
Perspective transformation for top-down court view
Real-time ball speed calculation
Side-by-side video output showing tracking results
Project Structure
Tennis-Tracker/
│
├── main.py                             # Main execution script
├── step_by_step_implementation.ipynb   # Jupyter notebook with implementation details
├── court_line_detector.py              # Court detection functionality
├── utils.py                            # Utility functions
├── tennis_court.jpg                    # Reference court image for visualization
│
├── models/                             # Pre-trained models
│   ├── keypoints_model.pth             # Model for court line detection
│   └── best.pt                         # YOLO model for ball tracking
│
└── input_videos/                       # Directory for input videos
    └── input_video_1.mp4               # Example input video
Requirements
Python
PyTorch
OpenCV
Ultralytics YOLO
NumPy
Matplotlib
Installation
Clone the repository:

git clone https://github.com/taufiktrf/Tennis-Tracker.git
cd Tennis-Tracker
Install the required packages:

pip install torch torchvision opencv-python ultralytics numpy matplotlib
Usage
Place your input tennis videos in the input_videos/ folder
Run the main script changing video_name variable:
python main.py
The output video will be saved in the project directory
