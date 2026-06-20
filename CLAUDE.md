# JARVIS Projekt – Offene Aufgaben

## Nächster Schritt: Obsidian Vault via MCP verbinden

Der Nutzer möchte seinen **Obsidian Vault** mit Claude Code über einen **MCP-Server** verbinden.

### Was bereits erledigt ist
- JARVIS Web-App (`jarvis-vercel/index.html`) ist fertig und hat bereits Zugriff auf den Obsidian Vault über die **Obsidian Local REST API**
- Die App ist für Vercel vorbereitet (`vercel.json`)

### Was noch fehlt
MCP-Server (`mcp-obsidian`) einrichten, damit Claude Code direkt auf den Obsidian Vault zugreifen kann.

### Nächste Schritte (beim nächsten Gespräch fortführen)

1. Nutzer nach folgenden Infos fragen:
   - **Port** der Obsidian Local REST API (Standard: `27123`)
   - **API-Key** aus den Plugin-Einstellungen in Obsidian

2. MCP-Konfiguration für Claude Code erstellen (`.claude/mcp.json` oder `~/.claude/settings.json`)

3. Installation erklären:
   ```bash
   npm install -g mcp-obsidian
   ```

4. Konfiguration testen

### Hinweis
- Funktioniert nur lokal (nicht in Cloud-Sessions), da die Obsidian Local REST API auf `localhost` läuft
- Nutzer ist mit dem Konzept vertraut und hat MCP Option 2 gewählt
