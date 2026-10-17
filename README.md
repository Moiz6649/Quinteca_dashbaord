# Quinteca Dashboard

Standalone Savant-style dashboard for Home Assistant. Installs as an integration and adds its own **sidebar panel**. No Lovelace setup, no token, no YAML.

- Home page: greeting, clock, one tile per service (only services with devices appear)
- Lighting / Shades / Climate / Media → room list → room page with custom cards
- Cameras and Security pages (door / lock / intercom status)
- **More**: add any entity or any Lovelace card (JSON) to any room
- Settings: rooms (from HA Areas), device → room assignment, hide devices, fullscreen mode
- Settings are stored on the HA server and shared by all devices (only admins can change them)

## Install
1. HACS → ⋮ → **Custom repositories** → add `https://github.com/<your-user>/quinteca-dashboard`, type **Integration**.
2. Download **Quinteca Dashboard** and **restart Home Assistant**.
3. Settings → Devices & services → **Add integration** → *Quinteca Dashboard* → enter the title (e.g. Quinteca).
4. **Quinteca** appears in the sidebar. Hard-refresh the browser if it doesn't.

Create a GitHub release (e.g. `v1.1.0`) so HACS can install it. Replace `YOUR-USER` in `manifest.json`.

## Fullscreen / wall panel
Settings → **Fullscreen** hides the HA sidebar on that device (☰ button brings it back).
