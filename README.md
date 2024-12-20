> [!NOTE]
> Please use **boydaihungst**'s fork for the latest version of this plugin:
> https://github.com/boydaihungst/mediainfo.yazi

# mediainfo.yazi

This is a Yazi plugin for previewing media files. The preview shows thumbnail
using `ffmpegthumbnailer` if available and media metadata using `mediainfo`.

## Installation

Install the plugin:

```
ya pack -a Ape/mediainfo
```

Create `~/.config/yazi/yazi.toml` and add:

```
[plugin]
prepend_previewers = [
    { mime = "{image,audio,video}/*", run = "mediainfo"},
    { mime = "application/x-subrip", run = "mediainfo"},
]
```
