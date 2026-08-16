# LoRa Chat — releases

Binary releases and the update manifest for the (private) LoRa Chat project.

- `manifest.json` — checked by the Android app (self-update) and by ESP32 nodes
  (`{"cmd":"fw_update"}` over BLE) to discover the latest versions.
- Release assets: `app-release.apk` plus optional `firmware-<env>.bin`
  (per-board) and `firmware-<env>-<node>.bin` (per-node, preferred by nodes
  when present, since firmware bakes per-node config at build time).
