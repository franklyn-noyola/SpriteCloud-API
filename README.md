# SpriteCloud-API
Introduction
Welcome to my test automation project, there're two different test files to validate the environments that were given (Web and API). In this readme file you'll find how to run those test files and also how to set Jenkins as the CI/CD tool to run those tests in a pipeline and provide the reports and results. Let's start to play with this!

First Steps
Clone the Github repo into your local machine from the master branch.

Install the following:

Install Python: https://www.python.org/downloads/ - For this project I have installed the latest version (3.10.1) of python. (You can check the documentation to make sure you have installed Python properly for your corresponding OS)

Install or Upgrade your Pip - You can upgrade by using the command: python -m pip install --upgrade pip

Now with Pip installed/upgraded, install the following:

Robot Framework - command: pip install robotframework

Selenium Library- command: pip install robotframework-seleniumlibrary

Requests Library - command: pip install robotframework-requests

JSON Library - comand: pip install robotframework-jsonlibrary

Now you are all set to run the test cases for the two environments. Let's move to the next thing.

ToolsQA site - 1st Project
Environment: https://demoqa.com/

For the first project we are going to validate a Website and you'll find some tests UI based. Let's see how to run the tests in different ways.

Run the tests Locally
To run the tests into your local machine, make sure you are on the placed in the SpriteCloud folder, if not you can always use the fancy cd SpriteCloud command in your terminal.

Now you can execute the following command: robot -d Results  Tests/DemoQA/DemoQATest.robot

After execution is done and succesfull, you can go to the SpriteCloud/Results folder and you should be able to see the log.html, output.xml and report.html files generated.

Run the tests via Jenkins
First of all, you've to install Jenkins. Follow the instructions to install it depending on your OS: https://www.jenkins.io/doc/book/installing/ (I've installed Jenkins LTS for Mac OS).

After you followed the instructions and you are able to log in into jenkins, you should create the new pipeline where the tests will be run.
