# City Obyte Governance Discord bot

Watch the [City Obyte](https://city.obyte.org) and posts notifications on Discord when something happens.

## Setup

- `yarn`
- Run with `node start.js`, it will create an app data directory in `%APPDATA%/city-governance-discord` then fail due to configuration missing
- While logged on Discord webapp, create an application at https://discord.com/developers/applications 
- Select the application, select bot in menu, copy the bot token
- Copy `.env.sample` file to `.env` and complete it with the bot token and the channel id the bot will post to
- While logged on Discord, use the following url template to add the bot to your server: https://discord.com/oauth2/authorize?client_id=881946977754038272&scope=bot&permissions=2048, `client_id` can be found in the General Information of your Discord application (Application ID), permissions should be `2048` to allow only posting message.
- Run the bot with `node start.js`