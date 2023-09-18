Some problems that we encountered while trying to get any of our projects to run are free services no longer being free, out-of-date versions for dependencies, expired links, and not being able to get access to the AWS account.

When trying to run the ClassMate project it used Heroku to run its cloud database. Heroku has been free for students in the past but in 2022, Heroku discontinued free tier and only had paid models. As such we decided to no longer pursue running that project.

The Sync-Ends project which we ended up getting to work had two issues. The first issue appeared during installation when pip could not install the version of typed-ast that was specified in the requirements.txt file. This caused us to switch from trying to install Sync-Ends via pip and the PyPi package. We instead cloned the repo using git and modified the requirements.txt file manually to the correct version of typed-ast. This then caused some issues with running the project as the instructions in the doc were no longer accurate. Through trial and error and some helpful, and less-than-helpful, error messages; we were able to run the program. This introduced the second issue of the link to a postman collection provided in the doc is outdated and no longer works. This caused us to have to dive into postman collections and create one and the APIs held inside ourselves.

During the setup for project Similii, there was an issue with using the AWS services that it needed. We reached out to the past contributors to get access but did not receive a response. It would've been helpful if they left some notes about AWS account management, but unfortunately we couldn't work past it.

The slackbot project has some bugs in it. In the README file, during setup, they mentioned the API_TOKEN variable to create, but they used a different name in the code. Without that, the code was throwing some different errors including one with Pickle Module errors. Also, some functionalities weren't working like the Email feature, which required additional efforts into diving at it. Its showing that there is some SMTP error related to email id and password authentication. We tried using a different combination apart from the one provided in the code, but it didn't work as expected. Also, the code readability wasn't so great, as the core code for the project was extended in a single file. Overall the project was running fine after some tinkering, maybe improvements over existing functions and the ones which were throwing errors can be looked into.

The Recipe Recommender setup was smooth and easy. However once we started running it, only the frontend part was working fine, including adding ingredients to the list. The backend, however couldn't work, where the search results weren't popping up. Upon back-tracking to the problem, it has been identified that a backend API issue, which needs more time to explore upon.

Overall, Sync-ends and Slackbot applications were proved to be less painful to setup, but successfully run on our local machines. The Recipe Recommender(STAR GEN) project's frontend part had no issues at all, however the backend needs to be explored further. Sync-ends functionality is perfectly working as described in the README and Slackbot functionalities were partially run. For improvements,
In Sync-Ends:
    we can first update the README file with latest instructions, add auto logging of all the APIs in question at someplace so that its history can be tracked properly.
In slackbot:
    Improve code readability via modularization, update README file with correct instructions, making sure that the functionalities in README are working properly. Also, making sure to perform code review and remove hand-coded variables (like system path, variable names).


