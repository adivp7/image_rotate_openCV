# image_rotate_openCV
This project is a simple C++ program to rotate an image through an angle using OpenCV v4.1.1.

To run this project:
> Compile rotate.cpp using OpenCV v4.1.1 libraries and MinGW-W64 compiler (v8.1.0 x86_64-posix-seh-rev0 used).
  Or run rotate.exe. The supplied dll's are sufficient to run the program.
> Enter image path (copy image to folder for convenience).
> Enter clockwise rotation angle in degrees.
> The original image and rotated image will be displayed in new windows.
> Click on the windows and press any key to close windows.

Rotations of multiples of 90 degrees are relatively straightforward and easily achieved using the rotate() function.

For other angles, a rotation matrix is created using the getRotationMatrix2D() function and the necessary scale so as to not cut off edges of the image. Then the warpAffine() function is used to apply said rotation matrix to the image.

- Aditya Painuly, B. Tech (CSE), GEHU
