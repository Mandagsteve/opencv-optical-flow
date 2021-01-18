# opencv-optical-flow

Installation
Before you start the demo of Optical Flow calculation, you need to create a virtual environment in your working directory and install the required libraries:

virtualenv -p python3.7 venv
source venv/bin/activate
pip install -r reqirements.txt
Sparse Optical Flow
There is a demo lucas_kanade.py script of Lucas-Kanade algorithm which can be run with this command:

python3 demo.py --algorithm lucaskanade --video_path videos/car.mp4
Dense Optical Flow
The wrapper of Dense Optical Flow algorithms dense_optical_flow.py can run a couple of OpenCV's algorithm implementations:

To start the Dense Lucas-Kanade algorithm:
python3 demo.py --algorithm lucaskanade_dense --video_path videos/people.mp4
To start the Farneback algorithm:
python3 demo.py --algorithm farneback --video_path videos/people.mp4
To start the RLOF algorithm:
python3 demo.py --algorithm rlof --video_path videos/people.mp4
