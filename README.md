# Customer Build Sheet

A sleek, single-file web app that generates your WAN/VCG build outputs.

## Files
- `index.html` — the app (open this in your browser)
- `serve.bat` — Windows one-click local hosting on port 8080
- `serve.sh` — macOS/Linux one-liner local hosting on port 8080

## Quick Preview
- Double-click `index.html`

## Share on your LAN (Windows)
1. Double-click `serve.bat`
2. Open: `http://<your-machine-ip>:8080`
3. Keep the terminal open to keep the server running

## Share on macOS/Linux
```bash
chmod +x serve.sh
./serve.sh
# then visit http://<your-machine-ip>:8080
```

## Notes
- /31 rule: **entered IP** = Gateway, **entered IP + 1** = Firewall
- BGP SVC Leaves 01–04 use RD bases: `10.100.220.6..9`
- 3-digit WAN VLAN → tag `40<wan>` (e.g., `210` → `40210`)
- 4-digit WAN VLAN → tag `4<wan>` (e.g., `1210` → `41210`)
