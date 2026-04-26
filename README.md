# Local manifests

Per-device `repo` local manifests for the LineageOS 23.2 ports
maintained under [HamelinPorts](https://github.com/HamelinPorts).

## Layout

| File | Device(s) |
|------|-----------|
| `a51.xml` | Samsung Galaxy A51 (SM-A515F/DSN, exynos9611 family) |
| `gta8.xml` | Samsung Galaxy Tab A8 2021 (SM-X205) |

Each file is self-contained — it defines its own `<remote>` entries
under unique names so multiple device manifests can coexist in the
same checkout without remote-name collisions.

## Usage

Clone into your LineageOS source tree's `.repo/local_manifests/`:

```sh
git clone https://github.com/HamelinPorts/local_manifests \
    .repo/local_manifests
```

If you only build for one device, you can delete the manifest files
for the other devices.  Then run `repo sync`.
