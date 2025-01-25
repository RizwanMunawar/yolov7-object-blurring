# YOLOv7 Object Blurring

A Python project for object detection and selective blurring using YOLOv7. This repository allows you to blur specific classes of objects in videos or images. It’s an ideal solution for anonymizing data in videos, protecting privacy, or focusing on certain objects.

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

**Some of my articles/research papers | computer vision awesome resources for learning | How do I appear to the world? 🚀**

[Ultralytics YOLO11: Object Detection and Instance Segmentation🤯](https://muhammadrizwanmunawar.medium.com/ultralytics-yolo11-object-detection-and-instance-segmentation-88ef0239a811) ![Published Date](https://img.shields.io/badge/published_Date-2024--10--27-brightgreen)

[Parking Management using Ultralytics YOLO11](https://muhammadrizwanmunawar.medium.com/parking-management-using-ultralytics-yolo11-fba4c6bc62bc) ![Published Date](https://img.shields.io/badge/published_Date-2024--11--10-brightgreen)

[My 🖐️Computer Vision Hobby Projects that Yielded Earnings](https://muhammadrizwanmunawar.medium.com/my-️computer-vision-hobby-projects-that-yielded-earnings-7923c9b9eead) ![Published Date](https://img.shields.io/badge/published_Date-2023--09--10-brightgreen)

[Best Resources to Learn Computer Vision](https://muhammadrizwanmunawar.medium.com/best-resources-to-learn-computer-vision-311352ed0833) ![Published Date](https://img.shields.io/badge/published_Date-2023--06--30-brightgreen)

[Roadmap for Computer Vision Engineer](https://medium.com/augmented-startups/roadmap-for-computer-vision-engineer-45167b94518c)  ![Published Date](https://img.shields.io/badge/published_Date-2022--08--07-brightgreen)

[How did I spend 2022 in the Computer Vision Field](https://www.linkedin.com/pulse/how-did-i-spend-2022-computer-vision-field-muhammad-rizwan-munawar) ![Published Date](https://img.shields.io/badge/published_Date-2022--12--20-brightgreen)

[Domain Feature Mapping with YOLOv7 for Automated Edge-Based Pallet Racking Inspections](https://www.mdpi.com/1424-8220/22/18/6927) ![Published Date](https://img.shields.io/badge/published_Date-2022--09--13-brightgreen)

[Exudate Regeneration for Automated Exudate Detection in Retinal Fundus Images](https://ieeexplore.ieee.org/document/9885192) ![Published Date](https://img.shields.io/badge/published_Date-2022--09--12-brightgreen)

[Feature Mapping for Rice Leaf Defect Detection Based on a Custom Convolutional Architecture](https://www.mdpi.com/2304-8158/11/23/3914) ![Published Date](https://img.shields.io/badge/published_Date-2022--12--04-brightgreen)

[Yolov5, Yolo-x, Yolo-r, Yolov7 Performance Comparison: A Survey](https://aircconline.com/csit/papers/vol12/csit121602.pdf)  ![Published Date](https://img.shields.io/badge/published_Date-2022--09--24-brightgreen)

[Explainable AI in Drug Sensitivity Prediction on Cancer Cell Lines](https://ieeexplore.ieee.org/document/9922931)  ![Published Date](https://img.shields.io/badge/published_Date-2022--09--23-brightgreen)

[Train YOLOv8 on Custom Data](https://medium.com/augmented-startups/train-yolov8-on-custom-data-6d28cd348262)  ![Published Date](https://img.shields.io/badge/published_Date-2022--09--23-brightgreen)


**More Information**

For more details, you can reach out to me on [Medium](https://muhammadrizwanmunawar.medium.com/) or can connect with me on [LinkedIn](https://www.linkedin.com/in/muhammadrizwanmunawar/)
