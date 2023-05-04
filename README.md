# -Trending Hashtags Generator for Instagram
Based on the content of the image, this AI tool determines which hashtags are currently popular and suitable. It produces the top ten trending hashtags that are pertinent to the subject matter of each image provided in the test case. 
#Getting Started
Google collab is sufficient to get started.
#Pre-requisites 
Packages that are required are :
•	numpy 
•	pandas 
•	matplotlib.pyplot 
•	matplotlib.image 
•	PIL.Image 
•	io
•	tensorflow 
•	tensorflow.keras.applications.MobileNetV2
•	pyspark.sql.SparkSession
•	pyspark.ml.evaluation.RegressionEvaluator
•	pyspark.ml.recommendation.ALS
•	pyspark.ml.recommendation.ALSModel
•	sklearn.model_selection.train_test_split
•	functools.reduce
•	os
•	tqdm
•	scipy.spatial.distance.cosine
•	selenium
•	time
•	re
•	json
•	random
•	Chrome and Firefox from selenium.webdriver
•	urlretrieve from urllib.request
•	By from selenium.webdriver.common.by
•	uuid4 from uuid
•	boto3
•	BytesIO from io
•	Image from PIL

#How It Works
The project involved scraping few Instagram images with some general hashtags like travel, fitness, etc., and storing the images in a folder named data and their details in a separate json file in a metadata folder. Hashtags from comments were also collected for modeling. Deep features were extracted from each image using MobileNetV2 and stored in a separate file. ALS model was applied to hashtag data to extract user and item features, and the dot product of each combination of features represented a recommendation score. The ALS model was stored in a separate file. The recommendation algorithm involved extracting deep features from a new image, finding the most similar images using cosine similarity, and using the ALS model to recommend hashtags with the highest dot product. The goal was to provide users with 10 accurate hashtag recommendations based on the content of their images.
