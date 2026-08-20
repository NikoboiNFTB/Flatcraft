# Flatcraft

Minicraft+ Flatpak Edition.

> [!NOTE]
> The original README is available at [/README.md.old](/README.md.old)

> [!WARNING]
> Fully vibecoded into a Flatpak. All of the commands below eventually got it working, but not all of them are probably necessary. I don't do Flatpak and I won't pretend I do. This was just a cool idea I had and ChatGPT said yeah it's doable, so "I did."

## Install

Run:

```
flatpak-builder --user --install --force-clean build-dir dev.nikoboi.flatcraft-plus-revived.yaml
```

## Launch

Run:

```
flatpak run dev.nikoboi.flatcraft-plus-revived
```

## Bundle

Run:

```
flatpak build-bundle repo flatcraft-plus.flatpak dev.nikoboi.flatcraft-plus-revived
```

### Fixes?

```
flatpak-builder --export-only --repo=repo_tmp dev.nikoboi.flatcraft-plus-revived.yaml
```

```
flatpak build-bundle repo_tmp flatcraft-plus.flatpak dev.nikoboi.flatcraft-plus-revived
```

### Fixes

```
flatpak-builder --export-only --repo=repo build-dir dev.nikoboi.flatcraft-plus-revived.yaml
```

```
flatpak build-bundle repo flatcraft-plus.flatpak dev.nikoboi.flatcraft-plus-revived
```

```
flatpak install --user flatcraft-plus.flatpak
```
