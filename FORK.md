# Fork-code/ha-beenthere

Local fork of [tampie85/ha-beenthere](https://github.com/tampie85/ha-beenthere).

Changes:
- Full access: every signed-in Home Assistant user can add, rename and delete
  travellers and groups, mark visits and change regional detail.
- Live updates use a `beenthere/subscribe` websocket command, because Core
  refuses to let non-admin users subscribe to custom bus events.
- Map zoom goes up to 64x (was 8x) with borders that stay thin when zoomed.
- In the sidebar panel (`fill_screen: true`) the map box grows to fill the
  free screen height; the map covers the box and can be dragged to pan.
  Dashboard cards keep the original layout.

Patch script: ~/ops/scripts/beenthere_patch.py on ubuntu-docker-host.

Updating: `git fetch upstream && git merge upstream/main`, re-check the
patched spots, push, then update in the HA Marketplace.
