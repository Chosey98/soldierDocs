# XP API

{% swagger baseUrl="https://api.soldier.gq" path="/xp/getXp/:robloxId" method="get" summary="Get XP" %}
{% swagger-description %}
This endpoint allows you to get the xp of a user.
{% endswagger-description %}

{% swagger-parameter in="path" name="robloxId" type="number" %}
Roblox ID of the user you want to get his xp
{% endswagger-parameter %}

{% swagger-parameter in="header" name="apikey" type="string" %}
API key for the server which can be obtained from our dashboard on our website
{% endswagger-parameter %}

{% swagger-response status="200" description="Incase of error the success will be false and there will be an error key which has the message of the error" %}
```
{ success: true, userId: robloxId, xp: amountofXp, nextRankId: theIdOfTheNextRank, nextRankXp: theXpOfTheNextRank}
```
{% endswagger-response %}
{% endswagger %}

{% swagger baseUrl="https://api.soldier.gq" path="/xp/addXp" method="post" summary="Add XP" %}
{% swagger-description %}
Adds xp to a user and ranks him if he has enough xp
{% endswagger-description %}

{% swagger-parameter in="header" name="apikey" type="string" %}
API key for the server which can be obtained from our dashboard on our website.
{% endswagger-parameter %}

{% swagger-parameter in="body" name="authorId" type="number" %}
The id of the author requesting to add xp
{% endswagger-parameter %}

{% swagger-parameter in="body" name="userId" type="number" %}
The id of the user being added xp to
{% endswagger-parameter %}

{% swagger-parameter in="body" name="xp" type="number" %}
The amount of xp to add
{% endswagger-parameter %}

{% swagger-response status="200" description="Incase of an error success will be false, and in case of promotion when adding xp the message will be 'xp added and promoted'" %}
```
{ success: true, message: 'xp added' }
```
{% endswagger-response %}
{% endswagger %}

{% swagger baseUrl="https://api.soldier.gq" path="/xp/removeXp" method="post" summary="Remove XP" %}
{% swagger-description %}
Removes xp to a user and ranks him if he has enough xp
{% endswagger-description %}

{% swagger-parameter in="header" name="apikey" type="string" %}
API key for the server which can be obtained from our dashboard on our website.
{% endswagger-parameter %}

{% swagger-parameter in="body" name="authorId" type="number" %}
The id of the author requesting to remove xp
{% endswagger-parameter %}

{% swagger-parameter in="body" name="userId" type="number" %}
The id of the user being removed xp from
{% endswagger-parameter %}

{% swagger-parameter in="body" name="xp" type="number" %}
The amount of xp to remove
{% endswagger-parameter %}

{% swagger-response status="200" description="Incase of an error success will be false, and in case of promotion when removing xp the message will be 'xp removed and demoted'" %}
```
{ success: true, message: 'xp removed' } 
```
{% endswagger-response %}
{% endswagger %}
