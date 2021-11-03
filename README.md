# Flatpak for Flycast

## Installation

1. [Set up Flatpak](https://www.flatpak.org/setup/)

2. Install Flycast from [Flathub](https://flathub.org/apps/details/org.flycast.Flycast)

`flatpak install -y org.flycast.Flycast`

3. Run Flycast

`flatpak run org.flycast.Flycast`

To uninstall: `flatpak uninstall -y org.flycast.Flycast`

## Build

The `flatpak-builder` package is required.

- Install the SDK

`flatpak install org.freedesktop.Sdk/x86_64/21.08`

- Build Flycast

`flatpak-builder --user --install --force-clean build-dir org.flycast.Flycast.yml`
