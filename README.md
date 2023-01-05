# sunvox-deb

Unofficial Debian / Ubuntu packages for SunVox, the modular synthesizer and tracker. https://www.warmplace.ru/soft/sunvox/

## Bootstrapping

If you haven't yet built any `.deb` packages on a Debian 11+ system, run:

```
sudo apt install devscripts
```

## Build

If this repository is up to date with the latest version of SunVox, run:

```
uscan --download-current-version --verbose
origtargz -u
debuild -us -uc
```

Otherwise, write a new changelog entry (`dch -v <upstream-version>+repack-0utopia1`) and then run the above commands.
