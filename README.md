# Install Build Dependencies

```shell
apt update
apt install meson, build-essential
```

# Install Gstreamer Rgaconvert

```shell
cd gstreamer-rgaconvert
meson setup build --prefix=/usr
meson compile -C build
meson install -C build
```

# Test Gstreamer Rgaconvert

```shell
gst-inspect-1.0 --plugin | grep rga
```
