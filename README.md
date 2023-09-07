# Automatic-Image-Analyze
Create Automation process for Image rekognition Analyze using Amazon Rekognition machine learning. Once a client upload an image to S3 Bucket this will trigger a Lambda function that will perform image analysis in AWS Rekognition and save the results into Amazon DynamoDB database

![image](https://github.com/omriv88/Automatic-Image-Analysis2/assets/113102456/cb6b3487-b9ad-403a-9337-289c0ffca45c)

#cloudshell:

* ~]$ sudo npm install -g aws-cdk-lib
![image](https://github.com/omriv88/Automatic-Image-Analysis2/assets/113102456/a281ce40-adea-4d53-9f55-ff15a3172008)
* ~]$ mkdir cdk-app
* ~]$ cd cdk-app/
* cdk-app]$ cdk init app --language javascript
* cdk-app]$ cd lib/
* lib]$ rm cdk-app-stack.js
* lib]$ touch cdk-app-stack.js
* copy the cdk-app-stack.js file into your lib/ directory
* cdk-app-stack.js:
![image](https://github.com/omriv88/Automatic-Image-Analysis2/assets/113102456/bf5932c9-9a28-4712-b945-6d9475a5c42b)
![image](https://github.com/omriv88/Automatic-Image-Analysis2/assets/113102456/9e741298-1d98-4b85-91eb-e9c88c5d1afb)
![image](https://github.com/omriv88/Automatic-Image-Analysis2/assets/113102456/81a2b6ea-f65b-4cf9-b8be-6e16c9893d54)
* lib]$ cd ..
* cdk-app]$ mkdir lambda && cd lambda
* lambda]$ touch index.py
* copy the index.py into your lib/ directory
* index.py:
![image](https://github.com/omriv88/Automatic-Image-Analysis2/assets/113102456/498fe7c2-9c76-42d1-abd9-9c689ad3c254)
![image](https://github.com/omriv88/Automatic-Image-Analysis2/assets/113102456/51a5b07d-daa2-49fc-9f14-9cbfecf93fc0)
* lambda]$ cd ..
* cdk-app]$ cdk bootstrap
* under CloudFormation -> Stacks -> CDKToolkit -> Resources (all the resource has been deployed)
![image](https://github.com/omriv88/Automatic-Image-Analysis2/assets/113102456/2f7934ea-00b4-4c60-882f-902a014b764c)
![image](https://github.com/omriv88/Automatic-Image-Analysis2/assets/113102456/0c1426f8-d3c5-4c65-a68f-6f68c27f517c)
* cdk-app]$ cdk synth (Get a whole CloudFormation template) 
* cdk-app]$ cdk deploy
* Upload the Image : CloudFormation -> Stacks -> CdkAppStack -> Resources -> click on S3 Bucket and upload a image 
![image](https://github.com/omriv88/Automatic-Image-Analysis2/assets/113102456/8071bbef-4899-43f8-a657-b078bd32093c)
![image](https://github.com/omriv88/Automatic-Image-Analysis2/assets/113102456/e069b0cc-1fcd-4c90-b9a6-f80249836589)
* image analysis resultes: -> CloudFormation -> Stacks -> CdkAppStack -> Resources -> DynamoDB -> Click  "Explore table items" 
![image](https://github.com/omriv88/Automatic-Image-Analysis2/assets/113102456/cda277bd-8666-4ee6-bd6f-a409cae235bc)
![image](https://github.com/omriv88/Automatic-Image-Analysis2/assets/113102456/793421b5-3ccf-4eb8-badf-69e6ea52f924)
* Upload more two images -> Goto S3 Bucket -> Upload 
![image](https://github.com/omriv88/Automatic-Image-Analysis2/assets/113102456/916deced-a51c-4ebf-b62f-27fa21a131f2)
* the tresultes in DynamoDB:
![image](https://github.com/omriv88/Automatic-Image-Analysis2/assets/113102456/73de41eb-dd1f-419e-8218-8c697a4336fe)
* For CleanUp
empty the s3 bucket and destroy the stack


