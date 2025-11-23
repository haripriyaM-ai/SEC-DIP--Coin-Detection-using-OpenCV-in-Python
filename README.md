# WORKSHOP – 4: Coin Detection Using OpenCV in Python
## NAME : HARI PRIYA M
## REGISTER NO : 212224240047

## AIM

To detect and count coins in an image using OpenCV methods such as grayscale conversion, thresholding, morphological operations, Blob Detection, and Hough Circle Transform, and to compare their performance.

## SOFTWARE USED
- Python 3.x
- OpenCV
- NumPy
- Matplotlib
- Jupyter Notebook / VS Code


## WORKING PROCEDURE
1.Loaded and displayed the coin image for initial observation. <br>
2.Converted the image to grayscale to reduce complexity. <br>
3.Applied thresholding, but results were noisy due to uneven lighting. <br>
4.Performed morphological operations (erosion, dilation, opening, closing), but they failed to isolate coins cleanly. <br>
5.Attempted blob detection using cv2.SimpleBlobDetector with parameters like area and circularity.

## OUTPUT 
<img width="600" height="420" alt="Screenshot 2025-11-23 020105" src="https://github.com/user-attachments/assets/eb7e21fd-f127-4393-a3c4-62bd670fa8a1" />

## Result:
Detected counts were incorrect (2, 6, 15, and 0 coins) due to fragmented shapes and noise interference.
Blob detection proved unreliable for this dataset.
Hough Circle Transform was applied to detect circular coin shapes directly from blurred grayscale image.

## Final Result:
Number of coins detected: 9


## CONCLUSION

Morphological processing and blob detection were unsuitable for this coin image due to textured background interference and broken segmentation.
Hough Circle Transform correctly identified all 9 coins by detecting circular edges, making it the most effective method for this task.
