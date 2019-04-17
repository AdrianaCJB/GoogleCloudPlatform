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

Go to Navigation menu > Storage > Browser and then click Create bucket.
- Give your bucket a universally unique name, then **click Create.**

### 3. Setting Airflow variables

Go to Airflow UI using the GCP Console:

1. Go back to the Environments page.
2. In the Airflow webserver column for the environment, click the new window icon.
3. Click on your credentials.
4. The Airflow web UI opens in a new browser window.
5. Select Admin > Variables from the Airflow menu bar, then Create
6. In this step you'll set the following three Airflow variables typically used by DAGs: **gcp_project, gcs_bucket, and gce_zone**.

### 4. Copying the DAG to Cloud Storage

Save **quickstart.py** file on your local virtual machine:
