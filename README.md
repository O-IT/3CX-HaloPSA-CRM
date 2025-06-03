# 3CX-HaloPSA-CRM

Using the 3CX CRM Integration Templates to have lookup and link to Halo PSA.
With the help from the Halo PSA knowledgebase and some great help from the discord community i created this simple to use template.

# Features

- Phone lookup and One Click to Halo

# Setup

## Halo

Add a new Halo API Application with the Auth-Code type.
You need to add the redirect url 'https://your3cxname.3cx.de/api/oauth2crm'.
For better security you can add the CORS or your 3CX like: https://your3cxname.3cx.de/

## 3CX

Go to 3CX Admin Portal. Add the `HaloPSATemplate.xml` in integrations and fill out the form.

| Parameter | Example | Info |
| - | - | - |
| IntanceUrl | somewhere.halopsa.com | Just your plain domain. It is possible to use a customer port with yoururl:8111 |
| ClientId | The Client id generated from Halo PSA |  |
| ClientSecret | The Secret generated from Halo PSA |  |
| Scope | all | You can change that depending on your needs |
| RefreshToken | Click on Authorize and follow the login |  |
| ContactUrlFragment | customers?userid= | The instance Url will be prefixed and the matched halo contactid will be attached at the end. |