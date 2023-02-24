
### Here is the background information on your task
Typically, traders monitor stock prices and trading strategies by having data displayed visually on their screens in chart form. Often these charts will be accompanied by alerts that notify users when certain events occur or when preset price thresholds are hit.

JPMorgan Chase created the Perspective tool over many years to allow users to present and manipulate data feeds visually in web applications.

Perspective provides a set of flexible data transforms, such as pivots, filters, and aggregations. It utilises bleeding-edge browser technology such as Web Assembly and Apache Arrow and is unmatched in browser performance. It is engineered for reliability and production-vetted on the JPMorgan Chase trading floor. Now it’s available to the development community as an open source library. If you want to explore that, a link is provided in the resources section.


### Here is your task
For the second module of this project, you will need to accomplish the following:

Set up your local dev environment by downloading the necessary files, tools and dependencies.
Fix the broken typescript files in the project repo to make the web application output correctly.

### Set-Up

Just like in the last task, you need to get your local development environment up and running. Given that you completed Task 1, you should already have python installed and be familiar with git.

First, fork and clone the project repo: 

https://github.com/vagabond-systems/jpmc-task-2

Remember to uncheck the “Copy the main branch only” box in the fork dialog on GitHub. A model answer has been provided in a separate branch from main.

<img width="820" alt="PyCharm IDE" src="https://user-images.githubusercontent.com/104922257/221221808-b46fd6fe-045b-4976-af01-7f053cb47090.png">

• Create a new virtual environment in the project root. Pycharm can do this automatically for you using the “configure python interpreter” option in settings.

<img width="787" alt="interpreter" src="https://user-images.githubusercontent.com/104922257/221220260-aaa4399f-bc58-4ed2-9ec0-d90e28061a41.png">

• Install all project python  dependencies. These are listed in the requirements.txt file.

In this task, we will be working with javascript in addition to python. Javascript has a handy package manager called npm, which handles package tracking, discovery, installation, and removal. We will be using it to install a series of javascript dependencies to your machine. If you already have access to npm on your system, you can skip this step. Otherwise, you will need to acquire it by following the instructions here (npm comes bundled with nodejs): 

https://nodejs.dev/en/learn/how-to-install-nodejs/

For this project to work, you must have node 18.10.0 installed on your machine. Ensure you have the correct version by running “node -v” in your terminal. If you do not, consider using nvm to install the correct version for you.

<img width="666" alt="node version" src="https://user-images.githubusercontent.com/104922257/221221063-eade5694-445d-4364-87c4-5ecdbbd5b4b1.png">

• Install the necessary dependencies by running `npm install` from the project repo

<img width="675" alt="npm install" src="https://user-images.githubusercontent.com/104922257/221221138-f8b77d98-5e40-4bba-8483-189d154f0c08.png">

• Start the python server by running server.py from the project repo
• Start the client by running `npm start` from the project repo

<img width="846" alt="npm start" src="https://user-images.githubusercontent.com/104922257/221221201-a1b0a510-8ce2-43ab-b753-64ac85def61b.png">

### Making Changes

When you’re in a work environment, you’ll usually receive tasks in the form of engineering tickets.
Here is an example of what this task looks like in the form of an engineering ticket.

#### Purpose:

The objective of this task will be for you to fix the client-side web application so that it displays a graph that automatically updates as it gets data from the server application (see Before and After images below). Currently, the web application only gets data every time you click on the 'Start Streaming Data' button and does not aggregate duplicated data.

####  Acceptance Criteria:

This ticket is done when the graph displayed in the client-side web application is a continuously updating line graph whose y-axis is the stock’s top_ask_price and the x-axis is the timestamp of the stock. The continuous updates to the graph should be the result of continuous requests and responses to and from the server for the stock data.
This ticket is done when the graph is also able to aggregate duplicated data retrieved from the server

#### Resources to help you with the task: 

https://nodejs.dev/en/learn/how-to-install-nodejs/

https://perspective.finos.org/

https://github.com/finos/perspective




