import cv2

from PIL import Image

from pytesseract import image_to_string


`cd Download`

`$ mv kor.traineddata /usr/local/share/tessdata`

`$ mv chi_tra.traineddata /usr/local/share/tessdata`

img = "ex1.png"

text = image_to_string(img, lang = "kor")

text.split("\n")

