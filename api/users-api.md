---
description: This is a brief explanation on how to use our Users API
---

# Users API

{% api-method method="get" host="https://soldier-bot.herokuapp.com" path="/users/roblox/:robloxId" %}
{% api-method-summary %}
Get User info using his Roblox ID
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get the user info of the user in our database using his roblox id. Such as the discord ID bound to him.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="robloxId" type="number" required=true %}
Roblox ID of the user
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
The user ID was found in the database
{% endapi-method-response-example-description %}

```
{ "status": "ok", "userId": "discordId", "robloxUsername": "username", "robloxId": "id" }
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a user matching that ID in that database
{% endapi-method-response-example-description %}

```
{ "status": "error", "errorCode": 404, "errorMessage": "User not found" }
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://soldier-bot.herokuapp.com" path="/users/rUsername/:robloxUsername" %}
{% api-method-summary %}
Get User info using his Roblox username
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get the user info of the user in our database using his roblox username. Such as his discord ID bound to him.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="robloxUsername" type="string" required=true %}
Roblox username of the user
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
The user was found successfully.
{% endapi-method-response-example-description %}

```
{ "status": "ok", "userId": "discordId", "robloxUsername": "username", "robloxId": "id" }
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
No user was found with this username.
{% endapi-method-response-example-description %}

```
{ "status": "error", "errorCode": 404, "errorMessage": "User not found" }
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://soldier-bot.herokuapp.com" path="/users/discord/:userId" %}
{% api-method-summary %}
Get user info using his Discord ID
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get the user info using his discord ID. Such as his roblox account bound to his discord ID
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="userId" type="number" required=true %}
Th
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
The user was found successfully.
{% endapi-method-response-example-description %}

```
{ "status": "ok", "userId": "discordId", "robloxUsername": "username", "robloxId": "id" }
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
No user was found with that discord ID.
{% endapi-method-response-example-description %}

```
{ "status": "error", "errorCode": 404, "errorMessage": "User not found" }
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

