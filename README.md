<div align="center">
  <h1>DiscordBot</h1>
  <p><strong>Python Discord bot with moderation, utility commands, dice rolls, and voice-channel controls.</strong></p>
  <p>
    <img alt="Python" src="https://img.shields.io/badge/Python-303840?style=flat-square" />
    <img alt="Discord.py" src="https://img.shields.io/badge/Discord.py-303840?style=flat-square" />
  </p>
  <p><a href="#overview">Overview</a> · <a href="#getting-started">Getting started</a> · <a href="#repository-map">Repository map</a></p>
</div>

---

## Overview

A personal Discord bot built with prefix commands. It combines small social utilities with moderation actions and voice-channel join/leave controls.

## What’s inside

- Administrator-gated mute, ban, unban, and kick commands.
- A dice roll, interactive calculator, and shortcut links.
- Voice-channel join and leave commands.

## Getting started

Create your own Discord application and bot, enable the privileged intents used by the code, and invite it to a test server with appropriate permissions. Then:

```sh
python -m pip install "discord.py[voice]"
export DISCORD_BOT_TOKEN="your-own-bot-token"
python taikidiscord/bot.py
```

Commands use the `!` prefix, for example `!roll`, `!calc`, `!join`, and `!leave`. Moderation requires the correct server permissions and role hierarchy; `!mute` expects a `Muted` role.

## Repository map

| Location | Purpose |
| --- | --- |
| [`taikidiscord/bot.py`](./taikidiscord/bot.py) | Bot instance, commands, and startup |
| [`taikidiscord/main.py`](./taikidiscord/main.py) | Legacy entry point; references an unavailable wrapper |

## Project status

Personal prototype. Start `bot.py` directly; the legacy `main.py` calls a wrapper that is not defined. A previously committed credential must be revoked or rotated; removing it from the current source does not erase Git history.
