# JS SDK API Example

This example is intended to run through all the various methods of the JS SDK.

# Prerequisites

<a href="https://www.stackmob.com/platform/api/schemas/create" target="_blank">Create these schemas</a> for your example app:

* `message` schema with a `string` field named `content`
* `user` schema with a `one to many` relationship with a `message` schema.
* `attraction` schema with a `geopoint` field named `location`

I know, would be nice to have these precreated for you, right?  That idea's in the feature list - sharable schema templates.  (But I digress)  

# Facebook Example Prerequisites

* user schema with FaceBook methods enabled
* FaceBook App ID (optional)

# OAuth 2.0 Example Prerequisites

StackMob will be transitioning JS security to OAuth 2.0, requiring your users to login to access restricted methods you specify.  The provided form shows how you can login.  You will get OAuth 2.0 access tokens in return.  Make calls as you normally would after.  To setup:  

* include your `publicKey: 'your public key'` in `StackMob.init` to enable OAuth 2.0 mode
* `user` schema with OAuth 2.0 methods enabled

# Running this example

Run this example from the `stackmob-javascript-example` root folder.

Click on the various links to trigger an API call.  Some examples require you to click on one link before another.  For instance, you can only "Read a User" after you "Create a User".  It should generally be intuitive.  

# Running this example with OAuth 2.0

1.  The OAuth 2.0 section will require a light modification to your `StackMob.init`.  Add your public key:

```javascript
StackMob.init({
  ...
	publicKey: 'your public key',
	...
});
``` 

2.  Click on the regular API links: Read User, Delete User.  You'll receive 401 unauthorized calls because you haven't logged in yet.
3.  Next, create a user via the link provided in that OAuth 2.0 section then login.  You'll be redirect to a login result page.
4.  Click back and try out all the methods again.  They should start working, and you should see `Authorization: MAC ....` in the request headers. 

