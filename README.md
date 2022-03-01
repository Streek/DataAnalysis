# Datascience Project (Github Languages)
## Table of Contents
1. About the Dataset
2. Rationale
3. Major Questions
a. What are the most popular languages now? (At the latest data possible)
b. What were the most popular languages at the earliest data point.
c. What languages have grown the fastest?
d. What languages have stayed high in popularity the longest?
e. If we had to pick a language to learn which one should we do?
4. The Approach
5. Technical Challenges
a. Dataset doesn't have a lot of information beyond counts.
b. Not granular enough.

## About the dataset
The dataset is a collection of issues, pull requests, and repositories that exist for each language on github as well as what year and quarter the reading was taken in.  The data set is simple but complete.

The data resides in the `./data` folder
## Rationale
I decided to use the github public respositories dataset because as a software engineer I always find it interesting what languages are popular, how quickly they raise and lower in popularity, and other metrics.  I'm commonly asked by people getting into engineering what language they should start with.  There's a lot of things that go into figuring out which language is the "right" one.  We can pick the most popular language at the time but who knows if it'll start popular in a few years, will you be able to find a job using that language.
## Major Questions
### What are the most popular languages now? (At the latest data possible)
We have data from 2011 to 2022, so at the beginning of 2022 (it's currently Q1 2022) what languages are most popular by count.  Can we gather any other insights from counts related to repos, issues, or pull requests?  Is there a most collaborative language?  Or a language with less errors per repository?
### What were the most popular languages at the earliest data point?
As above, in 2011 which languages have the most repositories, issues, or pull requests?  How similar is the list?
### What languages have grown the fastest?
What languages have grown the fastest from 2011 to 2022, is it different if we look at repositories versus if we look at issues or pull requests?
### What languages have stayed high in popularity the longest?
If we see a langauge in the top most popular early and late in the data set, have they stayed there the whole time?  Can we assume these are the most popular languages and thus will continue to be popular?
### If we had to pick a language to learn which one should we do?
Based on this is there a best language to pick for a new programmer based on popularity or use?

## Approach
This data set is pretty simple, we have the language name, the year, the quarter, and the count for that quarter in the form of CSV files.  Each CSV file is for another type of data, E.g. repositories, issues, pull requests, etc.

To unify the data we are renaming and merging the counts accross files.

I use pipenv which handles the virtualenv, python version, and pip versions, in one tool.
I setup the data in jupyter notebook.

The notebook file is `./Data.ipynb`

## Technical Challenges
The dataset is pretty simple.
There was some issues for some reason setting up the pipenv virtualenv but once I re-setup my pipenv it worked flowless.  I believe this was related to M1 mac issues in the version of python I had setup originally.

My Objectives:
Prepare data:
Gather necessary data to answer your questions
Handle categorical and missing data
Provide insight into the methods you chose and why you chose them
Analyze, Model, and Visualize
Provide a clear connection between your business questions and how the data answers them
4) Communicate your business insights:

Create a Github repository to share your code and data wrangling/modeling techniques, with a technical audience in mind
Create a blog post to share your questions and insights with a non-technical audience
Project Deliverables
There are two deliverables that are required for project completion.

A Github repository for your code.
A blog post of your findings.
Your Github repository must have the following contents:

A README.md file that communicates the libraries used, the motivation for the project, the files in the repository with a small description of each, a summary of the results of the analysis, and necessary acknowledgments.
Your code in a Jupyter notebook, with appropriate comments, analysis, and documentation.
You may also provide any other necessary documentation you find necessary.
For the blog post, pick a platform of your own choice. For example, it can be on your website, a Medium post (Josh's sample report on How Do YOU Become A Developer?), or a Github blog post. Your blog must provide the following:

A clear and engaging title and image.
Your questions of interest.
Your findings for those questions with a supporting statistic(s), table, or visual.
Note: The post should not dive into technical details or difficulties of the analysis; this should be saved for Github. The post should be understandable for non-technical people from many fields.