---
order: 150
icon: dot-fill
label: Moderation
author:
  name: Robbe
  avatar: https://cdn.discordapp.com/attachments/1034201179716079777/1084940308686589992/Robbe.png
tags: [intro]
---
### Let's talk about moderation!
At Beemo, we've got your back when it comes to handling problematic users. Our moderation tools are top-notch and can help you manage any issues that come up. Let's take a closer look at how they work, shall we?

First up, you'll want to explore the tabs below. They're packed with all sorts of useful information that will make moderation a breeze. We've designed our moderation tools to be easy to use and understand, so you won't have to worry about any complicated setup or confusing settings.

---

#### Moderation Commands

First up, we have the archive command. It creates a message archive for the specified user that expires after 12 hours. However, archives cannot be generated for moderators or admins to ensure messages in private channels stay protected. `/archive 515067662028636170`

Next, the avatar command can be used to get the avatar of a specified user. `/avatar 515067662028636170`

The ban command is used to ban a user, deleting their past 7 days of messages and notifying them through DMs. If you don't specify a duration, the ban will be set to permanent. `/ban 515067662028636170 7d Spam`

The cleankick command kicks the user and deletes their past 7 days of messages, notifying them through DMs and logging the incident. `/cleankick 515067662028636170 Spam`

If you need to edit the duration of an existing moderation case, use the duration command. You can only edit your own cases unless you are a moderation manager. `/duration 14 4d`

To kick a user, use the kick command. It notifies the user through DMs and logs the incident. `/kick 515067662028636170 Spam`

The modlogs command shows all moderation logs for a user, including a link to each case's action log and message archive. `/modlogs 515067662028636170`

You can add a mod note onto a user's logs using the modnote command. This note is only visible to moderators, and does not DM the user or show when the user types /mylogs. `/modnote 515067662028636170 Spam`

To get statistics of a specified moderator, use the modstats command. You can optionally specify a before and/or after date to get stats for specific time periods. You must be a moderation manager or admin to use this command. `/modstats 515067662028636170 before:2021/01/01 after:2020/01/01`

The mute command mutes the user, notifying them through DMs when the mute begins and ends and logging the incident. If you don't specify a duration, the mute will be set to permanent. `/mute 515067662028636170 3h Spam`

The presetreasons command lists all available preset reason variables for the server. If a preset variable is specified, this command will list the correlated preset reason. `/presetreasons spamming`

If you need to mass-delete messages in the channel invoked, use the purge command. You must be a moderation manager or admin to use this command. `/purge 400`

To edit the reason of an existing moderation case, use the reason command. You may only edit your own cases unless you are a moderation manager or admin. `/reason 14 Advertising`

The revoke command revokes the specified moderation case, preventing it from showing on /modlogs. You may only revoke your own cases unless you are a moderation manager or admin. `/revoke 14 Appealed`

The revokeall command revokes all cases tied to a user, preventing them from showing up on their moderation logs. You must be a moderation manager or admin to use this command. `/revokeall 515067662028636170 Appealed`

The saveban command is the same as /ban, except the user's messages are not deleted. `/saveban 515067662028636170 2d Advertising`

To unban a user, use the unban command. It attempts to DM the user and logs the incident. `/unban 515067662028636170 Reformed`

The unmute command unmutes the user, notifying them through DMs and logging the incident. `/unmute 515067662028636170 Reformed`

The userinfo command gets information regarding a user in the server, such as account age, join date, join position, and roles. `/userinfo 5150676620286361`

Finally, To warn a user, use the warn command. This will send a DM to the user notifying them of the warning and will log the incident for future reference. `/warn 515067662028636170 Spam`

---

### Archives
Are you curious about how archives work? They're a great feature that allows moderators like you to easily browse through a user's message history, including any edits or deleted messages. This makes it easier to keep track of what's been said and make sure everything stays on track. So, let's dive in and learn more about archives!

#### Making Archives
Let's take a look at the different ways archives can be generated with Beemo:

- Manually Generated

If you're a moderator, you can manually generate an archive for a user by running the command /archive [user]. This will grant you access to an archive that contains the user's message history from the past 3 days. Just keep in mind that manually generated archives expire 12 hours after the command execution.

!!!warning Important Note
Moderators or administrators cannot manually generate archives. This is to ensure that messages from private mod or admin channels are not exposed.
!!!

- Automatically Generated

Whenever a moderation command is run that targets a user (such as a ban), all of the user's messages (including edits and deletions) will be archived and attached to the case. These archives serve as a snapshot of the past 3 days of a user's message history and will not expire for the purpose of moderation log persistence.

If you want to check info on a case, simply run the command `/case <case id>` or `/modlogs <user id>` and the case-specific archive links will be displayed.

!!! Keep in mind
One thing to keep in mind is that when a user types `/mylogs`, they will not see the archives for their cases.
!!!

---

### Preset Reasons
With Preset Reasons, you can store pre-written messages that your moderators can use when they need to take the same moderation action multiple times. This saves them from having to write out the same message every time, which can be a real time-saver!

So, next time you need to take a redundant moderation action, just select the preset reason that fits the situation and hit send. Easy, right?

#### About
With Preset Reasons, you can use pre-made flags for reasons that come up frequently, kind of like canned responses for moderators.

This feature is especially useful for those reasons that tend to come up again and again, so you don't have to type out the same thing every time.

#### Configuring Preset Reasons
First, it's important to note that you'll need to have the Administrator permission or be a Moderation Manager to configure preset reasons.

To manage your presets, you can use the following commands: to set a new preset reason, just type `/mod presetreason [preset name] (reason)`. If you want to remove a preset reason, just type `/mod presetreason [preset name]` without a reason.

Once you've added your preset reasons, all moderators in your server can use them by simply typing `-reasonhere` as their reason. It's that easy!

If you want to view all of the available preset reasons, just type `/presetreasons`. And if you want to see a specific reason, you can do `/presetreasons -reasonhere`.

Using preset reasons in moderation commands is easy too! Just put `-reasonhere` as your reason at the end of the moderation command, and Beemo will automatically take action with that reason. You can also use the `/edit (case id) -presetreasonhere` command to apply a preset reason to an existing case.

