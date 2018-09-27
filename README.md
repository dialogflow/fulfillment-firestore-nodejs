# Dialogflow Firestore Sample
+ This sample demonstrates how to connect Dialogflow to the Firestore database.
+ Dialogflow parses users' requests and sends requests to Firebase function indicating whether it should add or retrieve an entry from the Firestore database. The Firebase function queries the database to add or retrieve the entry and then compiles the proper response to the user. You can speak to your Dialogflow agent and tell it to write something to the database or retrieve it.
+ The sample will save what you tell it to save into the database as well as retrieve the value you store previously.
+ When you speak to your Dialogflow agent a webhook call is sent to Firebase functions which talks to the Firestore database to retrieve or add a entry as see below:

This sample is meant to be a starting point for anyone looking to connect a database to their Dialogflow agent and can be expanded to store users preferences, retrieve relevant data from your systems or enable your users to collaborate via chat/voice.

```
Dialogflow → Webhook Request → Firebase Function → Firestore Database
```

## Setup

### Dialogflow and Fulfillment Setup
To create this agent from our template:

<a href="https://console.dialogflow.com/api-client/oneclick?templateUrl=https://oneclickgithub.appspot.com/dialogflow/fulfillment-firestore-nodejs" target="blank">
  <img src="https://dialogflow.com/images/deploy.png">
</a>

### Firestore Setup
1. In Dialogflow's console, in the left menu > go to **Fulfillment** > **Enable Inline Editor** > **Deploy**.
2. At the bottom, go to **View execution logs in the Firebase console**.
3. In the Firebase console, go to **Database** > **Create database**.
4. Select **Start in locked mode** > **Enable**.

## Running the sample
1. In [Dialogflow's console](https://console.dialogflow.com), in the Dialogflow simulator on the right, query your Dialogflow agent with `Write Buzz Aldrin to the database` and then query `What's in the database?` to get the response "Buzz Aldrin". 

## Related Samples
| Name       | Language           |
| ------------- |:-------------:|
| [Fulfillment & Regex Validation](https://github.com/dialogflow/fulfillment-regex-nodejs)      | Node.js |
| [Weather: Fulfillment & WWO API](https://github.com/dialogflow/fulfillment-weather-nodejs)     | Node.js      |  
| [Bike Shop: Fulfillment & Google Calendar API](https://github.com/dialogflow/fulfillment-bike-shop-nodejs)| Node.js |
| [Temperature Trivia: Fulfillment & Actions on Google](https://github.com/dialogflow/fulfillment-temperature-converter-nodejs) | Node.js |
| [Fulfillment & Actions on Google](https://github.com/dialogflow/fulfillment-actions-library-nodejs) | Node.js |
| [Fulfillment & Firestore Database](https://github.com/dialogflow/fulfillment-firestore-nodejs) | Node.js |
| [Multi-language/locale](https://github.com/dialogflow/fulfillment-multi-locale-nodejs) | Node.js |
| [Basic Slot Filling](https://github.com/dialogflow/fulfillment-slot-filling-nodejs) | Node.js |

For Fulfillment Webhook [JSON Requests & Responses](https://github.com/dialogflow/fulfillment-webhook-json).

## References & Issues
+ Questions? Try [StackOverflow](https://stackoverflow.com/questions/tagged/dialogflow) or [Dialogflow Developer Community](https://plus.google.com/communities/103318168784860581977).
+ Find a bug? Report it on [GitHub](https://github.com/dialogflow/fulfillment-webhook-json/issues).
+ Dialogflow [Documentation](https://dialogflow.com/docs/getting-started/basics).
+ [Dialogflow's console](https://console.dialogflow.com).

## How to make contributions?
Please read and follow the steps in the CONTRIBUTING.md.

## License
See [LICENSE](LICENSE).

## Terms
Your use of this sample is subject to, and by using or downloading the sample files you agree to comply with, the [Google APIs Terms of Service](https://developers.google.com/terms/).
