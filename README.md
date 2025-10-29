#Title
Dockerize a React Application with Multi-Stage Build

#Objective
Learn how to create a production-ready Docker image for a React application using a multi-stage Docker build. This helps you reduce image size, separate build dependencies from runtime, and prepare your app for deployment.

#Task Description
Build a simple React application (for example, created using Create React App). Write a multi-stage Dockerfile:

Use a Node.js image as the first stage to install dependencies and build the React app.
Use an Nginx image as the second stage to serve the compiled static files.
Add a .dockerignore file to exclude unnecessary files. Build the Docker image locally and run it to test if the React app is correctly served on localhost. Verify that the final image size is smaller than including all dev dependencies.

#Title
Set Up CI/CD Pipeline using GitHub Actions

#Objective
Understand how to automate testing and deployment using GitHub Actions. Learn to trigger workflows on code pushes, run tests automatically, and deploy artifacts to your hosting environment.

#Task Description
Create a .github/workflows/main.yml file in your repository. Configure it to:

Trigger on every push to the main branch.
Set up Node.js in the runner environment.
Install dependencies and run tests (e.g., npm test).
Build the project (e.g., npm run build).
Optionally, configure the workflow to deploy the build artifacts to a platform like GitHub Pages, Netlify, or S3 using appropriate actions. Commit and push changes to test if the workflow runs as expected.

#Title
Deploy Full Stack App on AWS with Load Balancing

#Objective
Gain experience deploying a full stack application to AWS and configure load balancing for scalability and high availability. Learn about EC2, Elastic Load Balancing (ELB), and VPC basics.

#Task Description
Build a simple full stack app (React frontend + Node.js/Express backend + optional database like MongoDB). Deploy backend and frontend separately to EC2 instances. Set up an Application Load Balancer (ALB) in AWS to distribute traffic between multiple backend EC2 instances. Configure security groups, VPC settings, and domain routing (via Route 53, if desired). Test your deployment by accessing the app from a browser, and ensure the load balancer handles traffic as expected.