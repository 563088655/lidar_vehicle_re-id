# lidar_vehicle_re-id
A method to compare the individual vehicle feature from the deep learning model to get the Correlation coefficient. You need to prepare the feature vector from a deep learning detect model and the data set or real world label file and calib file, the kitti data set and openpcdet be used in our experence. And we modified the feature's size to compare the different size vectors, please along your need to modify taht parameter.


## Requirements
- Python 3.x
- PyTorch
- NumPy
- Path
- pickle
- scipy
- Pillow


## Usage
To use the Feature Comparator, you need to specify the paths to the directories containing the `.pth` files (the feature vector from the detect model's backbone in Forward Propagation) for both datasets you wish to compare.

Ensure you have the required packages, and prepare the pth files, calib file, and label file, respectively. And you need modify the code if you don't want use those data set.

This project need to run the save_input_dict_files.py to save the every information we need, and run the save_things_feature_by_idx.py to get the individual feature, and finally run the compare_vectors.py to get the Correlation coefficient.

License
This project is licensed under the Apache License 2.0 License - see the LICENSE file for details.
