---
description: This is a brief explanation on how to use our Users API
---

# Users API

{% swagger baseUrl="https://api.soldier.gq" path="/users/roblox/robloxId/:robloxId" method="get" summary="Get User info using his Roblox ID" %}
{% swagger-description %}
This endpoint allows you to get the user info of the user in our database using the user's Roblox ID.
{% endswagger-description %}

{% swagger-parameter in="path" name="robloxId" type="number" %}
Roblox ID of the user
{% endswagger-parameter %}

{% swagger-response status="200" description="The user ID was found in the database" %}
```
{ "status": "ok", "userId": "discordId", "robloxUsername": "username", "robloxId": "id" }
```
{% endswagger-response %}

{% swagger-response status="404" description="Could not find a user matching that ID in that database" %}
```
{ "status": "error", "errorCode": 404, "errorMessage": "User not found" }
```
{% endswagger-response %}
{% endswagger %}

{% swagger baseUrl="https://api.soldier.gq" path="/users/roblox/robloxUsername/:robloxUsername" method="get" summary="Get User info using his Roblox username" %}
{% swagger-description %}
This endpoint allows you to get the user info of the user in our database using the user's Roblox username.
{% endswagger-description %}

{% swagger-parameter in="path" name="robloxUsername" type="string" %}
Roblox username of the user
{% endswagger-parameter %}

{% swagger-response status="200" description="The user was found successfully." %}
```
{ "status": "ok", "userId": "discordId", "robloxUsername": "username", "robloxId": "id" }
```
{% endswagger-response %}

{% swagger-response status="404" description="No user was found with this username." %}
```
{ "status": "error", "errorCode": 404, "errorMessage": "User not found" }
```
{% endswagger-response %}
{% endswagger %}

{% swagger baseUrl="https://api.soldier.gq" path="/users/discord/userId/:userId" method="get" summary="Get user info using his Discord ID" %}
{% swagger-description %}
This endpoint allows you to get the user info bound to the user's discord ID.
{% endswagger-description %}

{% swagger-parameter in="path" name="userId" type="number" %}
The user discord Id
{% endswagger-parameter %}

{% swagger-response status="200" description="The user was found successfully." %}
```
{ "status": "ok", "userId": "discordId", "robloxUsername": "username", "robloxId": "id" }
```
{% endswagger-response %}

{% swagger-response status="404" description="No user was found with that discord ID." %}
```
{ "status": "error", "errorCode": 404, "errorMessage": "User not found" }
```
{% endswagger-response %}
{% endswagger %}
