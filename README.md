# Local manifests

`repo` local manifests for the LineageOS 23.2 ports maintained under
[HamelinPorts](https://github.com/HamelinPorts).

## Recommended: per-device branch

Each supported device has its own branch carrying only the manifest
for that device.  Inside your LineageOS source tree, clone the
branch you need:

| Device | Codename | Branch |
|--------|----------|--------|
| Samsung Galaxy A51 (SM-A515F/DSN) | a51 | [`a51`](https://github.com/HamelinPorts/local_manifests/tree/a51) |
| Samsung Galaxy Tab A8 2021 (SM-X205) | gta8 | [`gta8`](https://github.com/HamelinPorts/local_manifests/tree/gta8) |

```sh
# example for gta8
git clone -b gta8 https://github.com/HamelinPorts/local_manifests \
    .repo/local_manifests
repo sync
```

## All-devices branch (this one)

The default branch (`lineage-23.2`) carries every device's manifest
file in one checkout — kept for backwards compatibility.  If you use
this branch, delete the manifests for the devices you do not want
before running `repo sync`.
