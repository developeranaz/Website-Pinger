# Website-Pinger
Website pinger is a free pinger by using free google script(gs). 
You can ping your website whenever you want whether it is day based, month based, time based, hourly based or minute based.
This will also gives a clean overview about analytics errors for your website.




### Requirements
* A free google account 

## How to use
* sign in to a google account
* Go to https://script.google.com
* Click `a new project` , You can rename default name `Untitled project` to whatever you like.
* Then in code editor remove all existing codes and paste the below code replaced with your own website.

```
function ping() {
var pingurl='https://last-bird.herokuapp.com'
var response = UrlFetchApp.fetch(pingurl);
Logger.log(response.getContentText());
}

```

* Then click on save button to save the project
* After saving, a `RUN` button appears 
* click on `Run` button
Review Permissions > Click `YOUR GOOGLE ACCOUNT` > If it shows `Google hasn’t verified this app` > Then click `Advanced` > `Go to Untitled project (unsafe)` > `Allow`
* After above step your project has permission to run gs.
* Run Trigger script to configure When you need to ping your URL or website
### Trigger
* After doing above step on left menu you can see trigger option > click it
* Then on Botton Right Corner You can see `Add Trigger` Button > click it
* Then set `Select event source`, `Select type of time based trigger` & `Select hour interval` as per you needs and save it. 

