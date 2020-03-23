---
layout: default
title: Glossary
nav_order: 7
permalink: /docs/glossary
---


App Key === API Key === Consumer API Key === Consumer Key === Customer Key === oauth_consumer_key
App Key Secret === API Secret Key === Consumer Secret === Consumer Key === Customer Key === oauth_consumer_secret
Callback URL === oauth_callback
 
Temporary credentials:

Request Token === oauth_token
Request Token Secret === oauth_token_secret
oauth_verifier
 
Token credentials:

Access token === Token === resulting oauth_token
Access token secret === Token Secret === resulting oauth_token_secret



# Setting up our OAuth 1.0

## What is OAuth?
OAuth is an standard for for authentication. The standard allows developers to provide user authentication, through API's. OAuth has many different workflows. The OAuth provider, in our case Twitter, will indicate the workflow that the developers will use. Though Twitter supplies developers with a set of workflows, the one that matches our intentions and needs is the 3-legged OAuth.

### 3-legged OAuth
With 3 legged OAuth, we will make several requests to Twitter's endpoints, in order to gain an access token that will authorize us to get the users' data from twitter. We will, first, redirect the user to a URL that Twitter's given us, along with our app's API Key and API Secret Key. This will tell twitter that the user is coming from our app, not any other source. As soon as the user logs in and authorizes our app to access their information, Twitter will send them back, with a code, that can be used to fetch an access token from Twitter. The recieved access token, will grant us access to the users' information, by sening requests, to certian end-points.
***
## Redirecting the user to Twitter
It's time to get back to writing our application. This time, though, we will be completing our app, so that it can communicate with the API.
    