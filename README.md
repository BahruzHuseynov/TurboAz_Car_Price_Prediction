<div align="center">
   <h1> Car Price Prediction based on scraped dataset</h1>
</div>

This project focused on learning and involved creating a dataset through web automation and scraping techniques. The collected data was then used to develop a car price prediction model for Azerbaijan's car market.

## Technology
- **Python**: Main programming language. <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt = "Python" height="30" >
- **Selenium**: An open source project to automate browsers. <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9f/Selenium_logo.svg/2560px-Selenium_logo.svg.png" alt="Selenium"  height="30"  />
- **Scikit-learn**: An open-source library in Python that helps us implement machine learning models. <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/05/Scikit_learn_logo_small.svg/2560px-Scikit_learn_logo_small.svg.png" alt="Scikit-learn"  height="30"  />
- **Numpy**: Used for numerical computations and efficient handling of large arrays and matrices, often applied in processing video frames. <img src="https://cdn.worldvectorlogo.com/logos/numpy-1.svg" alt="NumPy" height="30" />
- **Pandas**: A powerful library for data manipulation and analysis, often used to preprocess and manage tabular data. <img src="https://seeklogo.com/images/P/pandas-icon-logo-BE10401BF1-seeklogo.com.png" alt="Pandas" height="30" />
- **Seaborn**: A visualization library built on Matplotlib, used for creating attractive and informative statistical graphics. <img src="https://user-images.githubusercontent.com/315810/92159303-30d41100-edfb-11ea-8107-1c5352202571.png" alt="Seaborn" height="30" />
- **Matplotlib**: A comprehensive library for creating static, animated, and interactive visualizations in Python. <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/84/Matplotlib_icon.svg/768px-Matplotlib_icon.svg.png" alt="Matplotlib" height="30"/>

## Google Colab <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSArk3D34rWqNoPw4_n-ovyK0lz3yvknTVZd9yeCdZrsdDEViqoPMmjhFWD-iy4NO1UiyI&usqp=CAU" alt="Colab" width="40">
- To train or fine-tune detection and segmentation models, usage of GPU is recommended.
- During research, codes have been executed in Google Colab as it is a hosted Jupyter Notebook service that provides free access to computing resources, including GPUs and TPUs.

## Dataset
- In this research, the dataset was manually created using a smartphone, consisting of 12 videos — 10 for training and 2 for testing. These videos capture conveyor belts with LEGO bricks from multiple angles with varying complexities for diversity. LEGO bricks were annotated frame-by-frame using RoboFlow (https://roboflow.com/), which was the most time-consuming step.
- Dataset is publicly available in Kaggle: https://www.kaggle.com/datasets/hbahruz/multiple-lego-tracking-dataset

## Pipeline
<div align="center">
   <img src="images/Pipeline_Main.png" alt="Pipeline" width="700">
</div>

## Pre-trained parameters
- The folder contains .pt files of YOLOv8 and RT-DETR detection models which are the saved parameters of best YOLOv8 and best RT-DETR models represented in Lego_Results.xlsx (located under Results folder)

## Models
- Jupyter Notebook named "Fine-Tuning Detection Models" is used to fine-tune the YOLOv8 and RT-DETR and save the parameters
- data.yaml file is used in the training procedure of the detection models, which contains data path, augmentation types and other needy information
- Jupyter Notebook named "Fine-Tuned RTDETR + DeepSORT" is a combination of the Detection-Tracking pipeline. YOLOv8 can also be used instead of RT-DETR with some minor changes.

## Results
- The folder contains Lego_Results.xlsx which has all saved values during the execution of the codes
- There are also some figures underlining important points obtained from the experiments

