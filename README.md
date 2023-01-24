# SpriteCloud-API
# Introduction
Welcome to my API test automation project, there are four cases to these kind of test (POST, PUT, GET AND DELETE). In this readme file you'll find how to run those   kind of test, both locally (manually) or automatically (By Jenkins jobs) and provide the reports and results. Let's start to going through with this!

<b> First Steps </b> <br>
* Download Postman application https://www.postman.com/downloads/, if you don't have it installed, once you have it installed, create your scripts accordingly (JSON request), Once you have created your scripts, export the collection (test scrips created) to a JSON File and upload them into a remote repository, i.e. GitHub. 

* Clone the Github repo into your local machine from the master branch.

Install the following:
* Install NPM.
* Install Python: https://www.python.org/downloads/ - For this project I have installed the latest version of python. (You can check the documentation to make sure you have installed Python properly for your corresponding OS)
* Install Newman in the command line: npm install newman.
Install or Upgrade your Pip - You can upgrade by using the command: python -m pip install --upgrade pip

# ToolsQA site - 1st Project
Environment: https://petstore.swagger.io/

For this project we are going to validate APIs and you'll find some tests API based. Let's see how to run the tests in different ways.

<b>Run the tests Locally</b><br>
* To run the tests into your local machine, make sure you are on the placed in the workspace/SpriteCloud folder, if not you can always use the fancy cd SpriteCloud command in your terminal.
* Open Postman and retrive the APIs test scripts in the corresponding folder, you can run them one by one or all the collection.
* After execution is done and succesfull, you can see the results in the Postman results pane.

<b>Run the tests via Jenkins</b><br>
First of all, you've to install Jenkins. Follow the instructions to install it depending on your OS: https://www.jenkins.io/doc/book/installing/ (I've installed Jenkins for Windows latest version).

After you followed the instructions and you are able to log in into jenkins, you should create the new pipeline where the tests will be run.

<b>Follow the following steps: </b>
1. Create a New Item and select Freestyle Project (put a name for your jenkins job)
2. Click on OK Button
3. Once you are in your Freestyle project screen
4. Configure the project as follow:

![image](https://user-images.githubusercontent.com/17472758/214373506-ee9ed0fd-4401-4004-bd2f-b5b5b7d72a4c.png)
![image](https://user-images.githubusercontent.com/17472758/214373852-ee7e84ec-9ea4-4d9c-9689-fc8b8ee85054.png)
5. In the "Build" section select "Add build step" and from the dropdown pick "Execute shell" (or "Windows batch command" if it's your case)
6. In the command field add the command used to run the tests locally:
![image](https://user-images.githubusercontent.com/17472758/214373900-fe448faf-c8e8-4fcb-8941-4dddde263bb4.png)

# About the Scenarios
As a CRUD API it's important to make sure that data basic functionalities are covered, so based on that and the fact that is a pet store I've selected 3 of the Pet endpoints to add an User, after it's added, then I can update the Pet info, get the information and delete user and at the end reviewing the User again and make sure the User was deleted, cause this is a Pet store and first of all we want to make sure we are able to add the records for the Pets, before doing anything else with this information.

# Next Steps
The next steps for this project will be to increase more test cases, invalid ones, because all of these cases are happy path, and they are not validating if the field is carrying on with the expected field format, in order to check if there are bugs in there, so in this way I can report the bugs if any and report them to Dev in order to fix them and retest them.

