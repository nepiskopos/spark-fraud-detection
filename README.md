# Simple Machine Learning for Fraud Detection
Fraudulent job advertising analysis and detection using Spark, PySpark and Python Machine Learning.

For all the experiments, we used the [[Real or Fake] : Fake Job Description Prediction](https://www.kaggle.com/shivamb/real-or-fake-fake-jobposting-prediction) dataset.

## Part 1: Simple statistics and knowledge extraction using Spark / Scala

### Software setup instructions

1. Choose the desired version of Apache Spark from [here](https://spark.apache.org/downloads.html)
    For this experimentation we used Spark v2.4.5 pre-built for Apache Hadoop 2.7
    **Note:** This Spark version is only compatible with Java version 8
2. Download the chosen Apache Spark version and extract it to home directory
    ```console
    wget https://archive.apache.org/dist/spark/spark-2.4.5/spark-2.4.5-bin-hadoop2.7.tgz
    tar -xzvf ./spark-2.4.5-bin-hadoop2.7.tgz -C ~/
    ```
3. Add Apache Spark's binaries to PATH
    ```console
    echo 'export SPARK_HOME=~/spark-2.4.5-bin-hadoop2.7' >> ~/.bashrc
    echo 'export PATH=$SPARK_HOME/bin:$PATH' >> ~/.bashrc
    source ~/.bashrc
    ```
4. Install the compatible Java Runtime and verify installation (instructions for Ubuntu)
    ```console
    sudo apt-get install -y openjdk-8-jre
    which java
    ```
5. Test the proper execution of Spark shell
    ```console
    spark-shell
    ```
