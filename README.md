# Photo-into-Pencil-Sketch
In this project, I have converted a photo into pencil sketch using python. 

#### Step 1:
Find the image to be used and read it using cv2.imread().
#### Step 2:
Read the image in RGB(Red, Green, Blue). Then convert it into gray scale image. This makes our img black and white photo.
#### Step 3:
We will now invert gray scale image which we will call as invert. Inversion helps to enhance details. The Logical NOT or invert is an operator which takes a binary or gray level image as input and produces its photographic negative, i.e. dark areas in the input image become light and light areas become dark. 
*Invert Formula*
Q(i,j)=255-P(i,j)
#### Step 4:
We will now blur the img using Gaussian Blur called as Gaussian Smoothing. It is used in graphics to reduce image noise and reduce details.
#### Step 5:
Then invert the blurred img which we will call as invert_blur.
#### Step 6:
Now we are going to create the pencil sketch image by blending the “gray scale image” with the “inverted blurred image”. This can be done by dividing the “gray scale image” by the “inverted blurred image”. Since images are just arrays we can easily do this in programming by using the divide function from the cv2 library.
