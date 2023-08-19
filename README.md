# Cross Verification of Images for Eyecare

### Introduction
Sankara Eye Foundation USA is a not-for-profit missionary institution for ophthalmic care. They are Donors who fund cataract surgeries for the underprivileged. For this purpose, they fund eye hospitals based on free cataract surgeries performed. Funds are released based on the number of operations performed. 

The NGO must ensure that the funds are released only for genuine surgeries. As proof that the surgery is performed, the NGO requests eye hospitals to send in pre-operation (pre-op) and post-operation (post-op) photographs of the patient’s face for each surgery.

The NGO then verifies the pre-op and post-op images to ensure the surgery is performed before releasing funds. They also need to verify that photographs of the same patients are not being sent repeatedly to claim funds fraudulently.

They need a system that will help compare these photographs to highlight cases with a high probability of fraud. These can then be further investigated manually.

### Problem Statement of the NGO

Pre-op and post-op photographs will be provided. The NGO needs a system that will help compare the pre and post-operative images and identify that this is the same patient with a high level of confidence. They also want the system to be able to compare the pre-op photographs with an existing database of pre-op images and post-op photographs to a database of post-op images to ensure that the pictures have yet to be previously submitted.

The post-operative pictures captured have a part of the patient's face covered with a patch. The existing facial recognition algorithms available require all the parts of the face to be visible. Hence when a part of the face is covered with the patch, these algorithms are ineffective.

The problem is to find a solution that will be able to detect and match the patients from pre-op and post-op images to confirm it is the same patient (even when part of the face is covered with a patch )
The algorithm should also detect or identify if the images are photoshopped.

![Sample Image](http://deepblue.co.in/wp-content/uploads/2017/08/Cross-Verification-example.jpg)

### What the NGO Wants?

The system should be able to recognize and match the pre and post-operative photographs with a high degree of accuracy to check that they are the same person even when the part of the eye in the post-op image has a patch.

The case should be highlighted for manual verification if
* The pre-op image matches a pre-op image in the existing database
* A post-op image matches the post-op image existing in the database
* The pre and post-operative pictures submitted for the case do not match
* Image is detected as possibly photoshopped.

### The Challenge

The system must be able to match with a high level of accuracy that the patient in the pre-op and post-op image is the same person (even with the eye patch). The system must also be able to detect with a high level of confidence if the pictures of the same patient are submitted twice. The system should also be able to identify images that are photoshopped. The images which look suspicious should be highlighted for further manual investigation.

### Setup Instructions

1. Go to the root folder of the repository
`cd EYC3PDBS3`

2. Create conda environment from the yml file
`conda env create -f environment.yml`

> **Note**
> Conda must be installed in your machine to perform this action

4. Activate the Environment
`source activate python35.`

5. Run the flask application inside the main/demo to visualize the algorithm.

6. Run the Flaks application inside the main/app to view a demo of the end-user application.

### Developed by EYC3

