# Lowlight for SillyTavern

**Lowlight** is a roleplaying cyberpunk city: wet streets, neon, and people with lives of their own. This extension brings Lowlight's world into SillyTavern:
- **The live rooms** behind your chat: lights, glow, rain on the glass, steam, passing cars, and lightning.
- **The cast:** characters and personas, each with their own sprites and the city's lore book.
- **The city map.**
- **The rooms' songs.**
- **Lowlight's look.**

Your contact can change the room as you talk: the mood, the weather, the lights, or walking you both somewhere else.

The full game, with missions, jobs, quests and the city's clock, is on **https://www.patreon.com/cw/Farban**.

## Install

1. In SillyTavern, open **Extensions → Install extension**.
2. Paste `https://github.com/johdavken/lowlight-sillytavern` and install.
3. Reload. Lowlight asks once whether to install its cast (characters, personas and the lore book). Say **Y**.

To update, use **Extensions → Manage extensions → Update**. New characters install by themselves.

## Settings it needs

- **API:** Chat Completion → OpenRouter, with a model that supports tool calling. GLM (`z-ai/glm-5.2`) is what Lowlight is tuned on. On a Text Completion backend the rooms, sound and cast all work, but your contact can't change the room.
- **Enable function calling** (AI Response Configuration). The welcome switches it on for you. Without it the rooms still render, but your contact can't change them.
- **Context size of 16k tokens or more; 32k is better** (same panel). SillyTavern's default of 4,095 leaves no room for the conversation once the card and lore are in, so your contact would answer with no memory of the chat. If yours is still at that default, the welcome raises it to 32k; a size you set yourself is left alone. Both settings are SillyTavern's own, so they apply to all your chats.

## Keys

- **Alt+M** opens the city map; GO walks you both there.
- **Alt+Y** opens your persona, **Alt+P** the characters.
- **SYS** (top right): sound levels, every SillyTavern panel, CAST, HER ROOM TOOLS, and LOOK.
- `/select` opens the character select, `/room <name>` and `/mood <name>` change the room, and `/lowchat` switches between Lowlight's look and SillyTavern's own.

## Licenses

- **Code:** GPL-3.0-or-later (`LICENSE`).
- **Lowlight's writing, art and songs:** CC BY-NC-SA 4.0 (`CONTENT-LICENSE`). Share and remix them for free, with credit, but not commercially.
- **Third-party parts:** see `CREDITS.md` and `THIRD-PARTY-LICENSES.md`.

The lore book (`Lowlight`) is replaced on updates, so copy it if you want to edit it.
