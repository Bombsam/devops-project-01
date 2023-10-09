# My DevOps App

This repository contains a simple Node.js application, demonstrating the use of GitHub Actions for Continuous Integration (CI) and Continuous Deployment (CD) to Heroku.

## Application Overview

The application is a basic Express.js server that serves a static message to users. It's a starting point to showcase the DevOps capabilities rather than the functionality of the app itself.

### Running Locally

To run the application on your local machine:

1. Clone the repository:
    git clone https://github.com/Bombsam/devops-project-01.git

2. Navigate to the project directory:
    cd devops-project-01

3. Install the required packages:
    npm install

4. Start the server:
    node index.js

5. Open your browser and navigate to `http://localhost:3000/`. You should see "Hello, DevOps!".

## CI/CD Overview

This project utilizes GitHub Actions for both CI and CD:

- **Continuous Integration**: On every push to the `main` branch, the workflow installs the necessary dependencies and runs any tests (if available).

- **Continuous Deployment**: If the CI process succeeds and the push is on the `main` branch, the application is automatically deployed to Heroku.

### Heroku Deployment Details

The deployment is handled by the GitHub Actions workflow. It uses the Heroku API key and app name, stored as secrets within the GitHub repository, to push the changes to the corresponding Heroku app.

## Contribute

Contributions are always welcome! Please ensure that you update tests as appropriate and that the CI/CD pipeline passes for your changes.