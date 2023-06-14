
# CI/CD
***

*You design and implement a (semi)automated software release process that matches the needs of the project context.

## What is CI/CD
***

CI/CD is a software development approach that enables teams to streamline their delivery processes by combining continuous integration (CI) and continuous delivery (CD) or continuous deployment.

<img src="https://github.com/BramVerkuijlen/Portfolio-S3/assets/95694367/c640e81c-5fcf-4f04-92fd-deff7d3e0f1b" alt="CI CD image" width="600">

## CI
***
I've implemented Continuous Integration (CI) in my development workflow to ensure smooth code integration and reliable software delivery. To achieve this, I utilize separate repositories and maintain a dedicated development branch. This allows me to work on new features and bug fixes without directly impacting the main branch.

To further ensure the correctness of my code, I've incorporated automatic tests specifically for the development branch. These tests are designed to validate the functionality and integrity of my code changes before merging them into the main branch. By running these automated tests on the development branch, I can catch any potential issues early on and address them promptly.

In addition, I've configured a GitHub action that automates the build and test processes for both the development branch and the main branch. This ensures that my code is thoroughly tested and functional, providing an added layer of confidence before merging it into the main branch.

While implementing Continuous Integration (CI) in my development workflow, I encountered some challenges specifically related to my API. When executing the CI action to run the build process, GitHub faced difficulty recognizing the existence of my API build. As a result, the API build process kept running indefinitely without completion.
I have been investigating the cause of this issue and exploring potential solutions to ensure the seamless integration of my API build within the CI pipeline. 

[**Example CI Workflow**](https://github.com/Phantom-works/Adviser-Front-End/actions)



## CD
***

By setting up an automated workflow, I've successfully achieved Continuous Deployment (CD) in my project. Initially, I had configured the CD workflow to run on a fixed schedule every Tuesday at 2am. However, I later made the decision to enhance the workflow by triggering deployments on every push request to the main branch. This change allows for more immediate and responsive deployment of code changes.

With the updated CD workflow, whenever a push request is made to the main branch, the workflow automatically builds and deploys the latest version of the code as a Docker image to Docker Hub. This ensures that any updates or new features are promptly deployed and made available to users.


[**Example CD Workflow**](https://github.com/Phantom-works/Adviser-Front-End/actions)
