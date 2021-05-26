---
description: Brief description on how to use the Ranking API.
---

# Ranking API

{% api-method method="post" host="https://api.soldier-bot.tk" path="/ranking/rank" %}
{% api-method-summary %}
Set rank
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get free cakes.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="apikey" type="string" required=true %}
API key for the server which can be obtained by the owner from the dashboard on our website.
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-body-parameters %}
{% api-method-parameter name="authorId" type="number" required=true %}
The author Roblox Id ranking the user.
{% endapi-method-parameter %}

{% api-method-parameter name="userId" type="string" required=true %}
The userId of the user being ranked.
{% endapi-method-parameter %}

{% api-method-parameter name="rank" type="string" required=true %}
The rank name or id to rank the user.
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```
{    "name": "Cake's name",    "recipe": "Cake's recipe name",    "cake": "Binary cake"}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```
{    "message": "Ain't no cake like that."}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



