# Number-VS-Image
To understand what a RGB/RGBA channel is, we have to dip drive into the image infrastructure first which is actually digital composition.
Over here, we try to make a sort of sense of understanding how differentiation of number/digit with respective to the channel makes different colors and transparency.

An image may consist of single or several (RGB & RGBA) Bands/ channels. Very first time, let we see single band/ channels how looks like and how composed of.

In this article, we try to get some hand on experience. To do so, we need to read CSV file and have to call some library as well.

What we see, a 28x16 matrix having value 0 or 225.  One more insight, out of the matrix values 225 number/ digit having a shape of ONE.  
With our naked eyes, We may consider it as an IMAGE of ONE SIZED Height 28 & Weight 16. 

Let's get started, now it's time to play with numbers. For convenience, we covert this matrix as a (28x16) numpy array. 
Looks sounds good, right.
What if we consider it as an IMAGE representing with the values (0 ,225) and two colored image Black & White. Black & White Image basically a gray scale image. Zero represent Black and 225 represent White. What about other values between 0 – 225. We will discuss it later on. Now we will see, 28x16 matrix having value 0 or 225 in a image form how it looks like.


In “ONE” Image, pixel coordinate system with (0,0) center at top left corner. 0 to 255, There are 256 values represent a range of color where’s zero for Black and 225 for White. What about (0,0) and (8,2) coordinate on that image and what’s the pixel values and how it looks like.   

Since above showed Fig-ONE is a single Band/ Channel/ Gray Scale Image, one dimensional pixel value. Later on, we work with RGB or RGBA (3 Channel or 4 Channel).  Now we see the digital presentation of (0-255) 256 values in an image. 


.



    
For convenient operation:
CSV dataframe converted into a numpy array and data type uint8 which is 8bit range from 0 to 255

Range of color Black to white (0 -- 225)

Range of color Black to white (0 -- 225). Lets see the Plot of blackwhite_array

To form an RGB image from three array of number. We create three numpy array for R , G, B channel.
Very first time, we create a 28X16 numpy array having value 0 and 128 which is belong to 0-255. To access a numpy array, 3rd row and 8th column, we have to index number staring from 0.  With our naked eyes, we can see its 2X7 having 128 value. First row and first column that is 0X0 having value 0. 

An image from that array, how it looks like.  If we access to pixel, 3rd row and 8th column, we have to use Cartesian coordinate system having top left corner as (0,0). With our naked eyes, we can see its 7X2 having 128 value. First row and first column that is 0X0 having value 0. 


arrayPixelVale53 for RED , arrayPixelVale204 for GREEN and arrayPixelVale59 for BLUE.
arrayPixelVale53 contained values 0 and 53
arrayPixelVale204 contained values 0 and 204
arrayPixelVale59 contained values 0 and 59
The bled of this color value will be seen https://www.w3schools.com/colors/colors_rgb.asp
Same color as we see at https://www.w3schools.com/colors/colors_rgb.asp
Now we try to marge another channel alpha channel responsible for transparency of color. For that we will choose 127 which mid value of 0 to 255.  If 0 for black and 255 for white then we may imagine 127 for  dim color


four channel RBG and Alpha. We can check it from https://rgbacolorpicker.com/

So far as I discussed, How  number of array construct a single band/ channel image gray image. Merging three channel / band image constructing a RBG colorful Image. How numbers blending forms a colorful image. Finally, to control a transparency of a colorful image adding new aloha channel/ band. 

https://www.w3schools.com/python/

https://pillow.readthedocs.io/en/latest/reference/Image.html

https://numpy.org/doc/

https://rgbacolorpicker.com/

https://www.geeksforgeeks.org/

   

