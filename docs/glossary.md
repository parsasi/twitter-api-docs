---
layout: default
title: Glossary
nav_order: 7
permalink: /docs/glossary
---
# Glossary

This sections is dedicated to explaining the terminalogy that might be unfamiliar to you.

## API Terminalogy
Throughout the documentation, some terms are being using interchangably, regarding the API.

**App Key** is the key with which Twitter recognizes our app.API Key, Consumer API Key, Consumer Key, Customer Key and OAuth Consumer Key will refer to the same consept.

**App Key Secret** is the "password" for our app, in order to connect with the API. App Key Secret is often refered to as API Secret Key, Consumer Secret, Consumer Key, Customer Key or OAuth Consumer Key.

**Callback URL** is the URL that Twitter will use, to send the user back to, after authentication. Since we don't integerate OAuth 1.0 in our app, this will not be relevant to our app.
 
**Access token** will tell Twitter which user we are trying to access. We will user the words Token and OAuth Token for the same concept.

**Access token secret** will indicate wether or not our app should be able to access that specific users data. It will be called Token Secret or OAuth Token Secret.


## OAuth


**OAuth** is an standard for for authentication. OAuth standard allows developers to provide user authentication, through API's. It has many different workflows. The OAuth provider will indicate the workflow that the developers will use.

**3-legged OAuth** is done by making several requests to the provider's endpoints. The requests are done sequentially to get a request token a OAuth Access Token and a User Access Token.

