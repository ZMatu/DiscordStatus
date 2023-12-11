# Discord Status
This CSSharp plugin allows monitoring server status from discord with cute embeds and nameformat support.

## Requirments
[CounterStrikeSharp](https://github.com/roflmuffin/CounterStrikeSharp/) **>= 101**

## Usage
- Install plugin like u use to
- Make a webhost server and put connect.php there if you have one(you can use free webhosting like 000webhost)* not required
- Do the samething for map img url (or see below)
- Load the plugin
- Change the config
## Commands
- css_request - @notify members to join the server
- css_update_names - Update nameformat and updating the embed with the provided argument after the command. exmaple usage: css_update_names {FLAG}{CLAN} {NAME}: {K} - {D}
- css_update_settings - read and update settings from config without reloading the plugin
## Features
- **Displaying server status on discord**
- Showing Country Flags
- Custom Name Formatting
- Sorting Players by CT and T and with their respective team colors (not working if using flags)
- Sorting Players by kills
- different displays on Idle, with players, with players not inlined, requesting players, offline.
- Showing Connect ip:port
- Embeded links directing to automatically lauch steam and joins server
- Configurable update intervals to release serverloads
- Automatically update config and rename the old config

## Config
```json
{
  "GeneralConfig": {
    "ServerIP": "asd.asd", // actual ip address or custom domain: playcs2.com
    "UpdateInterval": 45,
    "PHPURL": "https://playcs2.com/connect.php"
  },
  "WebhookConfig": {
    "NotifyMembersRoleID": 0,
    "NewMapNotification": false,
    "GameEndScoreboard": true,
    "NotifyWebhookURL": "",
    "ScoreboardURL": "",
    "StatusWebhookURL": "",
    "StatusMessageID": 0
  },
  "EmbedConfig": {
    "Title": "",
    "MapImg": "{MAPNAME}.gif.jpg.png",
    "OfflineImg": "",
    "IdleImg": "{MAPNAME}.jpg/asdadsads.gif",
    "RequestImg": "",
    "EmbedColor": "#00ffff",
    "RandomColor": true,
    "MapField": "🗺️ㅤMap",
    "OnlineField": "👥ㅤOnline",
    "CTField": "CT :ㅤ{SCORE}",
    "TField": "T :ㅤ{SCORE}",
    "MVPField": " 👑ㅤMVP ",
    "NameFormat": "{FLAG}{CLAN} {NAME}: {K} - {D}",
    "PlayersInline": true
  },
  "Version": 4
}
```
```
NAME TAG FORMAT:
{NAME} = NAMES
{K} = KILLS
{D} = DEATHS
{A} = ASSISTS
{KD} = KD Ratio
{CLAN} = Clantag
{RC} = Region Code
{CC} = Country Code
{FLAG} = Country Flag
```
## Note
For imageurl u can also use "https://image.gametracker.com/images/maps/160x120/csgo/{MAPNAME}.jpg"

## Server Empty(Custom Img):
![image](https://github.com/Tian7777/DiscordStatus/assets/41808115/1b64768f-7ebe-4020-957c-8f9b514f988b)
## Server With Players(Custom Map Img / Custom Img):
![image](https://github.com/Tian7777/DiscordStatus/assets/41808115/0bba2635-886c-47ac-a7b6-c49b7fc0f53e)
## Scoreboard Snapshot
![image](https://github.com/Tian7777/DiscordStatus/assets/41808115/4d760cff-0483-4694-a1f2-97fb139b02f0)
## Request Players:
![image](https://github.com/Tian7777/DiscordStatus/assets/41808115/e50e0298-0581-485f-a1d6-46c6d9421bbd)

### Roadmap
- [x] Adding scoreboard snapshots 
