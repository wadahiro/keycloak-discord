# keycloak-discord

Keycloak Social Login extension for Discord.


## Install

Download `keycloak-discord-ear-<version>.ear` from [Releases page](https://github.com/wadahiro/keycloak-discord/releases).
Then deploy it into `$KEYCLOAK_HOME/standalone/deployments/` directory.

## Setup

### Discord

Access to [Discord Developer Portal](https://discordapp.com/developers/applications/#top) and create your application.
You can get Client ID and Client Secret from the created application.

### Keycloak

1. Open `Themes` setting page in `master` realm. Then set `discord` theme as `Admin Console Theme`. Note: You may need to re-login for reloading the theme.
2. Add `discord` Identity Provider in the realm which you want to configure.
3. In the `discord` identity provider page, set `Client Id` and `Client Secret`.
4. (Optional) Set Guild Id(s) to allow federation if you want.


## Source Build

Clone this repository and run `mvn package`.
You can see `keycloak-discord-ear-<version>.ear` under `ear/target` directory.


## Licence

[Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0)


## Author

- [Hiroyuki Wada](https://github.com/wadahiro)

