# Image-Based Geolocation Detection in Indoor Environments

This project aims to develop methods to detect the fine-grained geolocation of images, particularly in settings where traditional GPS coordinates and network addresses are insufficient, such as in small indoor and outdoor environments. Using a combination of a Convolutional Neural Network (CNN) model and feature matching techniques (SIFT and FLANN), the project recognizes the exact location of testing images within a museum by comparing them with training images of known locations.

## Project Overview
1. **Objective**: To determine the precise geolocation of testing images using machine learning and computer vision techniques.
2. **Methods**:
   - **CNN (Convolutional Neural Network)**: Trains on labeled images to predict coordinates of new, unlabeled images.
   - **Feature Matching (SIFT & FLANN)**: Extracts and matches features between known and unknown locations for location prediction.

## Structure

1. **Images Folder**: Place both `train` and `test` image folders in the same directory as the code.
2. **Training Data**: The `train.csv` file contains coordinates for training images and should be placed alongside the code files.

## Running the Models

### CNN Model
1. Open `cnn.ipynb` and run each cell sequentially.
2. **Note**: Skip the block that plots the coordinates (optional for essential output generation).
3. The script generates `output_cnn.csv`, which contains the predicted coordinates for the test images.

### SIFT & FLANN Feature Matching Model
1. Open `sift.ipynb` and execute each cell block-by-block.
2. **Note**: Skip the testing block that plots result images of SIFT (optional).
3. The script generates `output_sift.csv` with the predicted coordinates based on feature matching.

## Conclusion

Each method has distinct strengths:
- The **CNN model** provides a learning-based approach to location prediction.
- **Feature Matching** via SIFT and FLANN leverages detailed image features for high-precision matching.
- The combination of both methods enhances overall accuracy and robustness in fine-grained geolocation detection.

## License

This project is not licensed for distribution or modification. University students are permitted to reference this repository for educational purposes only. Copying or reproducing any part of this project without proper attribution may lead to serious plagiarism issues and academic consequences. Please ensure that any use of this material complies with your institution's academic integrity policies.
