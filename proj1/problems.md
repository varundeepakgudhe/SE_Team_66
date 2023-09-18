Some problems that we encountered while trying to get any of our projects to run are free services no longer being free, out-of-date versions for dependencies, expired links, and not being able to get access to the AWS account.

The ClassMate project encountered a roadblock when Heroku discontinued its free student tier in 2022, shifting exclusively to paid models. This change in pricing made it financially challenging to continue running the project, leading us to suspend further development. Staying updated on cloud service providers' pricing policies is crucial for project sustainability and cost management. In response to these challenges, evaluating alternative hosting options may be necessary for the project with limited budgets.

The Sync-Ends project which we ended up getting to work had two issues. The first issue appeared during installation when pip could not install the version of typed-ast that was specified in the requirements.txt file. This caused us to switch from trying to install Sync-Ends via pip and the PyPi package. We instead cloned the repo using git and modified the requirements.txt file manually to the correct version of typed-ast. This then caused some issues with running the project as the instructions in the doc were no longer accurate. Through trial and error and some helpful, and less-than-helpful, error messages; we were able to run the program. This introduced the second issue of the link to a postman collection provided in the doc is outdated and no longer works. This caused us to have to dive into postman collections and create one and the APIs held inside ourselves.

During the setup process for the Similii project, a significant obstacle arose due to issues related to AWS (Amazon Web Services) services that were required but inaccessible. The project team made diligent efforts to contact past contributors who might have had access to the necessary AWS resources, but regrettably, there was no response from them. In such situations, having notes or documentation regarding AWS account management left by previous contributors could have been immensely beneficial. Documentation or notes detailing AWS account setup, configurations, and resource management can be invaluable for ensuring the continuity of a project, especially when transitioning between contributors or team members.

The Slackbot project encountered a series of bugs that required meticulous troubleshooting. The README file initially indicated the need to set up an API_TOKEN variable, but within the codebase, a different variable name was employed. This inconsistency led to a cascade of issues, including unexpected errors involving the Pickle Module. Consequently, extensive debugging efforts were necessary to align the variable names correctly and rectify the associated errors. Furthermore, certain functionalities within the Slackbot project exhibited suboptimal performance. One notable problem arose in the Email feature, which demanded additional investigation. A persistent SMTP error tied to email ID and password authentication posed a significant challenge. Attempts were made to experiment with alternative combinations beyond those predefined in the code, but they weren't fruitful as well. Code readability also emerged as an area requiring attention for this project, where the core codebase was consolidated into a single file, resulting in reduced clarity and maintainability. To enhance the project, ensuring that existing functionalities are working, correct encoding of variables in both code and README and modularization should be considered.

On a positive note, the setup for the Recipe Recommender went relatively smoothly, with minimal hurdles encountered during the initial installation. However, as the application was set in motion, disparities emerged between the frontend and backend components. While the frontend operated seamlessly, allowing users to add ingredients to their list, the backend struggled to deliver search results as expected. This setback was traced back to an issue with the backend API, requiring further investigation and debugging, which proved to require additional time.

In summary, both Sync-Ends and Slackbot applications exhibited reasonable ease of installation on local machines, though they each presented unique challenges during runtime. The Recipe Recommender's frontend displayed robust performance, but the backend warrants additional attention.

To drive improvements in the working projects:

For <b>Sync-Ends:<b>

Begin by updating the README file with the most up-to-date instructions to streamline the setup process.
Consider implementing an automatic logging mechanism for all pertinent APIs, promoting a comprehensive history for better tracking and debugging.

For <b>Slackbot:<b>

Prioritize enhancing code readability through modularization, promoting a more organized and maintainable codebase.
Revise the README file to ensure accurate and effective setup instructions, and verify that all functionalities outlined in the README are fully functional.
Conduct a thorough code review, aiming to eliminate hard-coded variables (such as system paths and variable names), which can lead to improved code flexibility and robustness.
These enhancements are expected to contribute to a more seamless user experience and more robust functionality within both projects.



