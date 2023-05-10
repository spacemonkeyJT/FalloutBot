[Back to Contents](./README.md)

## Settings

Open the `config/settings.json` file, which will initially have some empty values to be filled in:

| Name      | Value                                                                                                             |
|-----------|-------------------------------------------------------------------------------------------------------------------|
| account   | The name of the account you want to connect to chat with. This can be your broadcaster account, or a bot account. |
| authToken | Authentication token to login to Twitch using the above account.                                                  |
| channel   | Name of the channel that the bot should login to.                                                                 |

To generate the auth token, use this link, and authorise using the account of your choice: https://id.twitch.tv/oauth2/authorize?response_type=token&client_id=uxj8hdpst8v4lutkr842b3lxz8tp0o&redirect_uri=http://localhost:3000&scope=chat%3Aread+chat%3Aedit. The browser will then navigate to a new URL including the auth token, which you can copy and paste into the settings. This process will be improved in a future version.

Other settings can be configured:

| Name                  | Value                                                                                                     |
|-----------------------|-----------------------------------------------------------------------------------------------------------|
| commandPrefix         | Prefix to identify commands, e.g. use # to have commands such as #spawn                                   |
| pointsPerMinuteViewed | Number of points viewers automatically gain for every minute spent watching stream.                       |
| pointsUpdateInterval  | How often automatically gained points are updated in milliseconds, e.g. 10000 to update every 10 seconds. |
| pointsPerCheerBit     | Number of points viewers gain for every bit cheered.                                                      |
| pointsPerSubscription | Number of points viewers gain for subscribing or gifting a sub.                                           |
| chatEnabled           | Whether the bot should say anything in chat.                                                              |
| debug                 | Enables verbose logging and other debug functions.                                                        |
