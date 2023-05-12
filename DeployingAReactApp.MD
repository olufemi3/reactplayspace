#How to Deploy a React App on cPanel

##1. Update your package.JSON file 
There should be a **package.json** file in the root directory of your app. You need to add an **homepage** entry to it that specifies the final homepage of your app. 

Add the entry below to your package.json file. Remember to change the **https://domain.name** to your actual domain.

"homepage": "https://domain.name",


##2. Build the React App

Go to Terminal and navigate to the root folder of your app 

While in the root folder run the follow command: 

“npm run build” 

Use the ‘sudo’ to run this as admin in case your build fails without it. Like so: 

“sudo npm run build” 

**Note that you'll be prompted to enter your computer login password**

##3. Move your build folder to cPanel

After successfully running build there will be an updated (or new) folder in the root folder of your App called 'Build'.

Upload the contents of this folder to the Public_html directory in cPanel.

Now run your website to make sure it works. 

And voila you’re done!
