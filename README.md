# Basic CICD using Github Actions and Docker 
This project is a basic CI/CD setup for a Python web app that displays "Hello World" on a webpage. 
The project uses GitHub Actions to automate testing, building, and deployment.
## Key Features
### App Structure: 
app.py serves "Hello World," and test.py verifies the output. If the test fails (message isn't "Hello World"), the CI pipeline flags an error.
### CI/CD Pipeline: 
Defined in .github/workflows/main.yml with two jobs:
### Build Job: 
Builds a Docker image of the app.
### Test Job: 
Runs test.py to ensure the message is correct.
### Deployment: 
On successful build and test, the Docker image is pushed to Docker Hub.
### Notifications: 
Email notifications are sent for successful builds or errors.
Once you pull the image and run it locally, it launches a webpage showing the output "Hello World." This project demonstrates a basic CI/CD setup with GitHub Actions, Docker, and AWS for deployment.
