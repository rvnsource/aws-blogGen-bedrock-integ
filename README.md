- Postman-APIGW-Lambda-Bedrock-Integration
- Copy code in lambaFuncCode.py into lambda function 
  -  Add boto3 latest (via Add layer) to lambda function:
     install necessary python pkgs in python named folder,
     zip that folder and upload to lambda function to Add layer)
  -  Add admin role permission to lambda function to access bedrock
  -  in lambda configuration timeout to atleast 1 min. (otherwise Internel server error)
  -  I used "meta.llama3-70b-instruct-v1:0", which I had Model access in aws bedrock
  -  finally, don't forget to save and deploy the lambda function
- Create API Gateway with http POST method
  - use 'dev' stage. 
- Post man Post http request to API Gateway endpoint 
  
ref. Generative-AI-With-Cloud repo.


