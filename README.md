# Color Burst and Shape Identification
This is a Python program using the basic concepts of Computer Vision. OpenCV module has been used for the detection of contours and Tkinter was used for UI elements.

# UI
<img src="https://github.com/manohar-iitg/ColorBurst-Shape/assets/96137651/a0ee14e0-ac85-4fe7-b825-0149e7918ad6" height=400 width=450>
<img src="https://github.com/manohar-iitg/ColorBurst-Shape/assets/96137651/f555ae62-a70a-413d-9b27-ea5dc3f1d61c" height=400 width=450>

# UI Features
* The program takes in an input image from within the program itself.
* The Tkinter window opens up with the image and a dropdown menu from which you can choose one of the given 5 colors. When we click on pop color. It pops out all the shapes of the particular color and also finds out the shapes.

# Detecting the color
* We used a HSV tool that can change all three parameters and find out at what particular value of H, S, V are we obtaining the color required. This has been determined prior to the execution of the program.
* When the user chooses a particular color, the pre-determined values are masked over the image and the color detection happens.

# Detecting the shape
* The shape is determined by contour detection. Firstly, the masked image is converted to Canny image which is used for edge detection.
* All the contours in the image are identified and no. of edges are identified approximately.
* It can detect upto side length of 6 (i.e., Triangle, Quadrilateral, Pentagon, Hexagon) and Circle.

# Limitations and Future Ideas
* Anything above approximate edges more than 6 is determined as a circle. Accuracy of contour detection can be improved by setting the parameters of canny. This can be done after studying many results.
* The image is provided from within the program itself. Tkinter can be used for asking the user for input of image from the interface and all the detections done on that image.

# NOTE!
* The modules used here - OpenCV, Pillow are external modules and need to be installed separately)
* pip install opencv-python --user
* pip install Pillow --user
