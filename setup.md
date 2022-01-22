---
description: This page will describe how to properly setup your server with Soldier.
---

# Setup

## Setting Up

To initiate the setup process, type the command below.

```
s!setup
```

Once you have typed the setup command, you will be prompted to answer the following questions:

1. What module you would like the server to be setup in?
2. **Roblox** This module enables options for group management, and user promotions and demotions. (Recommended option)
3. **Moderation** This module is meant for servers who only require moderation commands from our bot. It has no group management options.

{% hint style="info" %}
If you choose the **Moderation** module, you will skip the following steps and the setup process would be completed. (You can still enable moderation commands if you chose the **Roblox** module.
{% endhint %}

1. Whether you would like Moderation commands to be enabled.\
   Enabling this setting will allow moderation commands to be enabled in your server.
2. What is your Roblox Group ID?\
   Enter your Roblox Group ID for the group that you would like Soldier to be bound in. Entering an invalid Group ID will cause the setup to end.

{% hint style="warning" %}
Please do not bound groups that you do not own.\
This will cause unnecessary trouble for our team, and will result in your server being unbounded. If you're group has been bounded to another server, tell our [Support Team](https://discord.gg/KaSN7gnpkp).
{% endhint %}

1. Set who can rank members.\
   Members with this role are able to use the `s!promote / s!demote` command. They are also able to accept/decline ranking requests if the setting is enabled.
2. Set if ranking requests are enabled.\
   This setting determines whether ranking requests should be enabled, this opens up the opportunity for members with the ranking access role to be able to accept/decline requests sent from the `s!rank` command.
3. Set who can send a rank request.\
   Members with this role are able to use the `s!rank` command to send a rank request for anyone with a ranking access role to accept/decline.
4. Set where promotion requests should be sent at.\
   This setting determines where promotion requests should be sent at for members with a ranking access role to accept/decline.
5. Set where Soldier logs should be sent.\
   This setting determines where Soldier's logs should be placed.

Once you have completed these steps and confirmed the settings, your server's setup willl be completed.

{% hint style="info" %}
If you have chosen the Roblox module, you will need to send a request in our [Discord Server](https://discord.gg/hdm87pRgrb) for Soldier to be able to rank users accordingly.
{% endhint %}

### Additional Information

* If you chose not to enable ranking requests, but want to have Soldier logs, create a channel named `soldier-logs`. Once this channel is created, all new events will log to that channel as it normally would with ranking requests enabled.

### Re-Setup

If you need to change modules or enable/disable a setup setting, you can use the command below to re-setup your discord server with Soldier.

```
s!resetup
```
