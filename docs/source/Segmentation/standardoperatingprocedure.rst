Pectoral muscle MRI segmentation:
Standard Operating Procedure
1. Introduction
This document sets out the standard operating procedure (SOP) for manual segmentation of the pectoral muscles from MR images using the MITK software package. It consists of the details regarding the use of the software, study plan, and procedures for obtaining the manual segmentations.
2. Software version(s) and special features
2.1 Software version(s)
MITK 2018.04.2
2.2 Accessing the software
Firstly, you must download MITK software on the website: www.mitk.org/wiki/Downloads and choose the best version 2018.04.2.
After the download, go in the folder Downloads and extract the folder MITK and then, open the extracted folder bin. You can open the application MitkWorkbench.
2.3 Special features
The following special features or constraints apply to the study:
Semi-automated segmentation tool
identify which tools (if any) should be used

3. Accessing data
3.1 Mounting breast group eResearch drive
The drive containing the MRI images can be mounted on windows using the following steps:

Go to https://uoa-eresearch.github.io/vmhandbook/doc/map-drive-windows.html and follow instructions
Your project/research group has a storage drive managed by \\files.auckland.ac.nz\research\resabi201900007-biomechanics-for-breast-imaging

3.2 Location of MR images
The MR images are located in F:\Vault\Segmentations\Manual\VL01\T2_prone\maj_pectoral
3. Study plan
Training and group review
Three scans will be randomly chosen for training purposes and group review. Regular group reviews will be held to ensure that each segmentation is done properly and to the satisfaction of the review group.

The review group members include analysts, Dr Anthony Doyle (breast radiologist), Marianne Sanchez (investigator), Gonzalo Maso Talou, Prasad Babarenda Gamage, Poul Nielsen, Martyn Nash.

First-Run and Inter/Intra observer Analyses
The study consists of two steps: First-Run Analysis and Inter/Intraobserver Analysis.

In the First Run Analysis, two analysts are required to independently perform all the pectoral muscle MRI segmentations.
VL00034 prone

After finalising the first run study, twenty percent of the MRI cases will be selected at random as the repeat cases for Inter/intraobserver error and consistency check. During the Inter/Intraobserver Analysis, the two analysts should be blinded from their previous results.

Repeat and reconciliation analysis
The segmentation repeat and reconciliation analyses will be conducted after the first run and inter/intraobserver analysis. The threshold for this analysis will be generated based on the first run and inter/intraobserver results.

Documentation of problem cases
In situations where a case is identified as having an unusual anatomical feature or unique problem not covered in this procedure, there should be a group review of the case. The group will determine the disposition of the case. The nature of the problem and decision made will be documented in a Case Review document.
4. Definition of the pectoral muscle boundaries
The boundaries of the pectoral muscle are outlined below.
Medial border
Axila border
Caudal border
Cranial border

































5. Procedure
There are two ways that a segmentation can be created. These two ways will be described using VL00034 as an example.
Correction of an existing segmentation


In MITK, click on “Open File”.
Load an existing segmentation by navigating to the segmentation folder in the eResearch Drive and select one case e.g. VL00034 (you can find the location of the images as described  in Section 3.2). The segmentation will appear in the “Data Manager panel” on the left side of the MITK GUI..
Load the MR images by navigating to the image folder in the eResearch Drive e.g. Navigate to Z:\Vault\Datasets\VL01\00034\MRI_T2_prone, and select the MRI image for the case 34, and then click open. The MRI image will appear in the “Data Manager panel” on the left side of the MITK GUI.
Select the MRI in “Data Manager panel”and click on the “Segmentation” button in the right corner of the MITK GUI:

A new window will appear on the right of the MITK GUI with different tools for segmentation.

Click on New, a small window will appear in the center of the MITK GUI. Select the color and give the name to the segmentation Pectoral_VL00034.
Manually create the segmentation from scratch.
In MITK, click on “Open File”.
Load the MR images by navigating to the image folder in the eResearch Drive e.g. Navigate to F:\Vault\Datasets\VL01\00034\MRI_T2_prone, and select the MRI image for the case 34, and then click open. The MRI image will appear in the “Data Manager panel” on the left side of the MITK GUI.
Repeat steps 5.1.d - 5.1.f
Setup
View
To have a better view, you can select one of the four proposed and click on the blue square. For the sagittal view:

The easiest plan to segment is the Axial window.

Contrast and brightness - Adjust the contrast and brightness to show the images to best advantage.
You can also change the contrast if you encounter difficulties with the original image by changing the values (right corner). You have to test different values by yourself because it depends on the MRI.
For example : the default numbers in the case VL0008 are 161 and 320 but if I change the first number, the difference appears.
If I am changing the first number, I will obtain these results:
with 190
with 142
If I am changing the second number, I will obtain these results: with 350
with 290
You have to try different values to help yourself. You can change it all the time, some slides could be more difficult than others and don’t hesitate to use both at the same time.
Include any other setting that you use

You can move in the different plans with Image Navigator.


Generation of pectoral muscle segmentations
The steps to produce appropriate pectoral muscle segmentations include different tools :
Add and Subtract
The tools Add and Subtract permit to select an area of the pectoralis major muscle, but this tool is not precise.
Paint
The tool paint is the easier tool to perform the segmentation. It takes more time, but the borders are well defined. Then, you can fill the selection with the tool fill and correct it if you need with the tool wipe.
Region Growing
The tool Region Growing could be interesting because it selects areas by itself but most of the time, you need to correct it because it takes more or less.
Final review
A final review of the pectoral muscle segmentations should be made, ensuring all contours of the segmentations are positioned properly.
Save
Save the segmentation in the folder F:\Vault\Segmentations\Manual\VL01\T2_prone\maj_pectoral with the name VL000XX_Pectoral_muscle. In this folder, you can only save the segmentation not all the project. Right click on the segmentation file and select Save...
For more information, go on http://docs.mitk.org/2016.11/org_mitk_views_segmentation.html
