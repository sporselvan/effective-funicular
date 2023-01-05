# REST API IN lambda (Node.js)
This project is a collection of code that demonstrates how to create a REST API using AWS Lambda. 

No need to use express in lambda.By using this project folder structure any one can start creating REST api in Lambda.

The code in this repository will show you how to create a Lambda function that can be triggered by an HTTP request and return a response to the client. You will learn how to define the API endpoints and the Lambda function logic, as well as how to deploy the API to AWS.

I hope this repository will be helpful to those who are new to building REST APIs with Lambda and are looking for a starting point. If you have any questions or suggestions, please don't hesitate to reach out. Thank you for visiting. 

# prerequisite

1. Lambda function that configured with aws API Gateway.

# Best practices.

1. Avoid file upload functionality in lambda. Because lambda payload,reponse size limit is 6 MB. Instead we can keep S3 file upload functions in ec-2  and use that s3 file keys for importing file inside lambda.

2. Avoiding N number of DB connections try to use pool connections like mysql2 library. It will cache the connections and reuse it for another db request.

3. Use Async - Await instead callback.  Since you are creating a new project most of the npm packages supports async await. Using callback inside async function will be mess.


