---
description: This is a brief explanation on how to use our Users API
---

# Users API

{% api-method method="get" host="https://soldier-bot.herokuapp.com" path="/users/:userId" %}
{% api-method-summary %}
Get User info
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get the Roblox account bound to a ceratin discord user ID
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="userId" type="number" required=true %}
Discord ID of the user
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
The user ID was found in the database
{% endapi-method-response-example-description %}

```
{ "status": "ok", "userId": "discordId", "robloxUsername": "username",    "robloxId": "id" }
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a user matching that ID
{% endapi-method-response-example-description %}

```
{ "status": "error", "errorCode": 404, "errorMessage": "User not found" }
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



