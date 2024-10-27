# YOLOv7 Object Blurring

A Python-based tool for object detection and selective blurring using YOLOv7. This repository allows you to blur specific classes of objects in videos or images. It’s an ideal solution for anonymizing data in videos, protecting privacy, or focusing on certain objects.

### Prerequisites
- **Python 3.6+** installed on your system.
- **pip** upgraded to the latest version.

### Quick Start Guide

#### 1. Clone the Repository
Start by cloning this repository to your local machine:
```bash
git clone https://github.com/RizwanMunawar/yolov7-object-blurring.git
cd yolov7-object-blurring
```

#### 2. Set Up a Virtual Environment (Recommended)
Create a virtual environment to isolate dependencies and prevent conflicts with existing Python packages.

**For Linux Users:**
```bash
python3 -m venv yolov7objblurring
source yolov7objblurring/bin/activate
```

**For Windows Users:**
```bash
python3 -m venv yolov7objblurring
yolov7objblurring\Scripts\activate
```

#### 3. Install Dependencies
Upgrade pip and install the required packages by running:
```bash
pip install --upgrade pip
pip install -r requirements.txt
```

#### 4. Download YOLOv7 Model Weights
Download the [YOLOv7 pretrained weights](https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7.pt) and move them to the `yolov7-object-blurring` folder.

#### 5. Running the Code
Use the following commands to detect and blur objects in your video:

- **Basic Command** (change `source` to the path of your video):
  ```bash
  python detect_and_blur.py --weights yolov7.pt --source "your_video.mp4" --blurratio 20
  ```
  
- **Blurring Specific Classes** (e.g., `person` class):
  ```bash
  python detect_and_blur.py --weights yolov7.pt --source "your_video.mp4" --classes 0 --blurratio 50
  ```

- **Hiding Detection Boxes** (hides the bounding box for blurred areas):
  ```bash
  python detect_and_blur.py --weights yolov7.pt --source "your_video.mp4" --classes 0 --blurratio 50 --hidedetarea
  ```

#### 6. Accessing Results
The output video will be saved in the directory: `runs/detect/exp`. Each new run creates a new `exp` folder with the results.

---

### Example Results
| Objects Blurred A | Objects Blurred B | Hidden Detection Area |
| --- | --- | --- |
| ![Image A](https://user-images.githubusercontent.com/62513924/186101334-1de03f51-9f64-41fd-b488-b77eb949865d.png) | ![Image B](https://user-images.githubusercontent.com/62513924/186101348-3b06d516-5507-4548-8efa-9b55564a75fe.png) | ![Image C](https://user-images.githubusercontent.com/62513924/186102964-59f89ae2-80ac-43c9-ab64-54c607a1cbe9.png) |

### Resources and Further Reading

- **YOLOv7 Project:** [https://github.com/WongKinYiu/yolov7](https://github.com/WongKinYiu/yolov7)
- **OpenCV Documentation:** [https://opencv.org/](https://opencv.org/)

### Articles by the Author
For more insights and tutorials:
- [YOLOv7 Training on Custom Data](https://medium.com/augmented-startups/yolov7-training-on-custom-data-b86d23e6623)
- [Roadmap for Computer Vision Engineers](https://medium.com/augmented-startups/roadmap-for-computer-vision-engineer-45167b94518c)
- [YOLO vs YOLOv5: Which is Better?](https://medium.com/augmented-startups/yolor-or-yolov5-which-one-is-better-2f844d35e1a1)
- [Develop Analytics Dashboards with Streamlit](https://medium.com/augmented-startups/develop-an-analytics-dashboard-using-streamlit-e6282fa5e0f)

---

### Connect with the Author
Follow more updates on [Medium](https://chr043416.medium.com/) or connect on [LinkedIn](https://www.linkedin.com/in/muhammadrizwanmunawar/).
