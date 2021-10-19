# serverless-datapipeline-humorreview
_**No EC2 instance or Cloud9**_
## Overview
![image](https://user-images.githubusercontent.com/39500675/137433077-508dd37d-e140-4bf4-8ffc-427dd02b73ad.png)

## Test Data preparation
- download data here https://humor-detection-pds.s3-us-west-2.amazonaws.com/Humorous.csv and here https://humor-detection-pds.s3-us-west-2.amazonaws.com/Humorous.csv
- product: Oujia 
- make a shorter test dataset: top 2-3 from both
- don't make S3 bucket, don't upload your file
- add test data line by line to DynamoDB
- create a table in DynamoDB
## Create queue in SQS
## Create lambda functions
### Create loadreview
### Create analyzereview
### Use Lambda layer to import library
- Add layer by specifiying arn: https://melissa-bain.medium.com/how-to-import-python-packages-in-aws-lambda-pandas-scipy-numpy-bb2c98c974e9
- I used: ```arn:aws:lambda:us-east-1:113088814899:layer:Klayers-python37-pandas:1```
