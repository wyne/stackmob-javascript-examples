# OAuth 2.0 Login Example

StackMob will be transitioning JS SDK users to authenticating users with OAuth 2.0 (think similar to Facebook/Twitter JS SDKs).  Your app will have open access to people to create an account, but requests after that will optionally require authorization credentials.  The JS SDK does most of the heavy lifting.

This example is to show people how to use OAuth 2.0 before it becomes the standard for which to connect to StackMob.

This example:

* shows you how to setup your OAuth 2.0 authentication form.  
* shows you how to create a user
* show that calls without login are rejected
* show that calls after login (with authorization credentials) are accepted

Because the form is a UI component and you likely want to style it to your UI, we've kept the HTML as light as possible.

You can read more about <a href="" target="_blank">setting up OAuth 2.0 in your app</a> in our docs.  

# Prerequisites

* Make sure OAuth 2.0 is checked off at the bottom of <a href="https://www.stackmob.com/platform/api/schemas/edit/user" target="_blank">your user schema</a>.

# Running this example

Run this example from the `stackmob-javascript-example` root folder.

## Trying a calling DELETE with no authorization credentials

1.  Visit <a href="http://127.0.0.1:4567/authorization/oauth.html" target="_blank">http://127.0.0.1:4567/api/oauth.html</a>.
2.  Click on Delete User.  It will fail because you don't have authorization credentials yet.

## Login - Get Authorization Credentials


1.  Visit <a href="http://127.0.0.1:4567/authorization/oauth.html" target="_blank">http://127.0.0.1:4567/api/oauth.html</a>.
2.  Click the "Create a User" link.  A user will be created with username `oauthtestuser` and password `oauthtestpassword`.
3.  Submit the login form.  The fields are prepopulated with the user.
4.  You're now logged in.
5.  Click on the Delete User link.  It will now allow you to do so.  

