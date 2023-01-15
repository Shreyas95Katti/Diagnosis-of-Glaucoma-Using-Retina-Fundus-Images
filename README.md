# Diagnosis-of-Glaucoma-Using-Retina-Fundus-Images
Greetings!!

A project accomplished successfully while my team and I were research interns with the IEEE CS Bangalore Chapter. The study entails analysing retinal fundus images obtained from multiple sources. The model is taught to determine whether or not a patient has glaucoma. This procedure consists of three major parts. First, the region of focus in the whole fundus picture is identified by running the images through a basic U-network where the image is initially down sampled, processed, and up sampled to obtain the final region of focus (binary image). The picture with the primary region of focus is then fed through the DDSC-Net for region of interest segmentation,in the second stage. The cup and disc are detected in this segmented picture, and a clear circle is drawn around them. This new final image indicating the cup and disc boundaries marks the end of preprocessing. All pre-preparation photos are saved and then analyzed for glaucoma. The pre-processed photos are turned into binary images with two circles on a black backdrop to represent the cup and disc. OpenCV algorithms are used to compute the approximate radius of the cup and disc. The cup-to-disc ratio indicates whether or not the patient has Glaucoma.

We established a 0.4 threshold after checking with a few doctors and other web sources. Any cup to disc ratio less than 0.4 is considered a healthy eye, and the patient is classed as having Glaucoma or not depending on this characteristic.

The dataset can be accessed from:
https://riadd.grand-challenge.org/download-all-classes/
https://drive.google.com/file/d/1teYi_smpLiNZNJcTWdxXgKKLW2fkUQr4/view

## Thank You
