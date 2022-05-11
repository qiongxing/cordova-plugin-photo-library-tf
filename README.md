# What is this?

Basically, it's a fork/replacement for [xmarkclx/cordova-plugin-photo-library-sism](https://github.com/xmarkclx/cordova-plugin-photo-library-sism).

# What I Use It For, and thus what will almost always work

- Get permissions to access gallery/camera roll.
- Save image to gallery, even with query strings.
- Save video to gallery from external URL (even https:// URL 😎)

# How to Use?

Just use this as a drop-in replacement for that plugin.

Anyway, instead of installing the original plugin, install this one.

So follow the instructions from that one, but instead use this:

or if you have the old one installed already:

```bash
cordova plugin rm cordova-plugin-photo-library
```

Yeah, you will still need the "@ionic-native/photo-library" plugin.

add package in `dependencies`

```json
{
    "devDependencies":{
        ...
        "cordova-plugin-photo-library-tf": "https://github.com/qiongxing/cordova-plugin-photo-library-tf/archive/refs/tags/v3.0.1.tar.gz",
        ...
    }
}
```

# Release Notes

## 3.0.2

- fix android 11 & 12 saveImage flickering
