# Workflow Analysis

## A. The workflow is triggered when code is pushed to main branch, or when a pull request is made for the made branch 

## B. The four steps are as follows: 
1. Checkout Code - Get the code from the repository 
2. Validate HTML - Validate HTML Files
3. Check links - Check for Broken Links
4. Upload artifact - Upload the built site for deployment 

## C. The checkout code step uses actions/checkout@v4 to get the code from the repository. This is necessary, because every step after will need the most up to date code to run   their   checks 
## D. The enviornment configuration configures GitPages to prepare the website for deployment. 
## E. The automated deployment is more reliable then manmually deploying, because it automatically validates HTML, checks for broken links, makes sure that only code pushed to the main branch is deployed. In tandem, this reduces human error, as it actively validates, and makes sure no unfinished branches are pushed. 
## F. If we pushed code to a different branch, the deployment would not happen, as it is only called when anything is pushed to the main branch. 