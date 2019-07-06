# thedivisiontab-py
A Python wrapper for the The Division Tab API
# Usage
```python
>> from thedivisiontab_py.thedivisiontab_py import user

# Default platform: uplay
# Platforms: uplay, psn, xbl
>> result = await user.get_by_name("Dhs92", "uplay")
# expected output
# {
#  "results": [
#    {
#      "pid": "21a5e030-016c-4850-ab4f-e971712d8794",
#      "name": "Dhs92",
#      "user": "21a5e030-016c-4850-ab4f-e971712d8794",
#      "platform": "uplay",
#      "kills_pvp": 6,
#      "kills_npc": 6324,
#      "level_pve": 30,
#      "level_dz": 23,
#      "avatar_146": "https://ubisoft-avatars.akamaized.net/21a5e030-016c-4850-ab4f-e971712d8794/default_146_146.png",
#      "avatar_256": "https://ubisoft-avatars.akamaized.net/21a5e030-016c-4850-ab4f-e971712d8794/default_256_256.png"
#   }
# ],
# "totalresults": 1
#}

# only accepts a uplay pid
>> result = await user.get_by_id("21a5e030-016c-4850-ab4f-e971712d8794")
# expected output
# {
#  "test_mode": true,
#  "pid": "21a5e030-016c-4850-ab4f-e971712d8794",
#  "name": "Dhs92",
#  "platform": "uplay",
#  "user": "21a5e030-016c-4850-ab4f-e971712d8794",
#  "visitors": 23,
#  "utime": 1562442910,
#  "ecredits": 77517,
#  "level_pve": 30,
#  "level_dz": 24,
#  "lastmission": "sm_nz01_boo_specializationadventure",
#  "xp_clan": 28746899,
#  "xp_dz": 90833,
#  "xp_ow": 26521030,
#  "xp_pvp": 0,
#  "timeplayed_total": 301260,
#  "timeplayed_dz": 11540,
#  "timeplayed_pve": 289426,
#  "timeplayed_pvp": 0,
#  "timeplayed_rogue": 704,
#  "maxtime_rogue": 437,
#  "kills_npc": 9109,
#  "kills_pvp": 6,
#  "kills_total": 9115,
#  "kills_bleeding": 137,
#  "kills_shocked": 68,
#  "kills_burning": 318,
#  "kills_ensnare": 12,
#  "kills_headshot": 2161,
#  "kills_skill": 1265,
#  "kills_turret": 95,
#  "kills_pvp_namedbosses": 158,
#  "kills_pvp_elitebosses": 43,
#  "kills_pvp_dz_total": 10,
#  "kills_pvp_dz_rogue": 5,
#  "kills_pve_hyenas": 2953,
#  "kills_pve_outcasts": 1496,
#  "kills_pve_blacktusk": 2804,
#  "kills_pve_truesons": 2335,
#  "kills_pve_dz_hyenas": 61,
#  "kills_pve_dz_outcasts": 60,
#  "kills_pve_dz_blacktusk": 0,
#  "kills_pve_dz_truesons": 38,
#  "kills_wp_pistol": 73,
#  "kills_wp_grenade": 0,
#  "kills_wp_smg": 645,
#  "kills_wp_shotgun": 232,
#  "kills_wp_rifles": 6805,
#  "kills_specialization": 4104,
#  "specialization": "sharpshooter",
#  "headshots": 19390,
#  "looted": 1847,
#  "gearscore": 500,
#  "extra_data": "{\"CountCommendations\":\"43\",\"LatestCommendationScore\":\"0\",\"LatestGearScore\":\"500\",\"LatestMissionCompleted.missionState.Begin\":\"sm_nz01_boo_specializationadventure\",\"LatestWalletBalanceSplit.currencyName.Apparel Cache Key Fragment\":\"41\",\"LatestWorldTier\":\"Tier 5\",\"SumCriticalHits\":\"11846\",\"SumDzKills\":\"20\",\"SumHits\":\"133861\",\"SumPveKills\":\"4028\",\"factionDarkZoneKills.npcFaction.Militia\":\"38\",\"numberOfRoguePlayerKills\":\"5\",\"specializationKills.playerSpecialization.playerspecialization_demolitionist\":\"1718\",\"specializationKills.playerSpecialization.playerspecialization_sharpshooter\":\"4104\",\"weaponFactionKills.weaponFamily.Shotgun.npcFaction.Blackbloc\":\"141\",\"weaponFactionKills.weaponFamily.Shotgun.npcFaction.Cultists\":\"2\",\"weaponFactionKills.weaponFamily.Shotgun.npcFaction.Militia\":\"89\",\"weaponFactionKills.weaponFamily.SubMachinegun.npcFaction.Blackbloc\":\"276\",\"weaponFactionKills.weaponFamily.SubMachinegun.npcFaction.Cultists\":\"16\",\"weaponFactionKills.weaponFamily.SubMachinegun.npcFaction.Endgame\":\"72\",\"weaponFactionKills.weaponFamily.SubMachinegun.npcFaction.Militia\":\"281\",\"weaponFamilyKills.weaponFamily.MountedWeapon\":\"95\",\"weaponNameKills.weaponName.player_grenade_landing\":\"153\"}",
#  "avatar_146": "https://ubisoft-avatars.akamaized.net/21a5e030-016c-4850-ab4f-e971712d8794/default_146_146.png",
#  "avatar_256": "https://ubisoft-avatars.akamaized.net/21a5e030-016c-4850-ab4f-e971712d8794/default_256_256.png",
#  "playerfound": true
}
