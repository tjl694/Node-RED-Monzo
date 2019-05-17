# Node-RED Monzo
Custom flows for use of the Monzo API within Node-RED


Using the Monzo Developer API this project will give various Node-RED flows to help achieve various things!

First step is to setup an application on the Monzo Dev portal - https://developers.monzo.com/apps/home. Here are some great instructions based on those from @muyiwaolu's [monzo-python](https://github.com/muyiwaolu/monzo-python#getting-oauth-credentials) project:

## Getting OAuth credentials
In order to get OAuth credentials for monzo-python:

1. Head to the Clients Section of the developer playground.
2. Click "New OAuth Client".
3. Give your client a name, e.g. "MyApplication".
4. Enter the "Redirect URL" as the 'localhost'
5. Select "Confidential" from the Confidentiality dropdown box.
6. Click "Submit" and make a note of the newly created client id and secret, you will need this for your Node-RED configuration.

## Getting the token
After adding the flow in [Get-Token](Get-Token.json), open up the first _function_ node and add in your Client ID and Secret to the variables at the start.
Initalise a Monzo login through the app you created earlier, go to your email, copy the link from the 'Login' button of the Monzo email and paste it within the Inject node.
Once that's done, deploy the flow and click the inject button on the inject node.
This will automatically keep refreshing your token. You'll only ever have to redo this if your Node-RED instance is stopped for whatever reason.

## TODO:
- [x] Setup project

### Flows to add:
- [x] [Get token](Get-Token.json)
- [ ] Get account/pot details
- [ ] Get balance
- [ ] Add leftover money to pot

### Docs to add:
- [x] [Add Developer App setup](#getting-oauth-credentials)
- [x] [Get token](#getting-the-token)
- [ ] Get account/pot details
- [ ] Get balance
- [ ] Add leftover money to pot
