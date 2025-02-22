# Image-Feature-Extraction
COCO Feature Extraction with Pretrained Models
Overview
This project extracts image features from the COCO 2017 validation dataset using pretrained deep learning models like ResNet101, GoogLeNet, and ZFNet (AlexNet alternative). The extracted features are used to find the 10 nearest neighbors for selected object classes.

Dataset
COCO 2017 Validation Set (Download)
Extracted features are used to compare results across multiple models.
Models Used
ResNet101 🏋️
GoogLeNet 🔍
ZFNet (AlexNet alternative) ⚡
Project Workflow
Download & Extract the COCO dataset.
Load Annotations and select images from specific classes: person, car, dog, cat, airplane, bottle.
Apply Transformations and load images into a PyTorch DataLoader.
Load Pretrained Models and remove the last fully connected layer.
Extract Features and compute Euclidean distance to find similar images.
Visualize Nearest Neighbors for each class.
Setup & Usage
Requirements
Make sure you have the following installed:

bash
Copy
Edit
pip install torch torchvision numpy scipy matplotlib pillow
Running the Code
Clone the repository:
bash
Copy
Edit
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
Run the notebook:
bash
Copy
Edit
jupyter notebook coco_feature_extraction.ipynb
Results
The output displays the 10 nearest neighbors for each selected class using different models.

Example Output
yaml
Copy
Edit
Results for ResNet101:
Class person -> Nearest Neighbors: [  73  130  265 1057   87 1043  154  588 1231 1247]
Class car -> Nearest Neighbors: [ 164 3117 1600 6183 6169 6179 6176 6582 6551 6657]
...
Future Improvements
Extend to more object categories.
Experiment with different similarity metrics.
Implement a web app for visualization.
Contributors
Your Name
Feel free to contribute! Fork & submit a pull request 🚀