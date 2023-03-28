# High-Resolution CT Scan Segmentation
This repository contains an algorithm to segment high-resolution CT scans. The tasks for this project are divided into two parts: programming and software usage.

## Preprocessing and Segmentation
In this task, the CT-CASE15 (.dcm) image is downloaded, and if necessary, preprocessed. The lung-airway is then segmented from the 3D-CT image using thresholding, region growing, graph-cut or any other advanced method. The CT image is saved slice by slice in DICOM format where each slice is 2D. The slices of data can be read in the workspace and stacked back to 3D, or some software can be used to convert it to 3D.

## Evaluation
The scan does not include a significant amount of pathology, so even conventional methods may work up to some point. The ground truth is not shared, so visual inspection is used to decide if the segmentation is reasonable or not. A descriptive report is presented, summarizing the key processing steps associated with outputs (image screenshot), and includes insights.

## Segmentation Usding 3D Slicer
In this task, 3D Slicer is used to segment the airway tree from the high-resolution CT scan. Lungs are segmented using thresholding, region growing, or any other advanced method. Airways are segmented using region growing or any other advanced method. Lungs and airways are rendered in different colors, and they are visualized individually and also together using opacity parameters.

## EXACT09 Airway Segmentation Challenge
For more information about airway segmentation challenge EXACT09, and some available methods in the website along with their explanations, check here: 
http://image.diku.dk/exact/
