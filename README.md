![ASL](https://github.com/sourceduty/ASL_GIF_Maker/assets/123030236/8ed1ee06-8fe4-4f88-8040-51e8bec1caab)

> Create single word GIFs in American Sign Language (ASL).

#

This Python script was developed for creating animated GIFs that spell out words in American Sign Language (ASL) using a sequence of images, each representing a different ASL letter. The user inputs a word, and the program assembles a GIF from corresponding images stored in a folder. Each image file is named after the letter it represents (e.g., A.jpeg, B.jpeg), making it straightforward for the program to locate and use the correct images based on the user's input.

The script begins by defining a function create_gif_from_word, which ensures that the necessary directories for input images and output GIFs exist. It then converts the input word to uppercase and constructs a list of image file names that correspond to the letters in the word. This step is crucial because it aligns with the naming convention of the images in the folder, ensuring that the program can accurately retrieve each letter's image. The program checks if all required images are present in the input folder, and if any are missing, it raises an error and notifies the user. This validation step helps prevent issues that could arise from missing files and ensures that the GIF can be created successfully.

Once the necessary images are verified, the program opens each image and stores them in a list. Using Pillow, the first image in the list becomes the base frame of the GIF, while subsequent images are appended to it, creating the animation. The GIF is set to display each frame for 500 milliseconds and to loop indefinitely, ensuring continuous playback. The final GIF is saved in the output directory with a filename derived from the input word. This process allows users to create dynamic, animated representations of words in ASL, making it a valuable tool for educational purposes and for those learning or teaching sign language. The user-friendly design and error handling make it accessible even for those with minimal programming experience.

***
Copyright (C) 2024, Sourceduty - All Rights Reserved.
