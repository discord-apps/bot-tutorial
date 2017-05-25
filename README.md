# Official Discord API

## Contents
1. Introduction
<br/>a) What can an application do?
2. How to create an application


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
