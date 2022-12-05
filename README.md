# acc_server_manager
ACC Dedicated Server Manager for spawning instances through a docker image

## Concept
Web panel manages the game-server settings and instances
- Using redis as db
- Discord OAuth for accounts

##### Instance spawn flow
1. Select instance pre-set
   - server config for different races (e.g. practice, repeating-short, sprint-race, endurance-race)
2. `bg will connect with cloud provider and load the docker image with the pre-set`
   - the image is based on [ubuntu 20.04](), using [steamcmd](https://developer.valvesoftware.com/wiki/SteamCMD)
   - 