# workautomation-custom-uis

A selection of custom UIs for Genesys Cloud Work Automation

This is a place where I will continue to add examples of different WorkAutomation reports and views as examples only. These are seprated into their own dir in this repo.

To set them up and use them its the saem method as all my other client side repos and follows the format of my ![user snippets](https://github.com/mcphee11/vscode-user-snippets) for OAuth into the Genesys Cloud ORG.

## RealtimeView

The first example is a realtime view in the moment (doesn't refresh) of all the Worbins and the aggregates of the work types and sum of these items. As there is not a large multi select API right now I'm using a JOBS based API for each workbin so it does take some time to load but will then wrap it up in one view. I have excluded the `Terminated` & `Disconnected` items.

![](/docs/img/realtimeView.png?raw=true)

## Supervisor View

While there is already an existing supervisor view it doesn't allow fro across division access as well as the ability to `multi select` items. This view allows for that but id not recommend selecting 100s at a tiem as each update is its own individual PATCH request. This does make it much easier to multi select items and bulk assign them to a user.

![](/docs/img/listView.png?raw=true)
