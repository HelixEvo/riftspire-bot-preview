<p align="center">
  <img src="https://images.blocpow.io/riftspire-bot.jpg" alt="Riftspire BOT Logo" width="200"/>
  <h1 align="center">Riftspire BOT</h1>
  <p align="center">A powerful Discord bot for managing and monitoring Riftspire/Pterodactyl-based game servers.</p>
</p>

## 🚀 Features

- 📊 Dash Server Stats — View real-time statistics about your core system  
- 🌐 Node Stats — Monitor remote or local game nodes via Netdata  
- 🎮 Game Server Stats — Track uptime, player count, MOD's, general game settings and resource usage
- Automated Game and MOD updater with Discord feedback and in-game warnings/countdown
- 📁 Backups & Restores — Create and restore backups per game server from Discord
- 📤 Download Backups — Access saved backups via secure download from Discord
- 💬 Global Chat Relay — Cross-post in-game global chat to Discord  
- 🧑‍🤝‍🧑 Player Monitor — Track connected players across clusters 
- 🧬 Tribe Log Posting — Post tribe logs to channels in real-time
- 🤖 Bot Health Stats — Monitor Riftspire BOT’s internal performance

## 📸 Gallery

<p align="center">
  <img src="https://images.blocpow.io/bot-commands.jpg" width="400"/><br/>
  <em>🤖 Slash and legacy commands supported</em>
</p>

<p align="center">
  <img src="https://images.blocpow.io/core-stats.jpg" width="400"/><br/>
  <em>📊 Core system stats — CPU, RAM, uptime</em>
</p>

<p align="center">
  <img src="https://images.blocpow.iocore-stats-2.jpg" width="400"/><br/>
  <em>🌐 Remote node monitoring with Netdata</em>
</p>

<p align="center">
  <img src="https://images.blocpow.io/gameserver-info.jpg" width="400"/><br/>
  <em>🎮 Game server overview — players, version, mod info</em>
</p>

<p align="center">
  <img src="https://images.blocpow.io/list-backups.jpg" width="400"/><br/>
  <em>🗂️ Backup list — view and select from multiple saves</em>
</p>

<p align="center">
  <img src="https://images.blocpow.io/list-backups-2.jpg" width="400"/><br/>
  <em>📁 Auto-titled backups sorted by timestamp</em>
</p>

<p align="center">
  <img src="https://images.blocpow.io/download-backup.jpg" width="400"/><br/>
  <em>⬇️ Direct backup download with secure links</em>
</p>

<p align="center">
  <img src="https://images.blocpow.io/download-backup-2.jpg" width="400"/><br/>
  <em>🔒 Only permitted users can access backup files</em>
</p>

<p align="center">
  <img src="https://images.blocpow.io/globalchat-discord.jpg" width="400"/><br/>
  <em>💬 Global in-game chat mirrored to Discord</em>
</p>

<p align="center">
  <img src="https://images.blocpow.io/player-activity.jpg" width="400"/><br/>
  <em>👥 Player join/leave detection with live tracking</em>
</p>

<p align="center">
  <img src="https://images.blocpow.io/tribe-logs.jpg" width="400"/><br/>
  <em>🦖 Tribe log posting — unclaims, kills, activity logs</em>
</p>

## 📦 Requirements

- Node.js v18+  
- MariaDB / MySQL  
- Riftspire/Pterodactyl Panel (API access)  
- Netdata running on each node (remote or local)  
- Game servers must be reachable for RCON and/or Daemon/Wings API  

## 🔧 Setup

1. Clone the repository  
   ```bash
   git clone https://github.com/YOUR_USERNAME/riftspire-bot.git
   cd riftspire-bot
   ```

2. Install dependencies  
   ```bash
   npm install
   ```

3. Run setup  
   ```bash
   node setup.js
   ```

4. Start the bot  
   ```bash
   node index.js
   ```

## ⚙️ Configuration

Create a `.env` file based on this example:

```env
# Discord
DISCORD_TOKEN=your-bot-token

# Pterodactyl Panel
PANEL_URL=https://your.panel.url
PANEL_API_KEY=your-panel-api-key

# Database
DB_HOST=localhost
DB_PORT=3306
DB_USER=riftspire
DB_PASS=password
DB_NAME=riftspire_bot

# Remote Nodes (optional)
NODE_1_NAME=bitcoin.blocpow.io
NODE_1_NETDATA_URL=http://10.0.0.2:19999
NODE_1_WINGS_URL=https://10.0.0.2:8080
NODE_1_WINGS_KEY=your-wings-api-key
```

> 💡 Tip: You can support multiple nodes by repeating the `NODE_X_*` pattern.

## 🛠️ Included Scripts

- `setup.js` — CLI wizard to generate your `.env`  
- `checkNodes.js` *(optional)* — Tests connectivity to remote Netdata endpoints  
- `application.js` — Main bot entrypoint  

## 📚 Documentation

> Coming soon: Full usage guides, screenshots, and config walkthroughs.

## 💬 Get Support

Need help or want to suggest features?  
👉 Join the Discord: [https://discord.gg/yHxrk8Kg5R](https://discord.gg/yHxrk8Kg5R)

## ☕ Like This Bot? Buy Me a Brew (BTC)

If Riftspire BOT saves you time and stress, consider donating to support future updates.

- **BTC Address**: `bc1q53kphqjtph8q4ldd49e8yhwgqqf6wt9aerpxys`  
- Or scan this QR code:

<p align="center">
  <a href="https://www.bitcoinqrcodemaker.com" target="_blank">
    <img src="https://www.bitcoinqrcodemaker.com/api/?style=bitcoin&amp;address=bc1q53kphqjtph8q4ldd49e8yhwgqqf6wt9aerpxys"
         height="300" width="300" border="0"
         alt="Bitcoin QR code generator"
         title="bitcoin:bc1q53kphqjtph8q4ldd49e8yhwgqqf6wt9aerpxys">
  </a>
</p>

## 🪪 License

This project is licensed under the MIT License — free to use, modify, and share.

## 🌌 Made with ❤️ for the Dash Server Community
