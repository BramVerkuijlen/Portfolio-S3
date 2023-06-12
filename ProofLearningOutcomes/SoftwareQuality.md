# Software quality

You use software tooling and methodology that continuously monitors and improves the software quality during software development.

In my project, I implemented various practices and tools to ensure software quality throughout the development process. 

## Version Control with Git
***
I utilized Git's branching feature to manage my codebase effectively. Each new feature or bug fix was developed in a separate branch, isolating the changes and minimizing the impact on the main branch. This approach allowed for better collaboration, version control, and stability.

## Continuous Integration (CI)
***
To automate the testing and integration process, I integrated Continuous Integration (CI) using GitHub Actions. 
By defining a set of automated tests and checks, I ensured that every commit to the development branch triggered the execution of these tests. 
For more information on CI and CD go [here](https://github.com/BramVerkuijlen/Portfolio-S3/blob/main/ProofLearningOutcomes/CI-CD.md)

## UI Testing
***
For front-end quality assurance, I implemented UI testing techniques. 
Snapshot tests were created to capture the expected appearance and behavior of different components in the user interface.
These tests enabled me to identify any unintended visual changes and ensure consistency in the UI across different environments and code changes.

![Snapshot test](https://github.com/BramVerkuijlen/Portfolio-S3/blob/main/ProofLearningOutcomes/Images/snapshot%20testing%20front-end.png)

*Snapshot test for my Category list component.*

## Functional Testing
***
To validate the functionality of the front-end, I designed and executed functional tests. 
One particular test involved entering a category into a field and verifying if the correct category bubble was displayed on the page after pressing a button.
This test ensured that user input was processed accurately and reflected appropriately in the UI, enhancing the overall quality and reliability of the front-end.

![functional test](https://github.com/BramVerkuijlen/Portfolio-S3/blob/main/ProofLearningOutcomes/Images/Functional%20test%20front%20end.png)

*This functional test fills in a input field and presses the add button, after that it looks if a "category bubble" appeared with the correct category*

## Unit testing
***
I implemented unit testing for my back-end application using Jest. I conducted tests for the twitchKeyVerifier module, mocking functions like fn (for file operations), Axios (for API calls), and Date.now (to remove time dependency). These tests ensured accurate and reliable results, catching bugs and regressions early in development. Unit testing plays a vital role in maintaining software quality, providing a safety net for code changes and increasing the overall reliability of the back-end application.

![Unit testing](https://github.com/BramVerkuijlen/Portfolio-S3/blob/main/ProofLearningOutcomes/Images/Unit%20test%20TwitchAccess%20token.png)

*This test looks if the SetAccessToken function sets a new access token, mocking the current token to be expired.*

## Integration Testing (Work in Progress)
***
While I have not yet completed the implementation of integration testing in the back-end, I am actively working on it using Jest and Supertest. However, I have encountered some difficulties related to mocking environmental variables used for communication with the IGDB API.

In my unit tests, I successfully mock the IGDB API using similar techniques. However, during the start of the program, I set the access key as an environmental variable to ensure that my wrapper functions correctly. This presents a challenge when it comes to integration testing because I need to find a way to mock or provide these environmental variables in the testing environment.

Despite the current obstacles, I am committed to implementing comprehensive integration testing to ensure the smooth and reliable functioning of the entire system. 
