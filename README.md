# sunvox-deb

Unofficial Debian / Ubuntu packages for SunVox, the modular synthesizer and tracker. https://www.warmplace.ru/soft/sunvox/

## Build

If this repository is up to date with the latest version of SunVox, run:

```
uscan --download-current-version --verbose
debuild -us -uc
```

Otherwise, run:

```
uscan --download --verbose
dch -v <upstream-version>-0utopia1  # Write a new changelog entry
debuild -us -uc
```
