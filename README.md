# Pixel & Play Arduino Application 

This is a part of a university project consisting of a [Neopixel Arduino Game Console](https://www.instructables.com/Arduino-Neopixel-Console/). In particular, here you will find a useful application developed in processing to draw your own images and display them on the RGB LED Matrix with the help of an Arduino library developed by [Ramón Heras](https://github.com/ramonheras). The hardware can be downloaded [here](https://github.com/ramonheras/Pixel-and-Play-Open-Hardware/tree/master/PCB/gerber_files), it has been designed by [Salvador Ruiz](https://github.com/SalRuiSed). The [.stl files](https://github.com/ramonheras/Pixel-and-Play-Open-Hardware/tree/master/3D%20design/STL) of the case designed by [Ramón Heras](https://github.com/ramonheras).

The "MatrixPaint" has been developed on proccessing, you can use it to make paint Matrix Images easier and abstract the user from having to calculate the pixels that must be lighted up to display the image. We used it, for example, for painting the maps of the example games.

# Instructions for use

To run this programme, we first exported it as an *.exe* file for Windows but it did not work properly, so I strongly recommend downloading [processing](https://processing.org/download) and running it from there.

The interface has a canvas, emulating the Neopixel matrix (for changing the canvas matrix size modify the constants "*columns*" (**width**) and "*rows*" (**height**) in the main file).

There is a colour palette in the upper right corner, which can be modified if you wish to enter a specific colour. To change a colour field, look for the "*Palettes*" class, in "*Palettes.pde*", and enter the RGB combination of the desired colour in the same position of each matrix in its corresponding primary colour. 

If you've made a mistake painting a pixel and want to erase it, just paint it black. After pressing the "*Generate Code*" button you have to type a name for the drawing then, press enter.

In the same program directory, it will automatically create a file with the chosen name and with the extension "*.ino*". This file will contain an array of the selected screen size, with each of the pixels that must be turned on to form the created image. To display the image call the API "*Panel.h*" function named **image()**, whose first parameter is the created array. And the second argument is the position where the image will be displayed.

Some images on how it works [here](https://github.com/ManuelSN/Pixel_and_Play_Arduino_Application/tree/main/images).

You can see a demo of some games using different Arduino sensor incorporated in this [video](https://www.youtube.com/watch?v=bXoufN0ipHg).

That's all!

# Support

For any question, issue, help or if you want to collaborate, contact with me on my personal email address lolosancheznatera@gmail.com.



