# GoogleGmailAPI
A Basic Implementation of the GmailAPI Authorized to Read(Modify) Emails from gmail Inbox. 

What was the purpose.

We had to test a functionality of a web app that can able to create a user from the UI which sends a password to user's Email Id. We need to login using the password sent to user, to complete the test Scenario. 

The hard part was to automate the retrival of the password as this is sitting inside the user's Inbox. 

Initally we thought of Opening the User Email(Fake user) by automating the user name and password fills as part of the test Scenario. This was going in a whole different direction as lot of email clients do not allow  Frequent Login attempts and thrown in an captcha Login. (captcha 1 Automation 0).

Then I thought of, if we can get the password from an API reading through the user Inbox. TADA ! New repo !!!

### Steps
It tooks less than 30 mints to get into Gmail Inbox and through the Emails. All thanks to Awesome Team at Google writting docs: 

https://developers.google.com/gmail/api/quickstart/js


Use this wizard to create or select a project in the Google Developers Console and automatically turn on the API. Click Continue, then Go to credentials.

On the Add credentials to your project page, click the Cancel button.

At the top of the page, select the OAuth consent screen tab. Select an Email address, enter a Product name if not already set, and click the Save button.

Select the Credentials tab, click the Create credentials button and select OAuth client ID.

Select the application type Web application.

In the Authorized JavaScript origins field, enter the URL http://localhost:8000. You can leave the Authorized redirect URIs field blank.

Click the Create button.

Take note of the client ID in the resulting dialog. You will need it in a later step.

Click OK to dismiss the resulting dialog.

## YOUR ARE DONE

Replace the Client Id at : https://github.com/symmetriccurve/GoogleGmailAPI/blob/master/index.html#L59 


Click on Authorize, Select(if loggedIn) the Gmail Account to read from .  Play around the methods on the gapi for more Understanding.



