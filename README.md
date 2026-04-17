## Fish Segmentation and Classification Project

This project provides a large-scale dataset and code for the segmentation and classification of various fish species. It includes detailed image datasets, ground truth labels, and scripts for deep learning-based image analysis.

### Authors
O. Ulucan, D. Karakaya, M. Turkan  
Department of Electrical and Electronics Engineering, Izmir University of Economics, Izmir, Turkey  
Contact: mehmet.turkan@ieu.edu.tr

---

## Project Structure

```
├── Fish_Dataset/
│   ├── [Class Name]/
│   │   ├── [Class Name]/            # RGB images (00001.png ... 01000.png)
│   │   └── [Class Name GT]/         # Ground truth masks (00001.png ... 01000.png)
│   ├── README.txt                   # Dataset description
│   └── license.txt                  # License (CC BY 4.0)
├── NA_Fish_Dataset/
│   ├── [Class Name]/                # Natural images (JPG/PNG) for each class
├── Segmentation_example_script.m    # MATLAB script for segmentation
├── TP6.ipynb                        # Python notebook for DNN classification
├── README.md                        # This file
├── README.txt                       # Dataset publication and citation
├── license.txt                      # Project license
```

---

## Dataset Overview

### Fish_Dataset
- **Purpose:** For segmentation and classification tasks.
- **Classes:**
	- Black Sea Sprat
	- Gilt-Head Bream
	- Hourse Mackerel
	- Red Mullet
	- Red Sea Bream
	- Sea Bass
	- Shrimp
	- Striped Red Mullet
	- Trout
- **Structure:**
	- Each class contains 1000 RGB images and 1000 ground truth masks (segmentation labels).
	- Images are named sequentially (e.g., 00001.png ... 01000.png).
	- Ground truth masks are in the `[Class Name GT]` subfolder.
- **Image Size:** All images resized to 590x445 pixels.
- **Augmentation:** Images are augmented by flipping and rotating.
- **License:** Creative Commons Attribution 4.0 International (CC BY 4.0).

### NA_Fish_Dataset
- **Purpose:** For natural image classification and DNN training.
- **Structure:**
	- Each class folder contains natural images (JPG/PNG) of the fish species.
	- Used in the Python notebook for deep learning experiments.

---

## Scripts and Notebooks

- **Segmentation_example_script.m**
	- MATLAB script for semantic segmentation using the Fish_Dataset.
	- Explains how to set up image and label directories for training segmentation models.

- **TP6.ipynb**
	- Python notebook for deep learning-based fish species classification.
	- Steps include data loading, preprocessing, augmentation, model training, evaluation, and visualization.
	- Uses NA_Fish_Dataset for image classification tasks.

---

## How to Use

1. **Segmentation Tasks:**
	 - Use the Fish_Dataset and the provided MATLAB script to train and evaluate segmentation models.
	 - Each class has paired RGB images and ground truth masks.

2. **Classification Tasks:**
	 - Use the NA_Fish_Dataset and the Python notebook (TP6.ipynb) for DNN-based classification.
	 - The notebook covers data exploration, preprocessing, augmentation, model building, and evaluation.

---

## Citation

If you use this dataset or code, please cite:

@inproceedings{ulucan2020large,
	title={A Large-Scale Dataset for Fish Segmentation and Classification},
	author={Ulucan, Oguzhan and Karakaya, Diclehan and Turkan, Mehmet},
	booktitle={2020 Innovations in Intelligent Systems and Applications Conference (ASYU)},
	pages={1--5},
	year={2020},
	organization={IEEE}
}

---

## License

This project and datasets are licensed under the Creative Commons Attribution 4.0 International License (CC BY 4.0). See license.txt for details.
