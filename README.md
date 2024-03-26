# Background-Assignment

How to execute code:
* Download and open the background assignment.py file in Google Colab
* Upload the examples folder in My drive of Google drive
* Execute the code (run all cells)
* Output is saved in My Drive of Google Colab

I have done assignment in Google colab "background assignment.py" file

Task 1: 
Input : Image with white background
Output : Generate a text-conditioned scene with the image placed naturally in the scene.

To perform task 1, the stable diffusion inpainting model is used. It takes input parameters as prompt, image, mask image, guidance scale, generator, num of samples.

Prompts used for generating images are present in 'prompts.txt' file

Mask image is generated using YOLO model 'yolov8m-seg.pt'

For guidance scale, numbers like 7 to 8.5 give good results and forces the generation to better match with the prompt.

Number of samples is taken as 1

Task 2 :
* A small video output obtained by generating multiple frames
* Zooming out of the scene gradually

Generated images in task 1 are considered to create frames required for video generation.

The zooming effect is achieved by adjusting the cropping and scaling parameters of the original image.

Parameters are video dimensions, frames per second (fps), duration, starting and ending center points for zooming, starting and ending scales.

# Output for required task are attached in the repository mask images, prompts, videos
