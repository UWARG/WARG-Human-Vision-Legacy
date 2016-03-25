# WARG-Human-Vision
WARG-Human-Vision recieves photos with attached metadata corresponding to GPS coordinates, altitude and heading of the aircraft when the image was taken. Using this data along with data from the camera specifications (GoPro Hero 3+) areas, centroids and GPS Locations can be computed by selecting points on the image. The GUI computes the data with out the need for complex computer vision algorithms to determine if a target exists in the image.  

#Installation

#Running the GUI

#Buttons
Load: Loads the first picture in the file "Images_2_Process" folder

Select Verticies: Double click on the image where a corner of the target exists to leave a point. The number of points can must be from 3-8

Probe Drop Location: Double clicking on the image where a probe drop exists to compute the GPS Coordinates of the selected point

Point Target: Double click on the image at a point of interest and the GPS Coordinates of the point are computed. Up to 3 point targets can be selected

QR Code: Double click on the top left of the QR Code and double click on the bottom right of the QR Code to be scanned. The image is cropped to fit between the points and is scanned for QR Code data

Clear: Clears all points on the screen

Compute: Calculates the area in m^2 contained by the Select Verticies points and the GPS Coordinates of the centroid of the area. Displays all computed data to the user

Process: Writes computed data to log file in "DataLogs" folder and moves image to the "Processed_Images" folder. Once this is clicked no other computations can be done on the image

No Target: If no targets, probe drops or areas of interest are in the image clicking will move the image to the "Deleted" folder. Once this is clicked no other computations can be done on the image

