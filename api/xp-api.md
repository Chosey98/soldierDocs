# XP API

{% api-method method="get" host="https://api.soldier-bot.tk" path="/xp/getXp/:robloxId" %}
{% api-method-summary %}
Get XP
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get the xp of a user.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="robloxId" type="number" required=true %}
Roblox ID of the user you want to get his xp
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="apikey" type="string" required=true %}
API key for the server which can be obtained from our dashboard on our website
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Incase of error the success will be false and there will be an error key which has the message of the error
{% endapi-method-response-example-description %}

```
{ success: true, userId: robloxId, xp: amountofXp }
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://api.soldier-bot.tk" path="/xp/addXp" %}
{% api-method-summary %}
Add XP
{% endapi-method-summary %}

{% api-method-description %}
Adds xp to a user and ranks him if he has enough xp
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="apikey" type="string" required=true %}
API key for the server which can be obtained from our dashboard on our website.
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-body-parameters %}
{% api-method-parameter name="authorId" type="number" required=true %}
The id of the author requesting to add xp
{% endapi-method-parameter %}

{% api-method-parameter name="userId" type="number" required=true %}
The id of the user being added xp to
{% endapi-method-parameter %}

{% api-method-parameter name="xp" type="number" required=true %}
The amount of xp to add
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Incase of an error success will be false, and in case of promotion when adding xp the message will be 'xp added and promoted'
{% endapi-method-response-example-description %}

```
{ success: true, message: 'xp added' }
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://api.soldier-bot.tk" path="/xp/removeXp" %}
{% api-method-summary %}
Remove XP
{% endapi-method-summary %}

{% api-method-description %}
Removes xp to a user and ranks him if he has enough xp
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="apikey" type="string" required=true %}
API key for the server which can be obtained from our dashboard on our website.
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-body-parameters %}
{% api-method-parameter name="authorId" type="number" required=true %}
The id of the author requesting to remove xp
{% endapi-method-parameter %}

{% api-method-parameter name="userId" type="number" required=true %}
The id of the user being removed xp from
{% endapi-method-parameter %}

{% api-method-parameter name="xp" type="number" required=true %}
The amount of xp to remove
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Incase of an error success will be false, and in case of promotion when removing xp the message will be 'xp removed and demoted'
{% endapi-method-response-example-description %}

```
{ success: true, message: 'xp removed' } 
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://api.soldier-bot.tk" path="/xp/addXp" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="" type="string" required=false %}

{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
of an error success will be false, and in case of promotion when adding xp the message will be 'xp added and promoted'
{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

