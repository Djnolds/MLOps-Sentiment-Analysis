# MLOps-Sentiment-Analysis


# For Dagshub:

MLFLOW_TRACKING_URI=https://dagshub.com/ayorey/MLflow-Basic-Demo.mlflow
MLFLOW_TRACKING_USERNAME=Djnold

python script.py

export MLFLOW_TRACKING_URI=https://dagshub.com/ayoreynolds/MLflow-Basic-Demo.mlflow

export MLFLOW_TRACKING_USERNAME=Djnold


## DVC

dvc init

dvc repro

dvc dag


## MLflow on AWS

## MLflow on AWS Setup:
<!-- Login to AWS console.
Create IAM user with AdministratorAccess
Export the credentials in your AWS CLI by running "aws configure"
Create a s3 bucket
Create EC2 machine (Ubuntu) & add Security groups 5000 port
Login to AWS console.
Create IAM user with AdministratorAccess
Export the credentials in your AWS CLI by running "aws configure"
Create a s3 bucket
Create EC2 machine (Ubuntu) & add Security groups 5000 port

sudo apt update

sudo apt install python3-pip

sudo apt install pipenv

sudo apt install virtualenv

mkdir mlflow

cd mlflow

pipenv install mlflow

pipenv install awscli

pipenv install boto3

pipenv shell -->


## Then set aws credentials
aws configure


#Finally 
mlflow server -h 0.0.0.0 --default-artifact-root s3://mlflow-test-23

#open Public IPv4 DNS to the port 5000


#set uri in your local terminal and in your code 
export MLFLOW_TRACKING_URI=https://dagshub.com/ayoreynolds/MLflow-Basic-Demo.mlflow