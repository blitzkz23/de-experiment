# How to run:

## Amazon related setup:
```bash
1. Create EC2 instance, and generate key-pair.pem to access ec2 later

2. SSH on terminal by using provided command such as: 
ssh -i "ec2_airflow_key.pem" ubuntu@ec2-108-136-142-26.ap-southeast-3.compute.amazonaws.com

3. Install requirements rom requirement-ec2.txt manually on the instance

4. Run standalone airflow server:
airflow standalone

5. When airflow is ready, copy the admin and password (because one time only)

6. Open the instance public ipv4:8080 to access airflow UI, such as:
ec2-108-136-142-26.ap-southeast-3.compute.amazonaws.com:8080

7. If you cant see the UI, after doing above step, go to the security group > edit inbound rules > add rule > allow all trafic > change source to MyIp / Anywhere

```

## Run Program:
```bash
# Create venv
python -m venv env

# Activate venv
source env/bin/activate

# How to write requirements automatically (dont run this, just for my docs)
pipreqs /path/to/project

# Install requirements
pip install -r requirements.txt

```
