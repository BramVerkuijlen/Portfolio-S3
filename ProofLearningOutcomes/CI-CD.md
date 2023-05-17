
# CI/CD
***

*You design and implement a (semi)automated software release process that matches the needs of the project context.

## What is CI/CD
***

CI/CD is a software development approach that enables teams to streamline their delivery processes by combining continuous integration (CI) and continuous delivery (CD) or continuous deployment.

<img src="https://github.com/BramVerkuijlen/Portfolio-S3/assets/95694367/c640e81c-5fcf-4f04-92fd-deff7d3e0f1b" alt="CI CD image" width="600">


## Proof Learning outcome
***

### CI
***
I've implemented Continuous Integration (CI) in my development workflow to ensure smooth code integration and reliable software delivery. To achieve this, I utilize separate repositories and maintain a dedicated development branch. This allows me to work on new features and bug fixes without directly impacting the main branch.

To further ensure the correctness of my code, I've incorporated automatic tests specifically for the development branch. These tests are designed to validate the functionality and integrity of my code changes before merging them into the main branch. By running these automated tests on the development branch, I can catch any potential issues early on and address them promptly.

In addition, I've configured a GitHub action that automates the build and test processes for both the development branch and the main branch. This ensures that my code is thoroughly tested and functional, providing an added layer of confidence before merging it into the main branch.

[**Example CI Workflow**](https://github.com/Phantom-works/Adviser-Front-End/actions)

### CD
***

By setting up an automated workflow, I've successfully achieved Continuous Deployment (CD) in my project. This workflow specifically focuses on deploying the main branch of my code as a Docker image to Docker Hub. What sets it apart is the scheduling aspect: the CD workflow is configured to run like clockwork every Tuesday at 2am. This regular and predictable release schedule offers numerous benefits.

The implementation of CD with a scheduled deployment brings about a consistent cadence of releases. This regularity facilitates better planning and communication of updates to my users, keeping them informed and engaged. Moreover, the automated nature of the deployment workflow significantly reduces the need for manual intervention, mitigating the risk of human errors. As a result, I have more time available to dedicate to other essential tasks.

[**Example CI Workflow**](https://github.com/Phantom-works/Adviser-Front-End/actions)
