## LEAP is a web-based, open-source environment that allows pre-built prototypes to be launched instantly and modified within only 7 steps. It is designed for seamless integration with existing AWS accounts, requiring no modifications to the current AWS user interface. This approach ensures rapid deployment and maintains the security integrity of the user's AWS environment.

The environment is setup with the following these steps: 1/ User watches a short video that describes the simple setup process and basic info on CloudFormation and Amazon Bedrock model access, 2/ User requests and is granted access to an AI Model, 3/ User uploads the setup CloudFormation script which installs the web app and sets up all the necessary roles and permissions, 4/ User clicks on the URL for the web app to open it in their browser and chooses from pre-loaded prototypes, 5/ The CloudFormation stack is deployed on the backend and returns the new resources, 6/ Links to the assets are shown clearly to the user (frontend URL, API endpoint, link to Lambda function, etc.), 7/ A brief description about the generated resources and how they interact along with clickable links to 30 second videos that explain concepts (i.e. Prompt Engineering) and services (i.e. API Gateway) which creates a personalized learning path on the right side column. (See Appendix A for UI sample)

![image](https://github.com/user-attachments/assets/ed224afb-7407-4079-9df6-457a2969d31e)

### Main Features:
1.	Dynamic loading of custom-built prototypes from a GitHub repository
2.	One-click prototype deployment system for Generative AI applications
3.	Web-based interface hosted on S3 with a modern, responsive design
4.	Real-time deployment status monitoring, progress tracking and removal with cleanup
5.	Interactive architecture visualization for deployed prototypes
6.	Direct links to AWS console for deployed services (S3, Lambda, API Gateway)
7.	Cost tracking and estimation for deployed prototypes
8.	Integrated explainer system with video tutorials and documentation
9.	Persistent state management using local storage
10.	CORS-enabled API endpoints for secure cross-origin requests
    

The following initial custom prototypes for idea validation and MVPs will be included in the first version (to be released following AppSec review on November 15th)
: 1/ A full-stack serverless Generative AI chatbot app with a Rest API endpoint, 2/ A ‘chat with your documents’ Knowledge Base web app using Cognito to secure endpoints, 3/ A landing page that collects signups for preview access with a Gen AI prompt-flow backend plus basic analytics, 4/ a ‘wizard of oz’ prototype that analyzes uploaded documents with Gen AI using an Agent on Bedrock and returns an analysis. The second version of the environment includes the ability to customize the frontend using natural language for more flexibility in generating customized frontends plus the ability to continue development locally using SAM and AWS CDK.
