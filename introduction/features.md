---
order: 100
icon: dot-fill
label: Utility
author:
  name: Robbe
  avatar: https://cdn.discordapp.com/attachments/1034201179716079777/1084940308686589992/Robbe.png
tags: [intro]
---
### Utility
Get the most out of our product, including integrated XP and consumable-credit role-shops based on activity (we call them honey).
To get started, just check out the tabs below to see how Beemo can help you.

---

### Honey
our consumable credits system that lets you purchase roles! With Honey, you'll be able to easily manage your credits and enjoy all the perks that come with your new roles.

#### About Honey
With Honey, you can reward activity on your server with credits that users can later trade in for role rewards. These credits, called “Honey,” are earned at the same rate as XP. This means that users can spend their Honey without affecting their XP level. Pretty cool, right?

There are so many ways you can use this system! For example, you could allow active users to claim exclusive color roles as a reward for their activity. The possibilities are endless!

#### Commands
irst up, we have the honey command. You can use this command to enable or disable the honey system. For example, if you want to disable the honey system, simply type "/honey disable".

Next, we have the honey shop role command. This command allows you to set or remove a role as a honey shop role for purchase via the /honey shop command. To use this command, you'll need to specify the role's ID or mention, the cost in honey, and an optional description. For example, "/honey shop role 12345678 23 Purchase this honeycomb!".

If you need to reset a user's honey on the server, you can use the honey reset command. Simply specify the user's mention or role name/id after the command. For example, "/honey reset @Ayu" will reset Ayu's honey on the server. If you want to reset the honey for all users, use the "all" keyword. For example, "/honey reset all" will reset the server's honey.

Lastly, we have the honey set command. This command allows you to set a user's honey to a new amount. Just use the user mention or ID, and specify the new honey amount. For example, /honey set @Ayu 69.

---

### XP
As you participate in text and voice channels, you'll gain experience and level up. It's a fun and easy way to track your progress and see how you're doing compared to other members.

#### About XP
Users can level up through both text and voice channels, and even customize their curves and role rewards. Plus, servers can add specific roles to be rewarded at different level milestones, which is pretty cool!

But that's not all – if you enable Honey alongside XP, users will also gain Honey at the same rate, which can be used in the Honey role shop.

#### Commands
The first command is `"xp [enable/disable]"`. You can use this command to enable or disable the XP system. Simple, right?

Next up is `"xp rolereward [level] [role name/id]`". With this command, you can add or remove a specified role as an XP role reward for the level you've specified. If you want to remove a role reward, you don't need to specify the role.

If you want to see what XP role rewards are currently set up for your server, use the "xp rolerewards" command.

Now let's talk about resetting XP. If you want to reset a specific user's XP, use the `"xp reset [user mention/role name/id]"` command. You can also reset all users' XP on the server by using `"xp reset all"`. If you want to reset all users with a specific role, specify the `role name/id`.

To set a user's XP to a specific amount, use the `"xp set [user mention/id] [new amount]"` command.

If you add or remove XP role rewards from the system, make sure to use the `"xp refreshroles"` command to refresh all of the user's XP role rewards.

You can set how often 1 XP / honey can be earned through text channels with the `"xp textcooldown [seconds]"` command, and how often 1 XP / honey can be earned through voice channels with the `"xp voicecooldown [seconds]"` command.

If you want to add or remove a specified role as an XP & Honey-blacklisted role, use the `"xp blacklistrole [role name/id]"` command.

To see what roles are currently XP and honey-blacklisted, use the `"xp blacklistedroles"` command.

If you want to add or remove a specified text or voice channel as an XP and honey-blacklisted channel, use the `"xp blacklistchannel [channel name/id]"` command.

To see what text and voice channels are currently XP and honey-blacklisted, use the "xp blacklistedchannels" command.

Now let's talk about XP and honey admin roles. You can add or remove a specified role as an XP and honey admin role with the `"xp adminrole [role name/id]"` command.

To see what roles are currently XP and honey admin roles, use the `"xp adminroles"` command.

If you want users to keep their previous XP roles when they reach the next role reward, use the `"xp keepxproles [yes/no]"` command.

If you want user XP / honey to be reset upon leaving the server, use the `"xp resetonleave [yes/no]"` command.

`/xp resetonban yes`: This sets whether your XP or honey should be reset upon being banned from the server. If you set it to "yes," your XP or honey will be reset upon being banned.

`/xp notifications no`: This sets whether a level up notification should be sent when you level up. If you set it to "no," you won't receive a level up notification.

`/xp notificationschannel #notify`: This sets the channel where you want to receive level up notifications. If you put "none" for the channel name, you'll remove a set channel. If you don't specify a channel, the notice will be sent to your DMs.

`/xp commandchannel #bot-commands`: This adds or removes the specified text channel as an allowed channel for XP and honey commands.

`/xp commandchannels`: This lists the current XP and honey command channels.

`/xp rankcommandcooldown 5`: This sets the cooldown in seconds for the `/rank` command.

`/xp difficulty 2.0:` This sets the difficulty of the XP system. This modifies the multiplier so that the amount of XP needed to reach the next level is either larger or smaller. IMPORTANT: This setting will change the XP curve, which will affect the current level of all users.

`/xp leveltoxpratio 1.5`: This modifies the exponent of the XP function, which changes the relationship between XP gained and level achieved. The curve is determined by the formula: XP = Difficulty * (Level)^(Level to XP Ratio) + 4. For example, a difficulty of 1.2 and a level to XP ratio of 3.1 will result in a curve of xp = 1.2 * level^3.1 + 4, which means that it requires xp xp to be acquired in order to reach level level.