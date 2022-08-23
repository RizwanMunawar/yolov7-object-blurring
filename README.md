# yolov7-object-cropping

### Steps to run Code
- Clone the repository.
```
git clone https://github.com/RizwanMunawar/yolov7-object-cropping.git
```
- Goto the cloned folder.
```
cd yolov7-object-cropping
```
- Create a virtual envirnoment (Recommended, If you dont want to disturb python packages)
```
### For Linux Users
python3 -m venv yolov7objcropping
source yolov7objcropping/bin/activate

### For Window Users
python3 -m venv yolov7objcropping
cd yolov7objcropping
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
- Download [yolov7](https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7.pt) object detection weights from link and move them to the working directory {yolov7-object-cropping}
- Run the code with mentioned command below.
```
#if you want to change source file
python detect_and_blur.py --weights yolov7.pt --source "your video.mp4"

#for specific class (person)
python detect_and_blur.py --weights yolov7.pt --source "your video.mp4" -classes 0
```
- Cropped Objects will be stored in "working-dir/crop" folder.

### Results
<table>
  <tr>
    <td>Objects Cropped 1</td>
    <td>Objects Cropped 2</td>
    <td>Objects Cropped 3</td>
    <td>Objects Cropped 4</td>
    <td>Objects Cropped 5</td>
    <td>Objects Cropped 6</td>
    <td>Objects Cropped 7</td>
  </tr>
  <tr>
    <td><img src="https://user-images.githubusercontent.com/62513924/185807618-0d82e0ff-12f9-48b0-9c92-68f336acf621.jpg"></td>
     <td><img src="https://user-images.githubusercontent.com/62513924/185807623-ee024f23-a2ae-4560-b570-9d09ea773696.jpg"></td>
     <td><img src="https://user-images.githubusercontent.com/62513924/185807620-a3990460-2f88-45c3-9f17-0bd917574370.jpg"></td>
     <td><img src="https://user-images.githubusercontent.com/62513924/185807621-d53e3830-fe0c-43ca-af60-a285b2112cf8.jpg"></td>
     <td><img src="https://user-images.githubusercontent.com/62513924/185807624-0827eb80-2bf1-436d-ac38-c2cb864be9a2.jpg"></td>
     <td><img src="https://user-images.githubusercontent.com/62513924/185807625-18ddabec-90eb-40cc-8370-9ec603c2c14f.jpg"></td>
     <td><img src="https://user-images.githubusercontent.com/62513924/185807626-1f9299a5-9487-4c4a-ac21-76a43a8f146f.jpg"></td>
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

For more details, you can reach out to me on [Medium](https://chr043416.medium.com/) or can connect with me on [LinkedIn](https://www.linkedin.com/in/muhammadrizwanmunawar/)
