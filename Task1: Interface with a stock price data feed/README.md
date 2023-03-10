## Here is the background information on your task

You’ve been asked to assist with some development to add a chart to a trader’s dashboard allowing them to better identify under/over-valued stocks.

The trader would like to be able to monitor two historically correlated stocks and be able to visualise when the correlation between the two weakens (i.e. one stock moves proportionally more than the historical correlation would imply). This could indicate a potential trade strategy to simultaneously buy the relatively underperforming stock and sell the relatively outperforming stock. Assuming the two prices subsequently converge, the trade should be profitable.

Most data visualisation for our traders is built on JPMorgan Chase's Perspective data visualisation software, which is now open source. If you want to explore that, a link is provided in the resources section.

Before implementing this request using perspective, first, you’ll need to interface with the relevant financial data feed and make the necessary adjustments to facilitate the monitoring of potential trade opportunities.



## Here is your task:

For the first module of this project will need you to accomplish the following:


Set up your local dev environment by downloading the necessary repository, files, tools and dependencies
Fix the broken client datafeed script in the repository by making the required adjustments to it.
Push your changes and submit your work.

## Set-Up

Before you can tackle any software development task, you need to set up your development environment. You can think of your local development environment as a virtual workbench with all the tools necessary to work on your project. To set up your dev environment, follow the following instructions:


Install python 3 to your system - any recent version of python 3 will work fine, though the most up-to-date version is advisable. If you need help with this step, check out this excellent guide from real python: https://realpython.com/installing-python/

<img width="563" alt="python version check" src="https://user-images.githubusercontent.com/104922257/217436615-8e29d6e4-5ab0-4fc6-b448-bfc475f8d616.png">


<img width="800" alt="download latest version python" src="https://user-images.githubusercontent.com/104922257/217435673-6d4a1d87-36f3-431d-819f-d1d3497eded5.png">


Fork and clone the starter repo here: https://github.com/vagabond-systems/jpmc-task-1
IMPORTANT! Uncheck the “Copy the main branch only” box in the fork dialog on GitHub. A model answer has been provided in a separate branch from main.
if you are unfamiliar with forking, cloning, or git in general, take a look at the first two chapters of the git book here: https://git-scm.com/book/en/v2

<img width="900" alt="fork" src="https://user-images.githubusercontent.com/104922257/217436801-ccfd929b-6ba1-4636-8b35-6046b238e72d.png">



<img width="900" alt="HTTP" src="https://user-images.githubusercontent.com/104922257/217436847-b2028093-3bc8-43eb-9ab1-313078a9b2ed.png">



<img width="627" alt="cloning" src="https://user-images.githubusercontent.com/104922257/217436874-f9806553-ed16-4969-9d29-b1de73e1758d.png">


Open the project in your IDE of choice - if you don’t have a favourite python IDE yet, take a look at Pycharm Community Edition. It’s a well-designed IDE by Jetbrains packed with features and plugins, powerful enough to work on the most complex projects, and entirely free.

<img width="800" alt="PyCharm IDE" src="https://user-images.githubusercontent.com/104922257/217437379-1954a2e9-8f0d-4fe8-98b6-7d4629ec3fc6.png">

Create a new virtual environment in the project root. Pycharm can do this automatically for you using the “configure python interpreter” option in settings.
Install all project dependencies. These are listed in the requirements.txt file.


<img width="803" alt="venv" src="https://user-images.githubusercontent.com/104922257/217438345-173eb26e-b31a-4d02-b061-e0054cd04f60.png">

<img width="800" alt="open folder" src="https://user-images.githubusercontent.com/104922257/217437364-e2f6a0ed-b3ff-4c12-95d7-dd4636ebe2c8.png">


Congrats, you’ve got your local development environment up and running! Now it’s time to make changes to the codebase.

## Making Changes

When you’re in a work environment, you’ll usually receive tasks in the form of engineering tickets. Here is an example of what this task looks like in the form of an engineering ticket

[task_1_guide.docx.pdf](https://github.com/f-Safdar/J.P.-Morgan-Chase-Co-Software-Engineering-Virtual-Experience/files/10691385/task_1_guide.docx.pdf)

#### Purpose

We want to process the data feed of stock A and stock B’s price to enable us to analyse when trading for the stock should occur.

#### Acceptance Criteria

* getDataPoint function should return correct tuple of stock name, bid_price, ask_price and price. Note: price of a stock = average of bid and ask

* getRatio function should return the ratio of the two stock prices

* main function should output correct stock info, prices and ratio.
