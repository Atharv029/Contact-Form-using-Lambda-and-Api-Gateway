# Serverless CORS Handling with AWS Lambda and Database Integration

## Overview

This project demonstrates how to set up a **serverless backend** using **AWS Lambda**, **API Gateway**, and a **database** to bypass CORS (Cross-Origin Resource Sharing) issues and store data, allowing seamless interaction between frontend and backend.

### Key Features:
- **AWS Lambda** function to process requests.
- **API Gateway** to expose the Lambda function as a RESTful API.
- **CORS** headers configured within the Lambda function to allow cross-origin requests.
- **Database Integration**: Data is stored in a database, ensuring persistence across multiple requests.
- A simple HTML frontend to interact with the serverless backend.

### Problem:
Handling CORS issues is a common challenge when making requests to APIs hosted on different domains. This project showcases a solution using serverless technologies to eliminate the need for complex server management, solve CORS problems, and store data in a database for persistence.

### How It Works:
1. **Frontend (HTML/JavaScript)**:
   - An HTML page with a button that triggers a fetch request to the API.
   - The fetch call interacts with the API Gateway, which triggers the AWS Lambda function and stores data in the database.

2. **Backend (AWS Lambda + API Gateway + Database)**:
   - **AWS Lambda** processes the incoming request, performs necessary logic, and interacts with the database to store or retrieve data.
   - **CORS headers** are added to the Lambda function response, allowing cross-origin requests.
   - **API Gateway** serves as the endpoint that triggers the Lambda function, making the entire process serverless.
   - The Lambda function is connected to a **database** where data is stored and fetched as needed.

### Steps to Deploy:
1. Deploy the AWS Lambda function with the provided code.
2. Set up an API Gateway with CORS enabled to trigger the Lambda function.
3. Configure the Lambda function to interact with your database (e.g., DynamoDB, RDS).
4. Update the API URL in the HTML frontend to point to your API Gateway endpoint.
5. Test the integration by opening the HTML file in a browser and clicking the "Fetch Data" button.

### Technologies Used:
- AWS Lambda (Node.js)
- AWS API Gateway
- CORS
- Database Integration (e.g., DynamoDB)
- HTML, JavaScript (Frontend)

---

Want to see the project in action?  
📽️ **[Watch the full demo on LinkedIn](https://www.linkedin.com/posts/atharv-chawan-ab01152a7_building-serverless-solutions-with-aws-lambda-activity-7319684248548876288-N30y?utm_source=social_share_send&utm_medium=member_desktop_web&rcm=ACoAAEngtOQBeA6BfWpcxn-tiF0263Jpx1sqK6I)**  

I walk through how I used:
- AWS Lambda + API Gateway
- CORS handling
- Database integration
- Frontend interaction with serverless backend
