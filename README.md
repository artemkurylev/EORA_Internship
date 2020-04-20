# EORA_Internship

## To run blind detection with code from git you need to have:
python
scipy
numpy
opencv
dlib
shape_predictor_68_face_landmarks.dat or another pretrained model which is comaptible with dlib for face landmarks detection 
## Use following command 
```python blink_detect.py -v output.avi --shape-predictor shape_predictor_68_face_landmarks.dat``` if you want to use videofile(output.avi) as an input

```python blink_detect.py --shape-predictor shape_predictor_68_face_landmarks.dat``` if you want to use camera
## You can also use docker image 
```docker pull artikot/blind_detection```
For this type only one option with camera is availible

Use following command:

```docker run -v /tmp/.X11-unix:/tmp/.X11-unix -e DISPLAY=unix$DISPLAY --device /dev/video0 artikot/blind_detection```
