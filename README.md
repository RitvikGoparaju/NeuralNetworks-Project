OpenCV and tensorflow are the required libraries to run the project. Open a terminal, navigate to the project directory and run the following command lines in the terminal. Here is an example of how to run the code.
Download the VGG-19 model weights. Download it from the link "http://www.vlfeat.org/matconvnet/pretrained". 
After downloading, copy the weights file to the project directory.

For Simple Style Transfer -
python neural\_style1.py --content\_img pengu.jpg --style\_imgs rok.jpg --max\_size 1000 --max\_iterations 50 --device /gpu:0
For Multiple Style Transfer -
python neural\_style1.py --content\_img pengu.jpg --style\_imgs rok.jpg starry-night.jpg --style\_imgs\_weights 0.5 0,5 --max\_size 1000 --max\_iterations 50  --device /gpu:0
For Segmentation Style Transfer -
python neural\_style1.py --content\_img pengu.jpg --style\_imgs rok.jpg --style\_mask 1 --style\_mask\_imgs face\_mask.png --max\_size 1000 --max\_iterations 50  --device /gpu:0

