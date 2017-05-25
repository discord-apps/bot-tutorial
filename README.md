# Official Discord API

## Contents
1. [Introduction](https://github.com/discord-apps/tutorial/blob/master/README.md#introduction)
<br/>a) [What can an application do?](https://github.com/discord-apps/tutorial#what-can-an-application-do)
2. [How to create an application](https://github.com/discord-apps/tutorial#how-to-create-an-application)
3. [Non-Bot Applications](https://github.com/discord-apps/tutorial#how-to-create-an-application)
<br/>a) [User Bots](https://github.com/discord-apps/tutorial#user-bots)
<br/>b) [Self-Bots](https://github.com/discord-apps/tutorial#self-bots)
<br/>b) [Client ID and Token of a User](https://github.com/discord-apps/tutorial#client-id-and-token-of-a-user)

## Introduction
[Discord](https://www.discordapp.com/) allows you to create applications using their [OAuth2](https://www.discordapp.com/developers/docs/topics/oauth2) login socket and their [API](https://discordapp.com/developers/docs/intro) ([Application Programming Interface](https://en.wikipedia.org/wiki/Application_programming_interface)). This is useful to create messaging channels, storing data, creating login-services and interacting with people using the Discord Application, providing utilities and entertainment. The Discord API is documented on the <em>discord docs</em>, which may be found [here](https://www.discordapp.com/developers).

### What can an application do?

* Use your Discord account to safely login to your guild's website
* Display who’s online or in-game on your website or forum
* Automatically join private Discord servers or gain new roles based on external website permissions
* Other neat things.

## How to create an application
Creating an application is easy, simply follow these steps:
1. [Login](https://www.discordapp.com/login) on to Discord an visit the [Developer page](https://discordapp.com/developers).
2. Click on <strong><em>My Apps</em></strong> (navigation bar on the left), then click on <strong><em>New App</strong></em> (or follow [this link](https://discordapp.com/developers/applications/me/create)).
3. Choose a name that will identify the application and a description (optional). The name you type now will be the name of the bot. You will be able to change the application's name at any time, but it will not update the bot's username. To do this, you will need to make the bot request a name change from inside your application.
4. Once you have filled in the fields, click on <strong><em>Create App</strong></em>. Then, click on <strong><em>Create Bot User</strong></em>. Here you will be able to change the settings, set an avatar (<strong><em>App Icon</strong></em>). Once you're done, hit <strong><em>Save Changes</strong></em>.
5. There will be two relevant pieces of information which your application will need to function properly. The first is the <em>Client ID</em>, which will be located at the top of application settings. It will also be the number in the URL:
> <em>https://discordapp.com/developers/applications/me/[App-ID]</em>
6. The second string you need is the <em>Token</em> - Keep in mind this is sensitive information that will give anyone access to your bot. Thus, make sure <strong>not to share it with anyone you do not trust!</strong> The token is used to allow the application to login with the bot's account. Both the Client ID and the Token are unique numbers. If the token is compromised, you may generate a new one by clicking <strong><em>Generate a new token?</strong></em> (The token must be visible for the button to appear.

Now you have successfully created a Discord Bot.

## Non-Bot Applications
It is also possible to create user-bots and self-bots. While the two are often confused, there is a significant difference.

### User Bots
User Bots are User-Accounts that serve as bots. This is actually easier to do than creating a Bot account, as you only have to register normally and retrieve your login token. However, this would circumvent the key-limitation of a Bot-Account: joining guilds. Users do not require an invite link to join a guild, thus you would be able to load a bot on another guild without the owner's permission. Discord calls this <strong>API abuse</strong> (as you are miusing their API to do something it was not designed for) and is, thus, <strong>not allowed</strong>.

### Self-Bots
Self-Bots, on the other hand, are bots running on a user account, however they do not react to normal users: only the account which is currently logged in (aka the account they are being ran on) is able to interact with them. As long as the purpose of a self-bot is using [Embedded messages](http://imgur.com/a/yOb5n) or just adding custom emojis along with other utilities, it is allowed. Spam-Bots are <strong>NOT</strong> allowed and your account may be terminated if you are reported while doing so.

### Client ID and Token of a User
To get the <strong><em>Client ID</strong></em>, you need to go to the Settings and enable Developer mode, which is a useful setting that allows you to see user, guild, channel or message IDs:

<img src="http://i.imgur.com/P8qV3Tb.png"/>

Then, right click on your username on any message you sent, an @<em>mention</em> or user-list on the right and click on <strong><em>Copy ID</strong></em>.

Next, you will want to open the <em>Inspector Mode</em> on the desktop or the web client, visit <strong><em>Application</strong></em> (at the top), <strong><em>Local Storage</strong></em> (left) and click on <em>https://discordapp.com</em> if you are using the normal version and <em>https://canary.discordapp.com</em> if you are using the canary version. The last element of the table is called "token". That is your login token (without the double quotes). Again, it is <strong>VERY IMPORTANT NOT TO SHARE IT WITH ANYONE YOU DO NOT TRUST WITH YOUR ACCOUNT!</strong> Who has your token is able to:
* Send messages with your account,
* Interact with other users with your account,
* Perform administrator actions on Guilds you are an Administrator on,
* Change your Email address,
* Change your Username (and your login token!),
* Change your Password
* and much more.
