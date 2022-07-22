# Lambda-Function

Lambda function to sort the objects uploaded to main bucket into different buckets according to formats. Added CloudWatch and SNS functionality.

(Amazon S3, Lambda, CloudWatch, SNS, python)

Prerequisites:

1. Create a role with AWS S3 full access and AWS CloudWatch full access.

2. Create 4 buckets 

   • Main bucket where objects are uploaded

   • Txt, pdf, img bucket to store the objects after sorting accordingly.

Steps:

1. Create a lambda function. Remember to give the same name as main s3 bucket created
since the code takes the bucket name from the lambda function itself.

2. Add a trigger as S3 bucket by selecting the main bucket.

3. Add Destination as SNS topic

4. Add the code and deploy.

5. Now whenever there is an object uploaded into main bucket, it will be moved to another 
bucket according to the format.
