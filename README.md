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
