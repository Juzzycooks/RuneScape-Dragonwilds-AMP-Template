# RuneScape: Dragonwilds AMP Template

This revision assumes AMP installs the dedicated server into the `4019830` subfolder.

## Files included

- manifest.json
- juzzycooksdragonwilds.kvp
- juzzycooksdragonwildsconfig.json
- juzzycooksdragonwildsmetaconfig.json
- juzzycooksdragonwildsports.json
- juzzycooksdragonwildsupdates.json

## Important changes in this revision

- Base directory changed to `./4019830`
- Working directory changed to `./4019830`
- Executable changed to `/bin/bash`
- Launch command changed to `./RSDragonwildsServer.sh {{CustomArgs}}`
- Metaconfig path changed to `4019830/RSDragonwilds/Saved/Config/LinuxServer/DedicatedServer.ini`

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
- If startup still fails, check that these files exist:
  - `4019830/RSDragonwildsServer.sh`
  - `4019830/RSDragonwilds/Binaries/Linux/RSDragonwildsServer-Linux-Shipping`
- If needed, ensure both are executable with `chmod +x`.
