# Datalabs Datascience remote.sh

A script to make managing EC2 instances easier.

```
remote help

 ⚡ Datalabs DataScience EC2 remote control ⚡

 ⚠️  You must set the following ENV VARS:
 INSTANCE_NAME            - The name of the instance \(e.g. datascience_base\)
 REMOTE_DATALABS_PATH     - Path to the datalabs folder on the remote instance
 LOCAL_DATALABS_PATH      - Path to the datalabs repo on the local machine
 AWS_ACCESS_KEY_ID        - AWS access key
 AWS_SECRET_ACCESS_KEY_ID - AWS secret key

 💪 Available commands:

 start   - Starts the instance
 git     - Sets up a remote in your local datalabs repo that 
           points to the remote repo on the instance. This 
           allows you to push code directly to your instance 
           from your local datalabs folder with git push ec2
 connect - Tries to connect to the instance
 id      - Returns the instance id e.g. i-ae23f836a5f3de
 ip      - Returns the instance public address ec2-x-x-x-x...amazonaws.com
 status  - Returns the status of the instance
 list    - Lists all the datalabs datascience instances
 type    - Changes the instance type to that specified as an
           argument \(e.g. t2.small\), otherwise returns the
           instance type
 stop    - Stops the instance

```

## Env Variables

The following ENV vars must be set in your local env for this script to run correctly:

|ENV VAR|explanataion|Nominal value|
|---|---|---|
|INSTANCE_NAME|Name of the instance you wish to communicate with|datascience_base|
|REMOTE_DATALABS_PATH|Path to the the datalabs folder on the remote instance|/data/datalabs|
|LOCAL_DATALABS_PATH|Path to the datalabs folder on your local machine|/home/matthew/Documents/wellcome/datalabs|
|AWS_ACCESS_KEY_ID|AWS credentials||
|AWS_SECRET_ACCESS_KEY|AWS credentials||


