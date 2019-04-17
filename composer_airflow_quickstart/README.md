# Cloud Composer and Airflow Quickstart

Create and run an Apache Airflow workflow in Cloud Composer that completes the following tasks:

1. Create a Cloud Dataproc cluster.
2. Run an Apache Hadoop wordcount job on the cluster and output the results to Cloud Storage.
3. Delete the cluster.


## Setup
### 1. Create Cloud Composer environment:

Go to Navigation menu > Composer:
- Name: highcpu
- Location: us-central1
- Zone suffix: a
- Machine type: n1-highcpu-4 and **Click Create.**

### 2. Create a Cloud Storage bucket

Go to Navigation menu > Storage >Browser and then click Create bucket.
- Give your bucket a universally unique name, then **click Create.**


