# Fork-code/ha-beenthere

Local fork of [tampie85/ha-beenthere](https://github.com/tampie85/ha-beenthere).

Changes:
- Any signed-in Home Assistant user can add/rename travellers, mark visits,
  manage groups and regional detail. Deleting travellers or groups stays
  admin-only (`ADMIN_ONLY_ACTIONS` in `__init__.py`, `canDelete()` in the card).
- In the sidebar panel (`fill_screen: true`) the map box grows to fill the
  free screen height; the map covers the box and can be dragged to pan.
  Dashboard cards keep the original layout.

Updating: `git fetch upstream && git merge upstream/main`, re-check the
patched spots, push, then update in the HA Marketplace.
