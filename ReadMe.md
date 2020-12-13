# Annotation Tool for Head Detection
This tool is developed from YOLO Annotation Tool. For more information, please check this blog: [Yolo Annotation Tool-New](https://manivannan-ai.medium.com/yolo-annotation-tool-new-18c7847a2186).

#### Steps for execution
1. Before running this annotation tool, make sure these two folders ( __Images/__, __Labels/__ ) and the file <kbd>classes.txt</kbd> are in the same directory of <kbd>main.py</kbd>.

1. Keep all images in the folder __Images/__.

1. Modify <kbd>classes.txt</kbd> to set the class names.

1. Run <kbd>main.py</kbd> in Python3.

1. Fill the directory of images in  `Image Dir` box by typing `./`, and click `load` button.

1. Select the region of interest.

1. The output will be saved in the folder __Labels/__ by clicking buttons `<<Prev`, `Next>>`, or going to other images.

#### Directory structure after running:
```
AnnotationTool
│   ReadME.md
│   classes.txt    
│   main.py
|
└───Images
│   │   G-C1L1P-Mar30-C-Kelly_q2_02-06_120.jpg
│   │   G-C1L1P-Mar30-C-Kelly_q2_02-06_3840.jpg
│   |   ...
│          
└───Labels
    │   G-C1L1P-Mar30-C-Kelly_q2_02-06_120.txt
    │   G-C1L1P-Mar30-C-Kelly_q2_02-06_3840.txt
    |   ...
```

#### The output format
```
class_id  x_start  y_start  x_end  y_end  class_name
```
`(x_start, y_start)` is the coordinate of the top-left corner.
`(x_end, y_end)` is the coordinate of the bottom-right corner.


##### The output example
```
0 38.0 208.0 100.0 297.0 Cindy14P
1 159.0 157.0 231.0 241.0 Carmen13P
3 749.0 242.0 823.0 307.0 Marta12P
2 651.0 218.0 713.0 280.0 Marina15P
5 433.0 102.0 483.0 166.0 Kelly
```
