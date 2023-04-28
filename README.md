# Translate Emailer App


An web application that is used to send out translated email to multiple groups of recipients.

## Features

User can import or manually store customers' information on the application's built in database.
User can easily make changes to any customer's info on the app.

User can compose the email in any languages and customers will receive the translated version based on their language preferences.
Installation

This guide assume that user already have a Google Cloud Account.

## Set up a SendGrid Account


Go to SendGrid's Sign Up Page and open a new account.
Once logged in, on the main screen, click Create a Single Sender.
Fill out the Create a Sender page.
Confirm your email (User might need to add Two-Factor Authenticator).
Once email is verified, on the right panel, choose Email API. Under the drop-down menu, choose Integration Guide.
Choose Web API
Choose Python
On Create an API key section, enter a name for your key, then click Create Key
Copy this key
That's all you will need for this step.

## Create a new project on Google Cloud Platform

Navigate to the search box on the top bar and search for Create a Project
Enter the name for your project then click Create
From the project drop-down selector, copy ID of the project that you just created, then choose to switch to that project.
Activate the Cloud Shell by clicking the logo to the left of the search box
On the terminal, run the command (replace [PROJECT-ID] with the ID that you just copied)
gcloud config set project [PROJECT-ID]
You have just set up the environment to deploy the project!

## Enable Google Translate API
Navigate to the search box and search for Cloud Translation API
Click the result under Marketplace
Enable the API
Clone and edit the project
On the terminal, run the command
git clone https://github.com/uconnstamford/translate-emailer-app
Navigate to Open Editor
Once entered the Editor, on the left menu, navigate to folder translate-emailer-app
Open the config.py file under translate-emailer-app
Follow the instruction in the config file and fill out all required variables.
Save all file
Now, go back to the terminal, run the command
cd ~/translate-emailer-app/ && gcloud app deploy && gcloud app browse
If the region selection pops up on the terminal, choose 17. Then choose Y
Wait about 3 minutes for the terminal to finish deploying. Then click the application link to launch the App Engine.
