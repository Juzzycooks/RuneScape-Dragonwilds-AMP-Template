# RuneScape: Dragonwilds AMP Template

This revision adds the Linux runtime environment fix and corrects the OwnerId field name.

## Files included

- manifest.json
- juzzycooksdragonwilds.kvp
- juzzycooksdragonwildsconfig.json
- juzzycooksdragonwildsmetaconfig.json
- juzzycooksdragonwildsports.json
- juzzycooksdragonwildsupdates.json
- OPTIONAL_WRAPPER_PATCH.txt

## Important changes in this revision

- Added `XDG_RUNTIME_DIR=/tmp/amp-runtime` to environment variables
- Corrected `OwnerId` casing everywhere
- Keeps the `4019830` base/working directory fix
- Keeps the shell-wrapper launch path

## After deploying

Create the runtime directory for the AMP user:

```bash
mkdir -p /tmp/amp-runtime
chown amp:amp /tmp/amp-runtime
chmod 700 /tmp/amp-runtime
```

Then fetch the repo in AMP, create a fresh instance, save the server settings, and start the server.
