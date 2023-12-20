# Obituary Generator Project
## Project Overview
"The Last Show" is a full-stack application using React for the front-end and AWS services for the back-end. The application's purpose is to generate and display obituaries for fictional characters. AWS services like DynamoDB is used for the database and Lambda functions for back-end processing of creating and getting obituaries. The application generates obituaries using prompts from OpenAI's ChatGPT, converts them to speech using Amazon Polly, and stores the uploaded images on Cloudinary.

## Learning Outcomes
- Cloud Services Integration: Learn to integrate AWS services (Lambda, DynamoDB, Amazon Polly) and external APIs (ChatGPT, Cloudinary) in a single application.
- Serverless Architecture: Understand the principles of serverless computing and how to deploy serverless functions using AWS Lambda.
- Infrastructure as Code: Practice writing infrastructure as code using Terraform, allowing for automated and repeatable deployments.
- API Integration: Learn to interact with RESTful APIs, handling requests and responses, and understanding the importance of secure API key storage using the Parameter Store AWS service.
- Frontend Development: Enhance skills in React, state management, and connecting to a backend.
  
## How to deploy application
1. In the create-obituary and get-obituaries directories, ensure you install "pip install requests==2.28.2 -t ." and "pip install requests_toolbelt -t ." (This is the requests library that seemed to work and requests_toolbelt doesn't automatically come with it).
2. Retrieve your own ChatGPT and Cloudinary API keys and store them securely in the Parameter Store.
3. Create your own AWS IAM user access keys to use in the Terraform file.
4. In the infra directory, run "terraform init" and "terraform plan" and "terraform apply".
5. The create-obituary and get-obituaries URLs given need to be replaced in the src files.
6. In the base project directory, you can run "npm start". (Make sure you do npm install and npm run build first).