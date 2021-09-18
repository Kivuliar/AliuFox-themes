# Themer Docu for the xposed/plugin
This is a docu for dark mode theming, be welcome to add things to the docu! I would be really happy
* [License](https://github.com/GangsterFox/AliuFox-themes/blob/main/LICENSE)

<h1 align="center">Misc Strings for Plugin</h1>

**DO NOT CHANGE THE JSON DIRECTLY UNLESS YOU KNOW WHAT YOU ARE DOING, I AM NOT GOING TO GIVE YOU SUPPORT IF YOU DO CHANGE DIRECTLY.
INSTEAD USE THEMERS EDITOR TO ADD THINGS TO THE STRINGS**

> Strings used for the plugin to tell the user what the name of the theme is, author, version, License, etc but also things like custom font and custom background


* The manifest strings

Used to show name of the theme, author, etc. They are in the "manifest" section in the .json
```json
{
  "name": "the theme name",
  "author": "authors name",
  "license": "license, ask if you want to add one but dont know how to or what license to choose in #theme-development",
  "version": "this is the verion number, DO NOT USE TEXT AS A VERSION BECAUSE THIS **WILL** BREAK THE UPDATER AND WONT UPDATE YOUR THEME AT ALL",
  "updater": "this is where you put your raw.githubusercontent.com link, if you ever want to update your theme just bump the version number up"
}
```
When done correctly it should look like this in the json
![image](https://user-images.githubusercontent.com/84905506/132266565-ff27a087-4e36-48ca-baca-2a1d823939fd.png)

* Background strings

These are the strings for adding a background and also giving it transparency(alpha). They are in the "background" section in the .json
```json
{
  "url": "url for the bg image, recommended and trusted to use cdn.discordapp.com links",
  "alpha": "background transparency, goes from 0 to 255, 0 being fully transparent while 255 being fully opaque"
}
```
When done correctly it should look like this in the json
![image](https://user-images.githubusercontent.com/84905506/132266685-eaa4cca8-9d49-449a-bf8b-c17acc9d3270.png)
* Font string

The string for the font URL. The string is located in the "fonts" section in the .json
```json
{
  "*": "url of the font, recommended and trusted to use cdn.discordapp.com links"
}
```
When done correctly it should look like this in the json
![image](https://user-images.githubusercontent.com/84905506/132266358-3d8e34da-622d-49d9-b74a-d7dd1d413ee6.png)
<h1 align="center">Simple colors</h1>

string | behaviour
------------ | -------------
accent | "new messages since" text,<br/> send button, <br/>nitro "subscribe today", <br/>All toggles (position - ON), <br/>chat font scaling bar, <br/>DMs icon (top left), <br/>bot icon, <br/>upload emoji button, <br/>Role permissions (tick), <br/>join voice/video in server, <br/>phone number sent in chat, <br/>multiple buttons in settings (also "settings" in plugin list)
input_background | Server => overview => server name, <br/>editing role name, <br/>search (in server, dms, global via magnifier icon on the bottom), <br/>channel name and topic in server settings (edit channel), <br/>user notes background
mention_highlight | Highlights message that pinged you
statusbar | Top bar of the screen (above channel name) but only when you are in channel, dms, settings, friend list, stages
background | chat background, <br/>user list background, <br/>folders bg color, <br/>any bg you can think of, 
background_secondary | Top bar above channel name, <br/>search in DMs, servers, global

<h1 align="center">Colors</h1>

* Brand

string | behaviour
------------ | -------------
brand_new_530 | Ping color (@user changes color only), <br/>channel ping (ex. #general)
brand_new_560 | emoji reaction border
link | Link color

* Primary dark colors, used for the big things chat bg, server list, member list, etc for dark mode

string | behaviour
------------ | -------------
primary_dark_200 | Color for main text, <br/>text in embeds, <br/>server "mark as read", create channel, create category, change nickname, copy ID, <br/>channel list in server settings, <br/>member names + roles in member list, <br/>text in server settings => roles, <br/>"role color" text in role settings, <br/>most of the text in server invites, <br/>ban reason, <br/>text when about to kick/ban someone, <br/>friend list => names, <br/>users in "stage discovery", <br/>my account => user settings => phone number under sms auth, <br/>user settings => blocked users => "you don't have blocked users" text, <br/>perms in authorized apps, <br/>user settings => connections => spotify text about status broadcasting, <br/>user settings => appearance => *Aa* > **Aa**, <br/>attachment file names (when going to send one), <br/>most text in plugin related options
primary_dark_300 | text in single quotes, <br/>DMs (top left) icon, <br/>new group chat, <br/>discord icon (bottom left), <br/>friends, <br/>magnifier/search, <br/>stages, <br/>"sync your contacts" in friend list + add friend, <br/>search => last channel + suggestions + "where would you like to go?" + in mentions => filter icon, <br/>in stages - name and icon how many participants, <br/>all icons in user settings + "user settings" text, <br/>a lot of text in every setting, <br/>ticks (position OFF), <br/>attachments and emojis button, <br/>threads + "stay focused on a conversation" text when no active threads + '+' sign, <br/>search, <br/>invite members, <br/>settings icons, <br/>role names in member list (on the right panel), <br/>icons for default emojis, <br/>text under boosts, <br/>notifs, <br/>invite in server "profile", <br/>a lot of text (and icons!) in server settings, <br/>text under icons in profiles
primary_dark_360 | channel names/user names on DM list (not muted, not active/selected)
primary_dark_400 | "new unreads", <br/>status text in server/dm list/friend list, <br/>"today at" by the message, <br/>"message #channel/@user" on the bottom, <br/>"find perfect emoji" in emojis, <br/>search gifs/stickers, <br/>"find or start a conversation" top left, <br/>"tap to add note" in profiles, <br/>server "profile" - online/all members, <br/>"allow direct messages from server members", <br/>dot beside "XX EMOJIS [DOT HERE] Use anywhere with nitro", <br/>server overview > server name text, <br/>audit log - date, <br/>global search - search/mentions + usernames + statuses + server names + categories, 
primary_dark_600 | Main chat background, <br/> server folders background, <br/> member list background, <br/> bg in settings, <br/> bg in friend list, <br/> bg in search (global, server, dm), <br/> buttons in server "profile" (create channel, category, change nickname, direct messages, hide muted channels, copy ID and background for emojis there), <br/> every bg in server settings, "trust this domain" window, except the lower part of it with buttons
primary_dark_630 | bg for channel/dm list, <br/>chat icon bg (top left), <br/> top bar (where the channel name is), <br/> channel name (panel on the right side) with its desc and icons, <br/> embed background, <br/> background in user profile (under edit profile button / call or video icon), <br/> top bar in mutual servers/friends, <br/> search > mentions - "all servers" bar, search - background above "last channel" (under search/mentions top bar), <br/> top bar in friend list, "find your friends" button and call/message icon by each friend, <br/> stages > every stage has background now, <br/> user settings - top bar and your profile is colored now (except your customizable bg), <br/>every top bar in settings, <br/> connections > display on profile bg, <br/> authorized apps backgrounds
primary_dark_660 | attachment icon background, <br/>input area (where you type messages) background, <br/>when in settings - bar where your phone shows notif icons is colored, <br/> settings > connections - every connection is colored (top part of every connection), <br/> global search - both notif area and search/mentions tabs
primary_dark_700 | Phone's notifications bar, <br/>server list bg, <br/>"find or start a conversation" bg, <br/>things that are "out of view" (example, when looking at member list - look left and right), <br/>"find the perfect emoji" bg, same with gifs and stickers, <br/>bg in "server profile", <br/>server settings > enable community > those examples on top are having colored backgrounds (pokemon go, sneakers fans, learn latin, hogwarts school), <br/>server settings > roles - search bar bg, every role's bg, <br/>"scroll down" button (that appears bottom right), <br/>press and hold on a msg > emoji button bg, <br/>user profile (under custom bg, above about me section), <br/>
primary_dark_800 | Bottom bar (where friends, search, stages and your profile is) + space under it (android controls located there) - only when in dm list/channel list/friend list/stages/user settings (when in search - only android controls bar is changed), <br/>click and hold on a server - yup! that has a color now! (notifications/more options are there)
primary_dark_900 | Border color of authorized apps, <br/>after opening an attachment(image) - bg there changes (except for "view embed" bar), <br/>

* Primary strings used for both dark and light mode, used for smaller things


| String          | Purpose                 |
| ---------------- |:-----------------------:|
primary_100 | server > role settings (and role name) text (top bar)
primary_300 | server > member list > in the search bar (right side) some roles will change color, possibly ones with default grayish color, also in role list (example @everyone)
primary_700 | top bar (above channel name - but not when in search), <br/>spoilers, <br/>embed, <br/>DMs button, <br/>User status (online, idle, dnd, invis) background (in dm list only, not selected dm), <br/>notification (in app), <br/>(if using view permissions plugin - those will have background changed too) 

vvvvvvvvvvvvvvv to do vvvvvvvvvvvvvvv
<h1 align="center">uikit Strings</h1>

* uikit strings. They are in the Color Values screen if you dont know

| String          | Purpose                 |
| ---------------- |:-----------------------:|
| uikit_btn_bg_color_selector_brand | changes the settings button in settings like in the plugin list or dev options the 4 at the bottom |
| uikit_btn_bg_color_selector_green | change color for the online icon |
| uikit_btn_bg_color_selector_red | changes the ping color and in plugin list the uninstall button, also changes color for the "NEW MESSAGES" in chat |
| uikit_settings_item_text_color_dark | secondary text color |

<h1 align="center">Drawable Strings</h1>

* Drawable strings, used in a lot of places

| String          | Purpose                 |
| ---------------- |:-----------------------:|
| drawable_button_grey | unread messages button |
| drawable_overlay_channels_selected_dark | Selected channel color in channel list for dark mode |
| drawable_overlay_channels_pressed_dark | Pressed channel color in channel list for dark mode | 
| item_background_material | mostly used for the top bar(where the name of the plugin, version and author name is written) |
| design_bottom_navigation_item_background | is used mostly for the bottom part of the plugin page(where description is, uninstall and settings) also themes search box in plugins page |
| ic_channel_text | by the name it changes the channel text in the channel list, since it doesn't get themed it will only theme the # in the channel list and top bar when looking in chat |
| drawable_button_red | the red NEW↑ in the guild list when you get a ping in a guild |
| drawable_button_red_neutral | I actually have no idea what it does, if you find anything please tell me, thanks. |
| drawable_voice_indicator_speaking | the color for the ring when someone talks in a vc |
| drawable_voice_user_background_speaking | speaking background, I don't know how to better explain it |
| drawable_voice_sensitivity_progress | the progress bar for when you test out your mic sens |
| ic_ban_red_24dp | the ban icon color, kind of pointless tbh and no I don't know what the kick icon color string like at all |

<h1 align="center">Links for experienced Users</h1>

* This link by ven might help you if you know what you are doing

https://gist.github.com/Vendicated/7e8aa7b2512b8e38e041692cbf34acfa

<h1 align="center">Light mode theming</h1>

* The way to theme in light mode is to find as many strings which have the word "light". This means for example if you find primary_light, that means you found a light mode string.
* This might be quite weird to do since this is some territory no one has really tried yet. Bare in mind this might not work on plugin but dont take my word.
* When you try to theme in light mode, at least with primary colors, try to use the same strings as written in the docu but try to add the _light string. 
* **Always** search before you do anything to find strings.
* This means that if you will try theming in light mode, just try to add _light to the string
* And as always, Good luck
*this will get updated when I will found out more.* 
