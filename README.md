# Plugin Minecraft AstranixBackups
AutoBackupGoogleDrive is a lightweight Minecraft plugin that automatically backs up your server worlds and important data directly to Google Drive, keeping your server safe from crashes, data loss, or accidental deletion.
The plugin is designed to be simple, reliable, and easy to configure. All setup instructions are explained step-by-step inside the config.yml, allowing server owners to get started quickly without complicated commands.

## 🚀 Getting Started
### Ultimate Backups
config.yml
```yml
# ID of the Folder Where Your Google Drive Backup Is Located.
google-drive-folder-id: ""
backup-interval-minutes: 120
# Leave blank ("") to follow the Server/VPS default time.
backup-timezone: "Asia/Jakarta"

# 'worlds' is a special keyword that will automatically include all world folders.
backup-items:
  - "server.properties"
  - "bukkit.yml"
  - "spigot.yml"
  - "config"
  - "server-icon.png"
  - "banned-ips.json"
  - "banned-players.json"
  - "plugins"
  - "logs"
  - "worlds"

# Leave blank ("") if you don't want to use this feature.
discord-webhook-url: ""

notifications:
  in-game: false
  console: true

# WARNING: This will delay the server shutdown time until the backup is complete.
preRestartBackup: false

# If a crash is detected for 60 seconds, the plugin will attempt an emergency backup.
crashBackup: true
```

### Links
- Documentation: [Github](https://github.com)
- Plugin: [AstranixLiteBackups](https://builtbybit.com) [AstranixUltimateBackups](https://builtbybit.com)
- Support: [Discord](https://discord.com)
