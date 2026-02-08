# minecraft-bot

A simple TypeScript-based Minecraft bot that connects to a Minecraft Java server and stays online to keep the server active.  
Primarily useful for free hosting platforms like **Aternos**, **Minehut**, or any self-hosted Minecraft server.

> This bot only connects to a **running server**.  
> It does NOT automate starting or controlling any hosting panel.

---

## Features

- Connects as a real Minecraft player
- Keeps server active by staying online
- Written in TypeScript
- Works with Aternos and other Java servers
- Easy to configure and extend

---

## Requirements

- Node.js **v18 or higher**
- npm
- Minecraft Java account (for online-mode servers)
- A running Minecraft Java server

---

## Installation

Clone the repository:

```bash
git clone https://github.com/sh3xu/minecraft-bot.git
cd minecraft-bot
````

Install dependencies:

```bash
npm install
```

---

## Configuration

Create a `.env` file in the project root:

```env
SERVER_HOST=your.server.address
SERVER_PORT=25565
BOT_USERNAME=YourBotUsername
BOT_PASSWORD=YourBotPassword
```

### Example (Aternos)

```env
SERVER_HOST=example123.aternos.me
SERVER_PORT=25565
BOT_USERNAME=AFKBot
```

Notes:

* If your server runs on the default port `25565`, keep it as shown.
* For **offline-mode servers**, password may not be required.
* For **online-mode servers**, use a valid Minecraft account.

---

## Build & Run

Compile TypeScript:

```bash
npm run build
```

Start the bot:

```bash
npm start
```

Or run directly:

```bash
node dist/bot.js
```

If successful, the bot will join the server as a player.

---

## Using With Aternos

1. Start your Aternos server manually from the panel.
2. Wait until the server status is **online**.
3. Run this bot locally or on a VPS.
4. The bot joins the server and keeps it active.

Important:

* This bot does NOT bypass Aternos limits.
* Automating the Aternos panel is against their ToS.
* This bot only provides in-game presence.

---

## Using With Other Servers

This bot works with:

* Self-hosted servers
* VPS-hosted servers
* Paid Minecraft hosting providers

Steps are the same:

1. Start the server
2. Set correct host and port
3. Run the bot

---

## Troubleshooting

**Bot does not connect**

* Server is offline
* Wrong host or port
* Firewall blocking connection

**Authentication error**

* Wrong username/password
* Server auth mode mismatch

**Version issues**

* Minecraft server version not supported by bot library
* Update dependencies if needed

---

## Development

For development or extending bot behavior:

```bash
npm run dev
```

You can add:

* Chat listeners
* AFK movement logic
* Command handling
* Plugins like pathfinding

---

## Disclaimer

Use this bot responsibly.
Always follow:

* Minecraft EULA
* Server rules
* Hosting provider Terms of Service

---

## License

MIT License

```

Just say the word 👌
```
