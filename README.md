# Text-Extraction-Table-Image

This project aims to extract text from a table image into python objects. Below is a result of the detection:

![test case](/images/result1.gif)

## Prerequisites/Dependencies  
* OpenCV => 2.4.8
* Numpy
* PyTesseract

## Idea Behind The Code

I've publisehed the documentation on [my website](https://fazlurnu.com/2020/06/23/text-extraction-from-a-table-image-using-pytesseract-and-opencv/). Please read it to understand the idea behind the code.

## For Refinement

After your algorithm can detect the text successfully, now you can save it into Python object such as Dictionary or List. Some regions name (in the “Kabupaten/Kota” are failed to be detected precisely, since it is not included in Tesseract training data. However, it shouldn’t be a problem as the regions’ indexes can be detected precisely. Also, this text extraction might fail to detect the text in other fonts, depending on the font used. In case of misinterpretation, such as “5” is detected as “8”, you can do an image processing such as eroding and dilating.

My code is far from perfect, if you find some error or chances of refinement, write me a comment!
