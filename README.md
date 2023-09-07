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
![image](https://github.com/omriv88/Automatic-Image-Analysis2/assets/113102456/f753cdcc-556f-4cde-94f1-4015ecd7ee31)
![image](https://github.com/omriv88/Automatic-Image-Analysis2/assets/113102456/0aa65b94-859f-447a-b462-4896e190a886)
![image](https://github.com/omriv88/Automatic-Image-Analysis2/assets/113102456/f8eecdfb-9c2c-4468-aa41-0d5b936724a6)
