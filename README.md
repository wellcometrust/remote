# Datalabs Datascience remote.sh

A script to make managing EC2 instances easier.

```
remote help

 ⚡ AWS EC2 instance remote control ⚡

 ⚠️  You must set the following ENV VARS:
 INSTANCE_NAME            - The name of the instance (e.g. datascience_base)
 PREFIX                   - The prefix used to identify instances
                            of interest (e.g. datascience)
 REMOTE_PATH              - Path to remote working repo
 LOCAL_PATH               - Path to local working repo
 AWS_ACCESS_KEY_ID        - AWS access key ID
 AWS_SECRET_ACCESS_KEY_ID - AWS secret key

 ⚠️  All commands will filter terminated instances by default

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
 list    - Lists all the ec2 instances whose name has a prefix
           described by PREFIX.
 type    - Changes the instance type to that specified as an
           argument \(e.g. t2.small\), otherwise returns the
           instance type
 stop    - Stops the instance
```

## Env Variables

The following ENV vars must be set in your local env for this script to run correctly:

|ENV VAR|explanataion|Nominal value|
|---|---|---|
|INSTANCE_NAME|Name of the instance you wish to communicate with. Note that this requires that the tag `Name` is set on the instance of interest|datascience_base|
|PREFIX|Prefix used to identify instances for a given task|datascience|
|REMOTE_PATH|Path to remote working repository|/data/datalabs|
|LOCAL_PATH|Path to local working repository|~/datalabs|
|AWS_ACCESS_KEY_ID|AWS credentials||
|AWS_SECRET_ACCESS_KEY|AWS credentials||


