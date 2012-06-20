# StackMob Javascript Examples

Welcome!  Here are several examples utilizing the JS SDK.  Feel free to use the code as you wish - copy, reuse.. recycle?  

There are demos and examples for your reference.

Do you need a GitHub project simply to try StackMob hosting?  Feel free to use this one by forking it to your account!

You can find the `stackmob-javascript-examples` repo at <a target="_blank" href="https://github.com/stackmob/stackmob-javascript-examples">https://github.com/stackmob/stackmob-javascript-examples</a>   

# Contents

The root folder has `index.html` which will get you started right away!

Included are examples housed in each respective folder.   

# Running the Examples 

You're here because you downloaded the JS SDK Starter zip or you've forked/cloned the <a href="https://github.com/stackmob/stackmob-javascript-examples" target="_blank">JS Examples GitHub repo</a>.  You'll get the HTML files and also the respective version of the StackMob JS SDK that works with these projects.

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

