# Parking Space Counter using Python, OpenCV and Pickle
<img src="img/parkingcv_final.png" width="1000"> 

## Video Used

Tom Berrigan https://www.youtube.com/watch?v=yojapmOkIfg&list=LL&index=10

* Download this video in 1080p
* Rename it to parkinglot_timeplapse.mp4 
* Place it in project folder

## Packages
```sh
pip install cv2
pip install pickle
```

## Get started
```sh
run spot_picker.py
```
* Mark parking spaces with left click, delete with right click. 
* Output: spot_pos.pkl (stores (x,y) of each space)

```sh
run section_picker.py
```
* Mark parking sections with left click, delete with right click. 
* Only needs upper left and lower right section corners
* Output: section_pos.pkl (stores (x,y) of corner points selected)

```sh
run main.py
```
* Live update of total free spaces and free spaces in each parking section 

## Code inspired by:

Murtaza's Workshop - Robotics and AI https://www.youtube.com/watch?v=caKnQlCMIYI

## Reflection
* Parking spots picked by hand. Accurancy could be improved by careful selection or automating selection process.
* Useful to have of pixel threshold and img processing parameter intuition.
* Wind moving camera and white marks on parking space could represent potential problems.
* Simple computer vision techniques could solve real-world problems (no ML required)
