# MATLAB Multimedia Functions
A repository containing various MATLAB functions pertaining to multimedia including image/signal/video processing. Additional graphing scripts included.

<hr>

### Folder: Importing Video Files
• Grabs frames of video (mp4, mov, avi, etc) and stores in structure ready for processing/analysis.

|<img src="README Images/Import_Video_Frames.png" width = "600">|<img src="README Images/Import_Video_Frames.gif" width = "600">|
|---|---|

[Source Files: Importing Video Files](https://github.com/MichaelTr7/MATLAB-Multimedia-Functions/tree/master/Importing%20Video%20Files)

<hr>

### Folder: Scaled Fourier Transform
• Generates the Fourier Transform of a sinusoidal signal dependent on sampling frequency.
<br/>
• Uses the DSB (Double Side Band) form of showing the transform.


|Fourier Transform Sinusoid Frequency = 50Hz at Sampling Frequency = 1000Hz|Fourier Transform Sinusoid Frequency = 200Hz at Sampling Frequency = 1000Hz|
|--|--|
|<img src="README Images/Scaled_Fourier_Transform.png" width = "600">|<img src="README Images/Scaled_Fourier_Transform_2.png" width = "600">|

[Source Files: Scaled Fourier Transform](https://github.com/MichaelTr7/MATLAB-Multimedia-Functions/tree/master/Scaled%20Fourier%20Transform)

<hr>

### Folder: 3D-Plots in MATLAB App-Designer
• Plots spheres and circles on a 3D axes with adjustable centre positions. <br/>
• Can plot wireframes or shell shaded plots using surf.


|Circle Wireframe 3D-Plot|Sphere Wireframe 3D-Plot|Sphere Surf 3D-Plot|
|--|--|--|
|<img src="README Images/3D_Circle.png" width = "500">|<img src="README Images/3D_Sphere.png" width = "500">|<img src="README Images/3D_Sphere_Surf.png" width = "500">|

[Source Files: 3D-Plots in MATLAB App-Designer](https://github.com/MichaelTr7/MATLAB-Multimedia-Functions/tree/master/3D-Plots%20in%20Matlab%20App-Designer)

<hr>

### Folder: MATLAB App-Designer User Set Table
• Takes inputs as table headers/labels and creates a table of N by N size where, N is equal to the number of table headers/labels. <br/>
<p align = 'center'><img src="README Images/User Size Chosen Table.png" width = "300"></p> 

[Source Files: MATLAB App-Designer User Set Table](https://github.com/MichaelTr7/MATLAB-Multimedia-Functions/tree/master/MATLAB%20App-Designer%20User%20Set%20Table)

<hr>

### MATLAB Script to Strip Location Data from Smartphone Photos

```
%Script to strip location data of a folder of images%

%Directory path where the images are stored in a folder%
Directory_Path = "";
Image_File_Names = [dir("*.png")' dir("*.jpg")'];


for Image_Index = 1: length(Image_File_Names)

Image = imread(Image_File_Names(Image_Index).name);
Path = ['/Users/michael/Desktop/Exported_Images/Image' num2str(Image_Index) '.png'];
imwrite(Image,Path,'Mode','lossless');

end
```



