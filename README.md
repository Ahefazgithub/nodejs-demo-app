In this project, I set up a CI/CD pipeline using GitHub Actions to automate the process of building, testing, and deploying a Node.js web app. The goal was to create an automated workflow that builds the app, runs tests, and pushes the app to DockerHub whenever changes are made in the repository.

Here’s a breakdown of the steps I followed:
1. Set Up GitHub Repository and Project

    Created a GitHub repository to store the Node.js web application.

    The application was a simple Node.js app that serves as a sample for testing the pipeline.

2. Configured GitHub Actions Workflow

    Created the CI/CD pipeline configuration file (main.yml) under .github/workflows/ in the repository.

    The pipeline was designed to:

        Build: Install dependencies and prepare the Node.js application.

        Test: Run tests (e.g., using a testing framework like Mocha or Jest).

        Build Docker Image: Dockerized the Node.js app and built an image.

        Push to DockerHub: Pushed the Docker image to DockerHub after a successful build.

3. Trigger Pipeline on Push to main Branch

    The pipeline was set up to trigger automatically on a push to the main branch.

    This ensures that every time new code is pushed, the pipeline runs and deploys the latest version of the app.

4. GitHub Actions Jobs and Steps

    Defined the pipeline steps in the main.yml file:

        Build: Installs dependencies using npm install.

        Test: Runs tests using the Node.js test suite.

        Docker Build & Push: Builds the Docker image and pushes it to DockerHub using the docker CLI.

5. Testing the Pipeline

    After setting up the GitHub Actions workflow, I tested the pipeline by making changes to the Node.js application and pushing them to the main branch.

    Verified that the pipeline triggered successfully, the app was built and tested, and the Docker image was pushed to DockerHub.

6. Pushed All Project Files to GitHub

    After completing the project, I pushed all the project files (Node.js app and GitHub Actions workflow configuration) to my existing GitHub repository:
    ➡️ elevatelabs_task1
