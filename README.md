# Datalabs Datascience remote.sh

A script to make managing EC2 instances easier.

## Env Variables

The following ENV vars must be set in your local env for this script to run correctly:

|ENV VAR|explanataion|Nominal value|
|---|---|---|
|INSTANCE_NAME|Name of the instance you wish to communicate with|datascience_base|
|REMOTE_DATALABS_PATH|Path to the the datalabs folder on the remote instance|/data/datalabs|
|LOCAL_DATALABS_PATH|Path to the datalabs folder on your local machine|/home/matthew/Documents/wellcome/datalabs|
|AWS_ACCESS_KEY_ID|AWS credentials||
|AWS_SECRET_ACCESS_KEY|AWS credentials||


