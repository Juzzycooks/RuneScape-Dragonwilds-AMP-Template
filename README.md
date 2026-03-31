# RuneScape: Dragonwilds AMP Template

This revision removes CustomArgs from startup and updates the metaconfig heading to use the Unreal config section seen in the live logs.

## Files included

- manifest.json
- juzzycooksdragonwilds.kvp
- juzzycooksdragonwildsconfig.json
- juzzycooksdragonwildsmetaconfig.json
- juzzycooksdragonwildsports.json
- juzzycooksdragonwildsupdates.json

## Important changes in this revision

- Launch command changed to `./RSDragonwildsServer.sh`
- Ready regex tightened around confirmed runtime log lines
- Metaconfig heading changed to `/Script/Dominion.DedicatedServerSettings`
- ParamFieldName values updated to match the Unreal settings section

## Add to AMP

1. Put these files in the root of a GitHub repo.
2. In AMP go to Configuration -> Instance Deployment.
3. Add the repo in the format `user/repo:branch`.
4. Click Fetch.
5. Refresh the browser.
6. Create a new instance using the template prefix `juzzycooks`.

## Notes

- This template is for the native Linux dedicated server.
- Steam anonymous updates are disabled.
- Change the default admin password after deployment.
- After creating the instance, save the instance settings so AMP writes DedicatedServer.ini.
