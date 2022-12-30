# yolov7-object-tracking


### Steps to run Code
- Clone the repository.
```
git clone https://github.com/RizwanMunawar/yolov7-object-tracking.git
```
- Goto the cloned folder.
```
cd yolov7-object-tracking
```
- Create a virtual envirnoment (Recommended, If you dont want to disturb python packages)
```

### For Window Users
python3 -m venv yolov7objtracking
cd yolov7objtracking
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
- Run the code with mentioned command below (by default, pretrained [yolov7](https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7.pt) weights will be automatically downloaded into the working directory if they don't already exist).
```
# for detection and tracking

 python detect_and_track.py --weights yolov7.pt --source test_video.mp4 --classes 0 --view-img --nobbox --show-fps --track --show-track --thickness 3 --unique-track-color

 python detect_and_track.py --weights best.pt --source test_video.mp4 --classes 0 1 2 3 --view-img --nobbox --show-fps --track --show-track --thickness 3 --unique-track-color
