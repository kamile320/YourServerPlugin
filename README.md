# YourServer Plugin - Full Customization for Your Minecraft Server

[![SpigotMC](https://img.shields.io/badge/SpigotMC-119291-blue?logo=spigotmc)](https://www.spigotmc.org/resources/yourserver-plugin-with-full-customization.119291/)
[![Minecraft Versions](https://img.shields.io/badge/Minecraft-1.13%2B-green?logo=minecraft)](https://www.spigotmc.org/resources/yourserver-plugin-with-full-customization.119291/)
[![Languages](https://img.shields.io/badge/Languages-EN%2CPL%2CDE-yellow?logo=language)](https://www.spigotmc.org/resources/yourserver-plugin-with-full-customization.119291/)

## Overview
YourServer is a powerful, all-in-one plugin for Bukkit/Spigot/Paper servers, offering full customization for admins and players. It includes advanced management tools for bans, mutes, teleports, homes, warps, kits, warnings, and much more. Built for ease of use with multilingual support (English, Polish, German), it's perfect for community servers needing robust moderation without complexity.

**Key Highlights:**
- Compatible with Minecraft 1.13+
- Configurable via `config.yml` for permissions and behaviors
- Console-friendly commands
- No external dependencies

## Features
- **Moderation Tools**: Ban, tempban, mute, tempmute, warn, tempwarn, kick
- **Chat Management**: Admin chat, private messages, chat toggle/clear
- **Player Utilities**: Feed, heal, fly toggle, gamemode change, godmode, vanish
- **Teleportation System**: TPA requests, accept/deny, direct TP to players/coords
- **Home & Warp System**: Set, delete, list, and teleport to homes/warps
- **Kit System**: Permission-based kits with cooldowns
- **Statistics & Inspection**: Online players list, inventory/enderchest viewing, player ID check
- **Warning & Stats**: Warn history, tempwarn info, server statistics GUI
- **Customization**: Nicknames, emotes, cheat detection, and more
- **Multilingual**: Built-in support for EN, PL, DE

## Installation
1. Download the latest `.jar` from [Releases](https://github.com/Delivetator/YourServerPlugin/releases).
2. Place `YourServer.jar` in your server's `plugins/` folder.
3. Restart the server or run `/reload confirm`.
4. Edit `plugins/YourServer/config.yml` for custom settings (e.g., permissions, messages).
5. Reload with `/yourserver reload` (requires `yourserver.plugin.reload` perm).

**Note**: Ensure you have Spigot/Paper 1.13+ installed. No additional setup required!

## Commands
All commands work for players and console (except where noted). Use `<>` for required args, `()` for optional.

### Core Moderation
- `/ban <player> (reason)` - Ban a player (`ban`)
- `/tempban <player> <time> <unit> (reason)` - Temporary ban (e.g., `/tempban Steve 1 h`) (`tempban`)
- `/unban <player>` - Unban (`unban`)
- `/mute <player> (reason)` - Mute (`mute`)
- `/tempmute <player> <time> <unit> (reason)` - Temp mute (`tempmute`)
- `/unmute <player>` - Unmute (`unmute`)
- `/warn <player> (reason)` - Warn (`warn`)
- `/tempwarn <player> <time> <unit> (reason)` - Temp warn (`tempwarn`)
- `/delwarn <player>` - Delete warn (`delwarn`)
- `/deltempwarn <player>` - Delete temp warn (`deltempwarn`)
- `/warninfo <player>` - View warns (`warninfo`)
- `/tempwarninfo <player>` - Temp warn info (`tempwarninfo`)
- `/kick <player> (reason)` - Kick (`kick`)

### Chat & Communication
- `/adminchat <message>` - Admin-only chat (`adminchat`)
- `/chat <on/off/clear>` - Toggle/clear chat (no perm)
- `/msg <player> <message>` - Private message (no perm)
- `/helpop <message>` - Send help-op message (no perm)

### Player Management
- `/feed [player]` - Feed self/others (`feed`, `feed-player`)
- `/heal [player]` - Heal (`heal`, `heal-player`)
- `/fly [player]` - Toggle fly (`fly`, `fly-player`)
- `/gamemode <0/1/2/3> [player]` - Set gamemode (`gamemode`, `gamemode-player`)
- `/god [player]` - Toggle godmode (`god`, `god-player`)
- `/vanish [player]` - Toggle vanish (`vanish`, `vanish-player`)
- `/nick <nick/off>` - Change nick (`nick`)
- `/nick <player> <nick/off>` - Change other's nick (`nick-player`)
- `/invsee <player>` - View inventory (`invsee`)
- `/enderchest [player]` - View enderchest (`enderchest`, `enderchest-player`)
- `/id <player>` - Get player UUID (`id`)
- `/online` - List online players (no perm)
- `/check <player>` - Check for cheats (`check`)

### Teleportation & Locations
- `/tpa <player>` - Request teleport (no perm)
- `/tpaccept <player>` - Accept request (no perm)
- `/tpdeny <player>` - Deny request (no perm)
- `/tp <player>` - TP to player (`teleport`)
- `/tp <x> <y> <z>` - TP to coords (`teleport`)
- `/tp <player1> <player2>` - TP player1 to player2 (`teleport`)
- `/s <player>` - TP player to you (`tptome`)
- `/home <home>` - TP to home (no perm)
- `/sethome <home>` - Set home (no perm)
- `/delhome <home>` - Delete home (no perm)
- `/homes` - List homes (no perm)
- `/warp <warp>` - TP to warp (no perm)
- `/setwarp <warp>` - Set warp (`setwarp`)
- `/delwarp <warp>` - Delete warp (`delwarp`)
- `/warps` - List warps (no perm)
- `/spawn` - TP to spawn (no perm)
- `/setspawn` - Set spawn (`setspawn`)

### Kits & Utilities
- `/kit <kitname>` - Claim kit (`kit.<kitname>`)
- `/emotes` - Open emotes menu (no perm)
- `/statistics` - View stats GUI (no perm)
- `/yourserver version` - Check version (no perm)
- `/yourserver commands` - List commands (no perm)
- `/yourserver command <name>` - Command info (no perm)
- `/yourserver reload` - Reload config (`yourserver.plugin.reload`)

## Permissions
All perms are configurable in `config.yml`. Defaults:
- No perm = available to everyone
- Console bypasses all perms
- Example: `yourserver.ban` for `/ban`

## Configuration
Edit `config.yml` for:
- Messages (per language)
- Permission nodes
- Kit cooldowns/delays
- Warn thresholds (auto-ban after X warns)
- Language selection

Sample `config.yml` generated on first run.

## Support & Donations
- **Issues/Bugs**: Open a GitHub issue here.
- **Discord/Support**: Join the community (link TBA).
- **Donate**: Support development via [Tipply](https://tipply.pl/@Delivetator).

## License
MIT License – feel free to fork, modify, and contribute!

---

*Plugin developed by Delivetator. Forked and enhanced for better GitHub integration.*
