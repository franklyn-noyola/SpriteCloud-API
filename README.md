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

ToolsQA site - 1st Project
Environment: https://petstore.swagger.io/

For this project we are going to validate APIs and you'll find some tests API based. Let's see how to run the tests in different ways.

<b>Run the tests Locally</b><br>
To run the tests into your local machine, make sure you are on the placed in the workspace/SpriteCloud folder, if not you can always use the fancy cd SpriteCloud command in your terminal.

Open Postman and retrive the APIs test scripts in the corresponding folder, you can run them one by one or all the collection.

After execution is done and succesfull, you can see the results in the Postman results pane.

<b>Run the tests via Jenkins</b><br>
First of all, you've to install Jenkins. Follow the instructions to install it depending on your OS: https://www.jenkins.io/doc/book/installing/ (I've installed Jenkins for Windows latest version).

After you followed the instructions and you are able to log in into jenkins, you should create the new pipeline where the tests will be run.
