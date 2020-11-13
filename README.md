# wuhu-plugin-json-export

Super simple wuhu plugin for exporting compo data into JSON. Intended for use
with [jamviewer](https://github.com/chiptunecafe/jamviewer) and our
[normalization script](https://gist.github.com/rytone/140d438ef93251fb0e5b3d0b8b147e69).

## Installation

Just clone this repository into the Wuhu `plugins` directory.

## Usage

Enable the plugin, then a "JSON Export" option should appear in the Wuhu admin
sidebar. The data is emitted in the format:

```json
[
    {
        "directory_name": string,
        "display_name": string,
        "entries": [
            {
                "title": string,
                "author": string,
                "comment": string,
                "orgacomment": string,
                "filename": string,
                "playingorder": number
            },
            ...
        ]
    },
    ...
]
```
