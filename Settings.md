[Back to Contents](./README.md)

## Settings

General settings are found in the `config/settings.json` file:

| Name                  | Value                                                                                                             |
|-----------------------|-------------------------------------------------------------------------------------------------------------------|
| account               | The name of the account you want to connect to chat with. This can be your broadcaster account, or a bot account. |
| authToken             | Authentication token to login to Twitch using the above account.                                                  |
| channel               | Name of the channel that the bot should login to. The app will prompt for this on first launch if not set.        |
| commandPrefix         | Prefix to identify commands, e.g. use # to have commands such as #spawn                                           |
| pointsPerMinuteViewed | Number of points viewers automatically gain for every minute spent watching stream.                               |
| pointsUpdateInterval  | How often automatically gained points are updated in milliseconds, e.g. 10000 to update every 10 seconds.         |
| pointsPerCheerBit     | Number of points viewers gain for every bit cheered.                                                              |
| pointsPerSubscription | Number of points viewers gain for subscribing or gifting a sub.                                                   |
| chatEnabled           | Whether the bot should say anything in chat.                                                                      |
| debug                 | Enables verbose logging and other debug functions.                                                                |

By default the account and authToken are set up to use the bot account, JanglesTheBot. This is the user that will reply to commands in chat. This default account is set for out of the box convenience, but you can change this to another account, e.g. your own account, if you prefer.

To generate a new auth token, use [this link](https://id.twitch.tv/oauth2/authorize?response_type=token&client_id=uxj8hdpst8v4lutkr842b3lxz8tp0o&redirect_uri=http://localhost:3000&scope=chat%3Aread+chat%3Aedit), and authorise using the account of your choice. The browser will then navigate to a new URL including the auth token, which you can copy and paste into the settings. This process will be improved in a future version.
