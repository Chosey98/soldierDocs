---
description: This page describes what the "purge" command does.
---

# Purge

## Usage

This command is used to delete a set number of messages in a channel.  
Usage:

{% tabs %}
{% tab title="Purge" %}
```text
s!purge <number of messages>
```
{% endtab %}

{% tab title="Delete" %}
```
s!delete <number of messages>
```
{% endtab %}

{% tab title="Clear" %}
```
s!clear <number of messages>
```
{% endtab %}
{% endtabs %}

Once this command is executed, the number of messages specified in the command will be deleted in that channel.

{% hint style="info" %}
Messages in a channel for longer than 2 weeks cannot be purged.
{% endhint %}

## Permissions

Only members with the  `Manage Messages` permission are able to use this command.

