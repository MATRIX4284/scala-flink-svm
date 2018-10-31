
scala-flink-svm is application by which we are using file data source  of Flink to train a Support Vector Machine and give us some predictions.
I have used scala api of Flink to scrap the files to do the SVM training and prediction on a test file.


Download and extract the directory


1.Install Flink 1.6.0.

Go to flink_home/bin

and start flink by:

./start-cluster.sh


2.For building:
cd scala-flink-svnm

mvn clean package

The application jar named scala-flink-test-1.0.0-jar-with-dependencies.jar will be formed in the folder /target


3.run the application jar using:

flink run FQ./P/scala-flink-test-1.0.0-jar-with-dependencies.jar


There are two files are streaming input:

Training File:

svmguide1

Testing File:

svmguide1.t

the output will be under the folder liblu

