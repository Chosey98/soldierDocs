---
description: This page describes what the "rank" command does.
---

# Rank

## Usage

This command is used to send a ranking request for users with a ranking access role to accept.  
Usage:

```text
s!rank
```

Once this command is executed, a DM prompt will be initiated with the user who typed the command and Soldier,  this DM prompt will ask you for:

* The username of the person who want to promote / demote.
* What rank you wish to rank the user to.
* The reason for the request.

Once this request has been completed, the request will be sent to the promotion requests channel that was specified in setup.

{% hint style="info" %}
This is only available to user's with the request system enabled.
{% endhint %}

## Permissions

Only members with a `Rank Requester` role are able to use this command.

