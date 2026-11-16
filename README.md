# kobo-registry-extended

An extended [kpm](https://github.com/wolffshots/kpm) package registry for Kobo e-readers, using [wolffshots/kobo-registry](https://github.com/wolffshots/kobo-registry) as the base.

## Included packages

**Base (from kobo-registry):** kpm, NickelClock, NickelDBus, NickelNote, NickelMenu, Nickel Screensaver, NickelTypeFix, NickelHardcover, Kscribbler, Kobo Wi-Fi Remote, NickelDissolve, NickelSync, NickelHome, Kobo Tweaks, KOReader, Plato, KF Core/Extra fonts.

**Extended additions:** KoboCloud, KoboMail, Kobo-UNCaGED, kobo-btpt, KoboWriter, KoboTerminal.

> Notes: Some entries are best-effort based on upstream release/layout conventions (assets, paths, uninstall behavior) and may require verification or tuning for specific device/firmware/package versions. `tested_fw`, checksums, and some uninstall recipes are omitted where not confidently known.

## Use with kpm

```sh
kpm registry add https://github.com/OivilOccas/kobo-registry-extended --name extended
kpm registry refresh
kpm search
kpm install <package-id> --yes
```

Or point to a local/raw copy of `registry.toml` hosted in your own git repo/fork.

See [kpm README](https://github.com/wolffshots/kpm#registries) for details.
