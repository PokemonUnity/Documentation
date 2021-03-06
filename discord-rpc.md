# Discord RPC

Pokémon Unity supports integration with Discord Rich Presence, which displays your current map, follower, player name, and gender \(using an icon\).

Pokémon Unity uses a premade application for RPC by default, this guide will show you how to set up your own.

## Setting up an application

Firstly, sign up for [Discord](http://www.discordapp.com) and head to your [developer applications page](https://discordapp.com/developers/applications/me). If you're signed in, there should be a button that says "New App," click it.

You should see a page to name your app and setup a description.Once you give it a name and an icon, click on "Create App" and "Enable Rich Presence" once you're in the app config.You should now be able to upload a cover image as well as assets. Upload your cover image, copy your "Client ID" \(not the secret or token!\),and head back to PkUnity. View the components for the Global prefab and you should see a string box named "Application ID," usually this boxalready has an ID, just replace it with yours.

## Assets

After you have set the Application ID, head back to the website. Upload some assets to get started with, in "Assets/Resources/DiscordRPC" thereare some example assets you could use. The main menu uses the key "main\_menu" and the players use the keys "m\_\[outfitname\]" and "f\_\[outfit\]", usually the outfits are set to "hgss".

![](/img/application.png)

Now it's time to upload maps. Try to get your best screenshot of the overworld, you can manipulate the camera and reset the time of day using [Debug Mode](/debugmode.md). Once you have your screenshot, format it to 512x512 and upload it as an asset. Keep note of the key you used for later. After uploading everything, go to your map settings and add the token to "Discord Image Key." Repeat the same tokens for it's sub-maps as well, however set the state box to say something like "Inside a Pokemon Center," "Inside my house," or "Exploring Cave Zephyr." Once all of the tokens are set, head in-game and walk around a bit. Make sure the editor window is set as your game on Discord.

Check your presence, if it says something along the lines of this \(Should display follower info and current state in-game\), you've added everything correctly!

![](/img/presenceexample.png)

