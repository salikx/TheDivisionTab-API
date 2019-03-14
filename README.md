<p align="center">
  <h1 align="center">Official TheDivisionTab API Documentation</h3>
</p>

<hr>

## About
- Please note that We are offering this API to all of the users in the community who would to get creative with our data.

## Limitations
- There are no limitations to this API as long as it is not abused. We hold the right to refuse service to anyone who we believe is abusing this system.

<hr>

## Search by name

Request URL {GET} https://thedivisiontab.com/api/search.php


METHOD | **platform**:

- <i>**uplay**</i> will only display PC/Uplay players<br>
- <i>**psn**</i> will only display Playstation players<br>
- <i>**xbl**</i> will only display Xbox players<br>

METHOD | **name**:

- <i>**playername**</i> urlencode the playername<br>

Example: https://thedivisiontab.com/api/search.php?name=baiier&platform=uplay

Example response:
```
{
  "results": [
    {
      "pid": "9bd44bde-9c48-48ae-9c2b-4e11e4b16083",
      "name": "BaIIer",
      "user": "9bd44bde-9c48-48ae-9c2b-4e11e4b16083",
      "platform": "uplay",
      "kills_pvp": 0,
      "kills_npc": 159,
      "level_pve": 3,
      "level_dz": 0,
      "avatar_146": "https://ubisoft-avatars.akamaized.net/9bd44bde-9c48-48ae-9c2b-4e11e4b16083/default_146_146.png",
      "avatar_256": "https://ubisoft-avatars.akamaized.net/9bd44bde-9c48-48ae-9c2b-4e11e4b16083/default_256_256.png"
    }
  ],
  "totalresults": 1
}
```
This will return up to 30 players max.
<hr>

## Get player data by ID

Request URL {GET} https://thedivisiontab.com/api/player.php

METHOD | **pid**:

- <i>**pid**</i> is the ID that Ubisoft assigns to every player.<br>

An example of a player ID is: <i>**9bd44bde-9c48-48ae-9c2b-4e11e4b16083**</i>

Example: https://thedivisiontab.com/api/player.php?pid=9bd44bde-9c48-48ae-9c2b-4e11e4b16083

Example response: 
```
{
  "pid": "9bd44bde-9c48-48ae-9c2b-4e11e4b16083",
  "name": "BaIIer",
  "platform": "uplay",
  "user": "9bd44bde-9c48-48ae-9c2b-4e11e4b16083",
  "visitors": 1,
  "utime": 1552555520,
  "ecredits": 100,
  "level_pve": 3,
  "level_dz": 0,
  "lastmission": "mm01_grandhyatt",
  "xp_clan": 0,
  "xp_dz": 0,
  "xp_ow": 8169,
  "xp_pvp": 0,
  "timeplayed_total": 4001,
  "timeplayed_dz": 0,
  "timeplayed_pve": 4001,
  "timeplayed_pvp": 0,
  "timeplayed_rogue": 0,
  "maxtime_rogue": 0,
  "kills_npc": 159,
  "kills_pvp": 0,
  "kills_total": 159,
  "kills_bleeding": 0,
  "kills_shocked": 0,
  "kills_burning": 1,
  "kills_ensnare": 0,
  "kills_headshot": 28,
  "kills_skill": 14,
  "kills_turret": 3,
  "kills_pvp_namedbosses": 1,
  "kills_pvp_elitebosses": 0,
  "kills_pvp_dz_total": 0,
  "kills_pvp_dz_rogue": 0,
  "kills_pve_hyenas": 42,
  "kills_pve_outcasts": 0,
  "kills_pve_blacktusk": 0,
  "kills_pve_truesons": 0,
  "kills_pve_dz_hyenas": 0,
  "kills_pve_dz_outcasts": 0,
  "kills_pve_dz_blacktusk": 0,
  "kills_pve_dz_truesons": 0,
  "kills_wp_pistol": 0,
  "kills_wp_grenade": 0,
  "kills_wp_smg": 0,
  "kills_wp_shotgun": 0,
  "kills_wp_rifles": 142,
  "kills_specialization": 0,
  "specialization": "",
  "headshots": 186,
  "looted": 13,
  "gearscore": 0,
  "extra_data": "{\"LatestMissionCompleted.missionState.Begin\":\"mm01_grandhyatt\",\"weaponFamilyKills.weaponFamily.MountedWeapon\":\"3\",\"weaponNameKills.weaponName.player_grenade_landing\":\"8\"}",
  "avatar_146": "https://ubisoft-avatars.akamaized.net/9bd44bde-9c48-48ae-9c2b-4e11e4b16083/default_146_146.png",
  "avatar_256": "https://ubisoft-avatars.akamaized.net/9bd44bde-9c48-48ae-9c2b-4e11e4b16083/default_256_256.png",
  "playerfound": true
}
```

<hr>

## Affiliation
- TheDivisionTab API is in no way shape or form affiliated with Ubisoft and its partners. Any "The Division" name, logos and/or images are registered trademarks of Ubisoft.
