Original image: 
![og_imgfr](og_imgfr.png)

I found this cool image on the architecture section of unsplash. I wanted to see what the vertical and horizontal line filters could do with it since it has so many lines that are going in a circle. I modififed the horizontal and vertical line filters slightly, just adding bigger numbers to see what that would do.

Filter 1 = [ [-2, -3, -2], [0, 0, 0], [2, 3, 2]]

The result was about the same as the original vertical line filter. The only difference is that the whites were accented more with the filter with slightly bigger numbers

Filter 1 image:
![vert_img](vert_img.png)

Filter 2 I did the same, using larger numbers instead of the original, but keeping the design of the filter the same

Filter 2 = [ [-2, 0, 2], [-3, 0, 3], [-2, 0, 2]]

Filter 2 image: ![horiz_img](horiz_img.png)


For filter 3 I tried to see if I could get a diagonal line filter in some way. I did this by creating a diagonal line of zeroes in the 3X3 array. It seemed to work

Filter 3 = [[0,-1,1],[-1,0,1],[-1,1,0]]

Filter 3 image: ![diag_img](diag_img.png)

The convolution is going through each pixel in the image (for x/y in range(size_x/y-1). In the actual loop, it is going through a 3X3 array one at time, applying the filter that is a 3x3 array from one corner to the other, 9 times to get every pixel. This ends up emphasizing the lines that are emphasized by the filter. For the vertical, the zeroes end up being in the middle column of the 3x3 array that is the filter. Therefore, in the final image, that middle line is not seen as much, and the vertical lines are emphasized much more. This is super useful for computer vision because it allows for the features of an image to pop out way more. This means that the patterns are much easier to recognize for the computer, making it much easier to recognize objects

Pooling:
I pooled the vertical line image:
![vert_pooled](vert_pooled.png)

The pooling loop completes its task by selecting every other pixel in x and why with "for x/y in range(0, size_x,/y 2)". Then the filter appends the 2X2 array of the sorrounding pixels of the one selected in the for loop statement. After they are all appended, the "pixels.sort(reverse=True)" line selects the largest pixel value, and this one repleces tall the other pixels. This halves the size of the image, and gives a lot more weight to all the most important velues from every 2x2 array that is passed into the loop. 
