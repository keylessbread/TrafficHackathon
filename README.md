Within this repository I have included 5 files. Two of the files are the output of scripting a live video stream taken from ny.511.com which
shows videos from roadways in New York State. By using the exit with a blind turn, I thought I could represent the blind curves that are
sometimes evident during long backroads that bikers, runners and other pedestrians use for exercise. These files are called
1. traffic_1hour_dataset.xls : which was recorded from 8PM - 9PM on a Wednesday
2. traffic_1hour_dataset.xls : which was recorded from 9AM - 10AM on a Thursday

The Dockerfile and requirements detail the other applications that I used in order to launch an interactive website that allows users to
input times of the day to monitor traffic activity at certain locations along the Northway. The proprietary code that utilizes all of these
different applications and hosts is kept from the open repository because of the use of passwords and other backend identifiers.

The TrafficSYSscript.ipynb can be run in a Jupityer notebook in order to create a program that visualizes the tracking of cars on the road
in real time. It utilizes YOLO and OpenCV to stream videos from ny.511.com and superimpose labels on the cars that indicate their activity.
That is, whether the car is approaching a pedestrian, moving away, idle, or, passing or clear of the pedestrian location. The numbers attached
to these lables are the countdown timers that detail the approach or departure of the cars to the pedestrian location in milliseconds.
