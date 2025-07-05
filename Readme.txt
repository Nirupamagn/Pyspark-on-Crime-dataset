Pyspark program on Crime dataset to cluster the crimes based on the crime category and resolution taken against the crime using K-Means algorithm,  Logistic Regression and  Naïve Bayes algorithm. 

PySpark 
Google Colab 
Install PySpark by running: `!pip install pyspark` 
from pyspark.sql import SparkSession 
#Upload Dataset 
uploaded = files.upload() 
for filename in uploaded.keys(): csv_file = filename  
spark=SparkSession.builder.appName("CrimeClassification").getOrCreate() 