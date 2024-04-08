# yolov7-object-blurring

### Steps to run Code
- Clone the repository.
```
git clone https://github.com/RizwanMunawar/yolov7-object-blurring.git
```
- Goto the cloned folder.
```
cd yolov7-object-blurring
```
- Create a virtual envirnoment (Recommended, If you dont want to disturb python packages)
```
### For Linux Users
python3 -m venv yolov7objblurring
source yolov7objblurring/bin/activate

### For Window Users
python3 -m venv yolov7objblurring
cd yolov7objblurring
cd Scripts
activate
cd ..
cd ..
```
- Upgrade pip with mentioned command below.
```
pip install --upgrade pip
```
- Install requirements with mentioned command below.
```
pip install -r requirements.txt
```
- Download [yolov7](https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7.pt) object detection weights from link and move them to the working directory {yolov7-object-blurring}
- Run the code with mentioned command below.
```
#if you want to change source file
python detect_and_blur.py --weights yolov7.pt --source "your video.mp4" --blurratio 20

#for specific class (person or 0 classes)
python detect_and_blur.py --weights yolov7.pt --source "your video.mp4" -classes 0 --blurratio 50

#hide-detected-bounding-boxes
python detect_and_blur.py --weights yolov7.pt --source "your video.mp4" -classes 0 --blurratio 50 --hidedetarea
```
- Output file will be created in the <b>working-dir/runs/detect/exp</b> with original filename.

### Results
<table>
  <tr>
    <td>Objects Blurred A</td>
    <td>Objects Blurred B</td>
    <td>Objects Blurred Hide detected area</td>
  </tr>
  <tr>
    <td><img src="https://user-images.githubusercontent.com/62513924/186101334-1de03f51-9f64-41fd-b488-b77eb949865d.png"></td>
    <td><img src="https://user-images.githubusercontent.com/62513924/186101348-3b06d516-5507-4548-8efa-9b55564a75fe.png"></td>
    <td><img src="https://user-images.githubusercontent.com/62513924/186102964-59f89ae2-80ac-43c9-ab64-54c607a1cbe9.png"></td>
  </tr>
 </table>


 ### References
 - https://github.com/WongKinYiu/yolov7
 - https://opencv.org/
 
### My Medium Articles
- https://medium.com/augmented-startups/yolov7-training-on-custom-data-b86d23e6623
- https://medium.com/augmented-startups/roadmap-for-computer-vision-engineer-45167b94518c
- https://medium.com/augmented-startups/yolor-or-yolov5-which-one-is-better-2f844d35e1a1
- https://medium.com/augmented-startups/train-yolor-on-custom-data-f129391bd3d6
- https://medium.com/augmented-startups/develop-an-analytics-dashboard-using-streamlit-e6282fa5e0f
- https://chr043416.medium.com/setup-transfer-learning-toolkit-with-docker-on-ubuntu-a9b0198bae7
- https://medium.com/nerd-for-tech/object-detection-and-image-classification-helps-in-retail-analytics-46acc434daa0

For more details, you can reach out to me on [Medium](https://chr043416.medium.com/) or can connect with me on [LinkedIn](https://www.linkedin.com/in/muhammadrizwanmunawar/)
