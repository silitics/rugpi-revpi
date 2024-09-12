# Rugpi Example for Revolution Pi

This is an example for building bespoke variants of *RevPi Bookworm* with [Rugpi](https://rugpi.io).

> [!WARNING]  
> This is only a proof of concept, do not use in production! To get a fully functional setup, a deeper integration with RevPi is necessary. In particular, Rugpi must be appropriately configured to preserve all relevant configuration files.

To learn more about Rugpi, checkout <https://rugpi.io>. Rugpi allows you to build bespoke variants of popular Linux distributions and comes with a robust over-the-air system update mechanism, specially developed for Raspberry Pi.


## Instructions

The following instructions assume that you are using the 64-bit Bookworm beta image.

1. Download the *RevPi Bookworm 64-bit Lite* image from <https://revolutionpi.com/en/tutorials/downloads#revpiimages>.
2. Place the extracted image with the name `240902-revpi-bookworm-arm64-lite.img` in the `base` folder. Should your image have a different name, you need to adjust the `url` parameter in the RevPi base layer `layers/revpi-bookworm.toml`.
3. Afterwards you can build a customized with `./run-bakery bake image tryboot`.

The resulting image has Rugpi Ctrl installed and supports OTA updates.
