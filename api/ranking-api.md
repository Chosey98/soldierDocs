---
description: Brief description on how to use the Ranking API.
---

# Ranking API

{% swagger baseUrl="https://api.soldier.gq" path="/ranking/rank" method="post" summary="Set rank" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="header" name="apikey" type="string" %}
API key for the server which can be obtained by the owner from the dashboard on our website.
{% endswagger-parameter %}

{% swagger-parameter in="body" name="authorId" type="number" %}
The author Roblox Id ranking the user.
{% endswagger-parameter %}

{% swagger-parameter in="body" name="userId" type="string" %}
The userId of the user being ranked.
{% endswagger-parameter %}

{% swagger-parameter in="body" name="rank" type="string" %}
The rank name or id to rank the user.
{% endswagger-parameter %}

{% swagger-response status="200" description="Cake successfully retrieved." %}
```
{    "name": "Cake's name",    "recipe": "Cake's recipe name",    "cake": "Binary cake"}
```
{% endswagger-response %}

{% swagger-response status="404" description="Could not find a cake matching this query." %}
```
{    "message": "Ain't no cake like that."}
```
{% endswagger-response %}
{% endswagger %}

