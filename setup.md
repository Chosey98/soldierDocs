# Setup

## Setting Up

To start setting up the discord bot, you must write out the command:

```
s!setup
```

The bot then will ask you for the following stuff in order: 

1. The server type which you can choose between these three: 1. **Requests:** Handle rank requests by having people with ranking access permissions accepting/declining the requests 2. **Manual:** Rank the user directly through a single line command if you have the ranking access permissions role\(s\) 3. **Moderation:** Set up the server for simple moderation

{% hint style="info" %}
If you chose`Moderation`you can skip the following steps. If you don't you can still have moderation commands on/off in the next step
{% endhint %}

    2. Whether you want moderation commands enabled or not.

    3. The Roblox group ID must be a valid group and bound to one server only in this case the one you are setting up.

{% hint style="info" %}
If you are having any problems like the group is being bound to another server and you are the owner of the group file a ticket at the [Support server](https://discord.gg/WZUfAMS) and we would be glad to assist you immediately.
{% endhint %}

     4. The roles that you want them to have ranking access permissions.  
     5. The roles that you want them to have rank requesters permissions. \(Only if  
     the server type is set to `requests`\)  
     6. The channel you want to receive the promotion requests in \(Only if the server type is set to `requests`\)  
     7. The channel you want to receive the promotion-logs in \(Only if the server type is set to `requests`\)

After that, you confirm your settings and you are ready to go.

{% hint style="info" %}
If you are setting the server up as an army or a regiment/group, please open up a ticket in our [support server](https://discord.gg/WZUfAMS) so that we can add the bot to your group.
{% endhint %}

### Additional channels

* If you have a channel named `soldier-logs` then the bot will log everything to there

### Re-setup

If you want to re-setup your server you can use:

```text
s!resetup
```

