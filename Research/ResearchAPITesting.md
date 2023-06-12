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
This research aims to explore the most effective strategies and tools for testing my API.



## What does my API do?
***
My API is designed to provide a convenient and user-friendly way to search for games based on specific categories. By using the IGDB (Internet Game Database) API, you can request games belonging to various genres, platforms, or themes. The API acts as an intermediary, interacting with the IGDB API to retrieve relevant game data. Additionally the microservice retrieves the necessary access key and stores it in a JSON format. This allows for seamless and efficient communication between the microservice and the IGDB API.



## How to write a good test
***
When it comes to writing good tests there are some key principles to follow. One important aspect is to ensure readability, which greatly aids in debugging and maintaining the test suite over time.

One recommended approach is to use the Arrange-Act-Assert (AAA) pattern, as suggested by Microsoft's unit testing best practices. This pattern involves structuring the test into three distinct phases:

  + Arrange: In this phase, you set up the necessary preconditions for the test. This includes initializing objects, configuring dependencies, and preparing the system under test to be in a specific state.

  + Act: The act phase is where you perform the specific action or operation that you want to test. This could be calling a method, invoking a function, or simulating user interactions. The focus is on triggering the behavior that you want to verify.

  + Assert: In the assert phase, you make assertions to verify the expected behavior of the code being tested. You compare the actual results or state of the system under test with the expected outcomes. If the assertions pass, the test is considered successful; otherwise, it indicates a failure.

By following the AAA pattern, you make the test structure clear and explicit, allowing for better comprehension of the test's purpose and flow. This pattern also helps in understanding the dependencies and interactions involved in the test, making it easier to identify and diagnose any issues that may arise.

In addition to the AAA pattern, other good practices for writing tests include keeping them fast, isolated, repeatable, and self-checking. These characteristics ensure that tests are reliable, provide quick feedback, and can be executed frequently without relying on external dependencies or producing inconsistent results.
[[4]](https://learn.microsoft.com/en-us/dotnet/core/testing/unit-testing-best-practices)



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


## Sources

[1] Source: "Unit Testing Tutorial – What is, Types & Test Example" Thomas Hamilton, https://www.guru99.com/unit-testing-guide.html

[2] Source: "Integration testing or integration and testing (I&T)" Rahul Awati, https://www.techtarget.com/searchsoftwarequality/definition/integration-testing

[3] Source: "Combine API and UI Testing For Confidence At Every Layer Of Your Application" Smartbear , https://smartbear.com/learn/automated-testing/what-is-end-to-end-testing/

[4] Source: "Unit testing best practices with .NET Core and .NET Standard" Microsoft , https://learn.microsoft.com/en-us/dotnet/core/testing/unit-testing-best-practices

[5] Source: "Jests official docs" Jest , https://learn.microsoft.com/en-us/dotnet/core/testing/unit-testing-best-practices
