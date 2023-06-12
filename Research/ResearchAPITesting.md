# How can I effectively test my Api and what tools should I use?

**By: Bram Verkuijlen**

**Date: 8-6-2023**
***

![image](https://github.com/BramVerkuijlen/Portfolio-S3/assets/95694367/858033c8-96f4-45bd-80ac-91e3f3ce8f4e)

*AI art made by [hotpot.ai](https://hotpot.ai/art-generator?s=dalle-mini)*

## Introduction
***

As the demand for efficient and reliable APIs grows in the software development landscape, thorough testing becomes essential.
But how can we effectively test a microservice and select the right tools? 
This research aims to explore the most effective strategies and tools for testing my microservice.

## What does my API do?
***
My API is designed to provide a convenient and user-friendly way to search for games based on specific categories. By using the IGDB (Internet Game Database) API, you can request games belonging to various genres, platforms, or themes. The API acts as an intermediary, interacting with the IGDB API to retrieve relevant game data. Additionally the microservice retrieves the necessary access key and stores it in a JSON format. This allows for seamless and efficient communication between the microservice and the IGDB API.

## Different ways to test an API
***
When it comes to testing an API, there are several approaches available, but not all of them may be applicable or necessary for every project.
For my API I will explore three commen testing methodologies: unit testing, integration testing, and end-to-end testing.

+ #### Unit testing
Unit testing is an essential practice in software development, where developers write code specifically designed to test individual functions or units of an application.
Unit testing can be performed manually or, more commonly, automated using a UnitTest framework. In the automated approach, developers write test code within the application, which can later be removed or commented out before deployment. [[1]](https://www.guru99.com/unit-testing-guide.html)

+ #### Intergration testing
Integration testing, also known as integration and testing (I&T), is a crucial phase in software testing where different modules or components of an application are tested as a combined entity. This testing approach focuses on verifying the interaction and interfaces between these modules, ensuring they work seamlessly when integrated. Integration testing involves combining the modules and evaluating their behavior as a cohesive unit. Integration testing helps identify errors in module integration, handle changing requirements, address common issues missed during unit testing, and ensure the smooth functioning of the entire application. [[2]](https://www.techtarget.com/searchsoftwarequality/definition/integration-testing)

+ #### End to end testing

End-to-end testing is a vital component of the software development lifecycle that aims to validate the functionality and performance of an application in real-life scenarios. It involves testing the entire application from start to finish, simulating user interactions and replicating live settings to ensure that all sub-systems, including UI and API layers, external databases, networks, and third-party integrations, work harmoniously. The complexity of modern software applications necessitates thorough end-to-end testing to identify any failures or instabilities that could impact the overall product. [[3]](https://smartbear.com/learn/automated-testing/what-is-end-to-end-testing/)

## A good unit test

There are a couple characteristics of a good unit test:

   + Fast Execution: Unit tests should execute quickly, ideally taking milliseconds to run. Fast tests allow for frequent execution, enabling developers to get quick feedback on code changes.

   +  Isolated: Unit tests should be isolated from external dependencies, such as databases, file systems, or network resources. They should be self-contained and not rely on external factors that can introduce variability or fragility into the test results.

  + Repeatable: Unit tests should produce consistent results when executed multiple times, as long as the code being tested remains unchanged. Tests should not rely on randomness or time-based factors that can cause inconsistent outcomes.

  + Self-Checking: A good unit test should automatically determine whether it has passed or failed without any human intervention. The test assertions should clearly indicate the expected behavior and verify it against the actual outcome.

  + Timely: Writing unit tests should not consume a disproportionately large amount of time compared to writing the code being tested. Test development should be efficient, and the effort invested in writing tests should be proportional to the complexity and criticality of the code being tested.
  
Following these characteristics ensures the test is reliable.

the readabillity of a test is also very importand for debugging, microsoft recomends to follow the Arrange-Act-Assert (AAA) pattern. This pattern separates the setup (arrange) phase, the execution (act) phase, and the verification (assert) phase of the test. Clearly organizing these steps helps in understanding the dependencies, the code being tested, and the expected behavior. [[4]](https://learn.microsoft.com/en-us/dotnet/core/testing/unit-testing-best-practices)

In order to keep unit tests focused on testing a single unit of code, developers often use mocking or stubbing techniques. Mocking involves creating objects that simulate the behavior of real objects but are specifically designed for testing purposes. These mock objects allow developers to isolate the code under test and control the behavior of external dependencies.

By using mocks, developers can replace complex or slow dependencies, such as databases, web services, or external APIs (in my case), with simplified versions that provide predetermined responses. This way, unit tests can execute quickly and in a controlled environment, without relying on external resources.[[5]](https://jestjs.io/)

## Sources

[1] Source: "Unit Testing Tutorial – What is, Types & Test Example" Thomas Hamilton, https://www.guru99.com/unit-testing-guide.html

[2] Source: "Integration testing or integration and testing (I&T)" Rahul Awati, https://www.techtarget.com/searchsoftwarequality/definition/integration-testing

[3] Source: "Combine API and UI Testing For Confidence At Every Layer Of Your Application" Smartbear , https://smartbear.com/learn/automated-testing/what-is-end-to-end-testing/

[4] Source: "Unit testing best practices with .NET Core and .NET Standard" Microsoft , https://learn.microsoft.com/en-us/dotnet/core/testing/unit-testing-best-practices

[5] Source: "Jests official docs" Jest , https://learn.microsoft.com/en-us/dotnet/core/testing/unit-testing-best-practices
