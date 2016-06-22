# ACJIRA-959

See: https://ecosystem.atlassian.net/browse/ACJIRA-959

# How to run

* Install dependencies: `npm install`
* Start ngrok: `ngrok http 3000`
* Start a the server: `node app.js`
* Add your ngrok url in the `atlassian-connect.json` file (3x).

# Verify Bug

The add-on creates an global permission named 'ACJIRA-959 Global Permission' and adds an menu item to the system nav bar that will show a general page.

A user without the 'ACJIRA-959 Global Permission' will not see the menu item. If this user is given the global permission though the system administration, the menu item will show. When the item is clicked the user will be directed to a page 'You do not have the correct permissions to view the page Hello World'.
