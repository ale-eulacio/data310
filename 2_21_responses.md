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
