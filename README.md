# Dialogflow Firestore Sample
This sample demonstrates how to connect Dialogflow to the Firestore database. Dialogflow parses user's requests and sends requests to Firebase function indicating whether it should add or retrieve an entry from the Firestore database. The Firebase function queries the database to add or retrieve the entry and then compiles the proper response to the user. You can speak to your Dialogflow agent and tell it to write something to the database or retrieve it. The sample will save what you tell it to save into the database as well as retrieve the value you store previously. When you speak to your Dialogflow agent a webhook call is sent to Firebase functions which talks to the Firestore database to retrieve or add a entry as see below:

```
Dialogflow → webhook request → Firebase function → Firestore
```

This sample is meant to be a starting point for anyone looking to connect a database to their Dialogflow agent and can be expanded to store users preferences, retrive relevent data from your systems or enable your users to collaborate via chat/voice.

## Setup Instructions

### Dialogflow and Fulfillment Setup
Click on the **Add to Dialogflow** button below and follow the prompts to create a new agent:

[![Firestore Sample](https://storage.googleapis.com/dialogflow-oneclick/deploy.svg "Firestore Sample")](https://console.dialogflow.com/api-client/oneclick?templateUrl=https://storage.googleapis.com/dialogflow-oneclick/dialogflow-agent-firestore.zip&agentName=FirestoreSample)

1. Click on the button above and click `Create agent`
1. After the creation is complete (this may take a few minutes) click `Open agent`

### Firestore Setup
1. Click on the ["Fulfillment" tab](https://console.dialogflow.com/api-client/#/agent//fulfillment) in your Dialogflow agent
1. Click on `View execution logs in the Firebase console` at the bottom of the fulfillment page to open the Firebase console
1. Click `Database` in the left panel of the Firebase console and click `Create database`
1. Select `Start in locked mode` and click `Enable`

## Running the sample
1. In [Dialogflow's console](https://console.dialogflow.com), in the Dialogflow simulator on the right, query your Dialogflow agent with `Write Bobby Tables to the database` and then query `What's in the database?` to get the response "Bobby Tables".  You can replace "Dialogflow rules" with any string in your query.

## How to make contributions?
Please read and follow the steps in the CONTRIBUTING.md.

## License
See [LICENSE](LICENSE).

## Terms
Your use of this sample is subject to, and by using or downloading the sample files you agree to comply with, the [Google APIs Terms of Service](https://developers.google.com/terms/).
