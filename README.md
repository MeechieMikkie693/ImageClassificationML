Problem Statement: To develop an automated image classification model using machine learning techniques that can accurately classify unencountered new images into predefined categories, based on their Visual features.

This study focuses on the image classification technique using supervised machine learning, specifically the Support Vector Learning (SVL) model, to develop an efficient method for classifying images by collecting data using Python's Bing downloader package. The process involves several steps, including data collection, preprocessing, feature extraction, model training, and evaluation.  The collected dataset are then pre-processed using the skimage library in Python, which includes resizing, normalization, flattening of the images(converting into a suitable format for the ML algorithm) and noise reduction(for audio/video dataset, specifically). Labelling being an important step in supervised learning, where each image is assigned a corresponding class label. Once the images are labelled, relevant feature extraction techniques are applied to extract essential information from the images. The Support Vector Learning (SVL) model is then trained using the labelled and pre-processed images. The model learns to classify images based on the extracted features and their corresponding labels. MATLAB’s plot() function is used for dataset visualization. The model is later tested and trained using 20 by 80 ratio of the dataset, and the accuracy is determined using the confusion matrix and sci-kit learn library of Python.

Methodology involved:
1.	Gathering of the data: using Bing-Image-downloader Python Library to scrape the images from the web.
2.	Create a separate directory and a subdirectory to store the image dataset of different classes/categories.
3.	Image preprocessing:
 •	A path is created which helps in accessing every image using the os.path.join() function of the OS library.
 •	Resizing and normalizing the pixel values(from 0 to 1) is done using the Python’s skimage library.
 •	Flattening and storing of the image vectors is again done using the Python’s skimage and Numpy library.

4.	Data set graph: A graph of different categories against number of image set in each category is plotted using the matplotlib.pyplot library.
5.	Train test split from model selection of sklearn ml model: The sci-kit learn library of Python is used to split the data into training and testing.
6.	Training the ML model based on the supervised pre-processed data set: The SVM(Support Vector Machine) classification algorithm(based on supervised learning method, labelled data) is trained and the required parameters(C, Kernel, gamma etc.) are set as apt.
7.	Checking the accuracy of the ML model: The model is evaluated using accuracy score and confusion matrix of sklearn.metrics library of Python.
8.	Save the model: The model is saved using Pickle Library.
9.	Testing the model: The model is tested using a new image(not the one from the test/train dataset) and necessary changes are made again based on the predicted output and the actual output ratio.
