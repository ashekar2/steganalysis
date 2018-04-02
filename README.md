# Steganalysis for Images

This notebook explores the idea of steganaylsis - the study of detecting messages hidden using steganography; this is analogous to cryptanalysis applied to cryptography. The application will be on images. This file enables the following functionalities:
* Encoding an image into another image - hide a secret in an image!
* Decode the sed encoded image in order to retrieve the hidden information.

Methodologies:
* We make use of Least Significant Bit (LSB) encoding in order to "hide" the secret image in the visible image.
* We consider each pixel to be represented by 8 bits (in order to achieve a range of 0-255)
* We take the 4 Most Significant Bits of the secret image and "hide" them in 4 Least Significant Bits of the visible image.
* We apply the reverse process in decoding the image.

Requirements:
* python 3.5
* pillow
