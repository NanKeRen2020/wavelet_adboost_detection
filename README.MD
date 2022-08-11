About
=====

A nonrigid and rigid object including face face detection algorithm based on orthogonal wavelet 

with linear phase.This algorithm inspired from Viola-Jones haar-adboost, replace  

Haar-like templates with orthogonal wavelet templates.


Environments
=============

Ubuntu1604  OpenCV 3.4.x


Build & Run Instruction
=======================

To build this project, you must copy all cpp file to replace corresponding file 

in opencv-3.4.x/apps/traincascade/ folder after download opencv source code.

You can reference to OpenCV buid instruction https://docs.opencv.org/3.4.16/d7/d9f/tutorial_linux_install.html.

After build complete, you can find named opencv_traincascade excute binary with orthogonal wavelet feature 

in opencv-3.4.x/build/bin/.


opencv_traincascade usage reference to opencv homepage instruction 
https://docs.opencv.org/3.4.16/db/d28/tutorial_cascade_classifier.html
https://docs.opencv.org/3.4.16/dc/d88/tutorial_traincascade.html


Why Wavelet Template
====================

1) Wavelet feature is 2D nonseperable based on wavelet theory, 

which can detect any shape object including non rigid on image.

While haar feature is more suitable to detect rigid object on image,

such as huamna face of image, otherwise it cannot get good detcion result.

2) Less feature number becase of Less feature templates than haar feature templates, 

but can get complete feature representation for detcion object. 

Bacase wavelet templates is 2D nonseperable, which can get all detail information in arbitrary dirction.


References
==========

[1] Peng, SL,et al."Construction of two-dimensional compactly supported orthogonal wavelets filters with linear phase".
    ACTA MATHEMATICA SINICA-ENGLISH SERIES 18.No.4(2002):719–726.
[2] P. Viola and M. J. Jones, Robust real-time face detection, International Journal of Computer Vision, 57 (2004), 
    pp.137–154. http://dx.doi.org/10.1023/B:VISI.0000013087.49260.fb. 







