# 17CS0043 A Compact Implemenation of Video to Manga Framework
Author: HU Jiamian, 54018371

This project is aming for transforming video to comics/manga. Two stages are required to complete the process.
Two stages are required to complete all process.

## Stage 1: Data preparing
1. Make sure video file under folder Testing_videos/, then do the frame splitting:
```
python Read_Video.py
```
After running the program, input video file name:
```
Please input the video file name: yourVideoName.mp4
```
2. Make sure subtitle file under Scripts folder and do read text:
```
python Read_script.py
please input subtitle file name: subtitle.srt
```
3. If 1 is successfully completed, do face detection:
```
python FaceDetection.py
Please input your direction folder name: yourTestingdirectory
```
4. Run comic grids to detect scene. May takes some time.
```
python Comic_grids.py
Please specify usage of this function: 1. Scene detection 2. generate comic"
1
```
If fales report occurs, please implement this process in Python IDE such pyCharm.
## Stage 2: Generate Comic
Run comic_grids.py to generate comic:
```
python Comic_grids.py
```
Input parameters to select usage of this function. In this stage, it is make comic.
```
Please specify usage of this function: 1. Scene detection 2. generate comic"
2
```
Input styles provided. 0 for la muse, 1 for rain princess, 2 for scream, 3 for undine, 5 for wave, 6 for werck.
```
First, input the comic style: your selected style
```
Wait for some time, the comic is ready in Comic folder.
