# Omarchy kit releases

Public runtime bundles for certified Omarchy desktops. Install from the kit ISO;
then run `kit update`. No GitHub account or private repository access is needed.

Each release contains `bundle.tar.zst`, `manifest.json`, `channel.json` and
`channel.json.sig`. The kit verifies the Ed25519 channel signature using its
installed release key, then checks the archive SHA256 and every payload file.
The ISO and update use the same runtime payload. Prereleases are test channels
and are never selected by the normal updater.

Source and certification are maintained in the owner's private setup-kit repo.
This repository is a distribution channel, not a source mirror. Runtime shell
plugins retain their licenses; native plugins are distributed as compiled assets.
