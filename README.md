# Diagnosis-of-Glaucoma-Using-Retina-Fundus-Images

## Overview
This project was successfully completed by my team and me during our tenure as research interns with the IEEE CS Bangalore Chapter. The study focuses on analyzing retinal fundus images to determine whether a patient has glaucoma.

## Process
The procedure consists of three major parts:

**Region of Focus Identification:**

1. Region of Focus Identification:
   - Images are processed through a basic U-network where they are downsampled, processed, and upsampled to identify the region of focus (binary image).

2. Region of Interest Segmentation:
   - The focused image is fed through DDSC-Net for segmentation.
   - The cup and disc are detected, and circles are drawn around them, marking the end of preprocessing.

3. Analysis for Glaucoma:
   - Preprocessed images are turned into binary images with two circles representing the cup and disc.
   - OpenCV algorithms compute the approximate radius of the cup and disc.
   - The cup-to-disc ratio is used to diagnose glaucoma.
  
## Diagnosis Criteria

- A threshold of 0.4 is established based on consultations with doctors and web sources.
- A cup-to-disc ratio less than 0.4 is considered healthy.
- Patients are classified as having glaucoma or not based on this characteristic.

## Dataset
The dataset can be accessed from:
- https://riadd.grand-challenge.org/download-all-classes/
- https://drive.google.com/file/d/1teYi_smpLiNZNJcTWdxXgKKLW2fkUQr4/view

## Thank You

