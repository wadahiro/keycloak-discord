# keycloak-discord

Keycloak Social Login extension for Discord.


## Install

Download `keycloak-discord-ear-<version>.ear` from [Releases page](https://github.com/wadahiro/keycloak-discord/releases).
Then deploy it into `$KEYCLOAK_HOME/standalone/deployments/` directory.

## Setup

### Discord

Access to [Discord Developer Portal](https://discord.com/developers/applications) and create your application.
You can get Client ID and Client Secret from the created application.

### Keycloak

Note: You don't need to setup the theme in `master` realm from v0.3.0.

1. Add `discord` Identity Provider in the realm which you want to configure.
2. In the `discord` identity provider page, set `Client Id` and `Client Secret`.
3. (Optional) Set Guild Id(s) to allow federation if you want.


## Source Build

Clone this repository and run `mvn package`.
You can see `keycloak-discord-ear-<version>.ear` under `ear/target` directory.


## Licence

[Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0)


## Author

- [Hiroyuki Wada](https://github.com/wadahiro)

