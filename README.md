# StackMob Javascript Examples

Here are examples of the StackMob JS SDK.  This repo will house examples showcasing the JS SDK's features and will also serve as a demo/how-to area. 

# Contents

Included are examples housed in each respective folder.  Each project refers to the StackMob JS SDK `stackmob.js` in the root folder. 

# Running the Examples 

Fork or clone this repo.  You'll get the HTML files and also the respective version of the StackMob JS SDK that works with these projects.

You'll need to initialize `StackMob.init({ ... })` with your application's information.  Some of these examples also need specific schemas and relationships set up.  These will be described in the example pages.

When setting up your StackMob Local Runner to run these locally, setup your `.stackmob` config file in this root folder:

		/stackmob-javascript-examples/.stackmob
		
You should then run StackMob Local Runner from the root folder.  Your Terminal:

		stackmob-javascript-examples>  stackmob server
   
This is required because the projects refer to the JS file relatively:

		<script type="text/javascript" src="../stackmob.js"></script>
		
Once Local Runner is running, feel free to start exploring!

<a href="http://127.0.0.1:4567/api/examples.html" target="_blank">http://127.0.0.1:4567/api/examples.html</a>

# Contributing to the Examples

Have some examples on how to use the StackMob JS SDK in NodeJS?  How about CoffeeScript?  Email us at support@stackmob.com or simply fork this repo and submit a pull request!  

If you'd like to share your repo, contact us at support@stackmob.com and we can also link to it.

