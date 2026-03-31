# RuneScape: Dragonwilds AMP Template

Files included:

- manifest.json
- juzzycooksdragonwilds.kvp
- juzzycooksdragonwildsconfig.json
- juzzycooksdragonwildsmetaconfig.json
- juzzycooksdragonwildsports.json
- juzzycooksdragonwildsupdates.json

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
- If the wrapper script does not launch directly, switch the executable to `/bin/bash` and pass `./RSDragonwildsServer.sh` as the command line.
