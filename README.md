# Automatic-Image-Analysis2
Create Automation process for Image rekognition analysis using Amazon Rekognition machine learning. Once a client upload an image to S3 Bucket this will trigger a Lambda function that will perform image analysis in AWS Rekognition and save the results into Amazon DynamoDB database

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




