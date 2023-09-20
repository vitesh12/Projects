# Number Plate Detection using OpenCV and Python
The Haar cascade classifier will be used to detect the licence plate in the picture. A haar cascade classifier is an efficient approach for detecting objects. It is a method based on machine learning.

To train a number plate classifier, the algorithm requires a large number of positive pictures (number plate photos) and negative images (no number plate images). These positive and negative pictures are used to train the classifier. It is then used to other photos to detect objects (number plates). For object detection, we can employ previously learned haar cascades.

## Steps
* Import the required library. In all the following examples, the required Python library is OpenCV. Make sure you have already installed it.

* Read the input image using cv2.imread(). Specify the full image path. Convert the image to grayscale image.

* Initiate the Haarcascade classifier object plate_cascade = cv2.CascadeClassifier() for number plate detection. Pass the full path of the haar cascade xml files. You can use the haar cascade file haarcascade_number_plate.xml to detect the number plate in the image.

* Detect the number plate in the input image using plate_cascade.detectMultiScale(). It returns the coordinates of the detected number plate in (x,y,w,h) format.

* Draw the bounding rectangles around the detected number plate in the original image using cv2.rectangle().

* Display the image with the drawn bounding rectangles around the license number plate.

Let's have a look at some examples for more clear understanding.

![Number Plate Detection using OpenCV and Python](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhjsOn1e-xjnnnrXr4LRl5qiTWEQjsz7tAoZ_8Uz5boJ2R1mkqy-obR_igPWYz389dCktHN-7Pk85ODLAMXl3uC2ilIOz_8koyklvR-aDMCY0FXcQWQYOlHgt7lLvYExhUjL7DENE5-MdQyJTXKzAmSTqip-9ABPurS6fW7kEft-dnbosGjK4srhv-lEpQ/s320/Numberplate_detected.jpg)

On execution, it will produce the following ```output```−
```
Number of detected license plates: 1
```
![Number Plate Detection using OpenCV and Python](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEh6-hm3mDby762Ovd-d-dC-ejrbMbZxFjKQf0BWVjRRwDVXcmURDyhBbJtY9HQo4gD7xVvLlLTYRBqywvg7vCxPkr9ACRZ3PYx5FxPAdw7HSOdaJYu9pKbrj96w2_1HROd7_MEVkNCPW0Yi2W3AL0O3dyT-o-7gtSL4Qhgjl6-r9CFiq1Obs47mrxYnl2g/s320/sample.jpg)
