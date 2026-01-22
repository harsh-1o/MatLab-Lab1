# MATLAB Image Brightness Adjustment

This is my first MATLAB lab project 🎉.  
The project demonstrates how to perform **basic image processing** operations such as darkening and brightening an image using MATLAB.

---

## 📌 Project Overview
The script:
- Reads an image from the computer.
- Creates a **darkened version** of the image by subtracting pixel values.
- Creates a **brightened version** of the image by adding pixel values.
- Displays the **original**, **darkened**, and **brightened** images side by side.

---

## 🖼️ Example Workflow
1. Load an image (`1.jpg`).
2. Apply brightness adjustments:
   - Darkened Image = `img - 50`
   - Brightened Image = `img + 50`
3. Display results using `subplot`.

---

## 📂 Code
```matlab
clc;
clear;
close all;

% Read image
img = imread("C:\Users\Student\Pictures\1.jpg");

% Darkening the image
dark_img = img - 50;

% Brightening the image
bright_img = img + 50;

% Display result
figure;

subplot(1,3,1);
imshow(img);
title("Original Image");

subplot(1,3,2);
imshow(dark_img);
title("Darkened Image");

subplot(1,3,3);
imshow(bright_img);
title("Brightened Image");
