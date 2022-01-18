# Object: GIF

| Field                   | Value   |
| ----------------------- | ------- |
| **Content Object Type** | `gif`   |
| **Group**               | `block` |
| **Valid children**      | (none)  |

---

Embeds a "GIF" from a 3rd party source.

## Attributes

| Name      | Description                                                    |
| --------- | -------------------------------------------------------------- |
| `id`      | An identifier for the GIF on the service it originated from    |
| `width`   | The assumed width the GIF will take up                         |
| `height`  | The assumed height the GIF will take up                        |
| `service` | An identifier for the service the GIF originated from          |
| `media`   | A map holding various media references to display the GIF from |
| `url`     | A hyperlink to view the GIF on the 3rd party service's website |

## Example

```
{
    "type": "gif",
    "attrs": {
        "id": "14342340",
        "width": 640,
        "height": 342,
        "service": "tenor",
        "media": {
            "webm": {
                "url": "https:\/\/media.tenor.com\/videos\/133fd8a0ff4df3c4917de3366f5b7b91\/webm",
                "tiny": "https:\/\/media.tenor.com\/videos\/0e977c9973a4911d0402a3f92c0c741a\/webm"
            },
            "mp4": {
                "url": "https:\/\/media.tenor.com\/videos\/84b353f4f08a077bdebfbf1cb7cc8c88\/mp4",
                "tiny": "https:\/\/media.tenor.com\/videos\/db2ffa857d099c06c7f9d673db7fe3dd\/mp4"
            },
            "preview": "https:\/\/media.tenor.com\/images\/efb0bfd0c8913559e16e2b894cdfbc69\/tenor.png"
        },
        "url": "https:\/\/tenor.com\/8lge.gif"
    }
}
```

#### Produces:

![https://tenor.com/8lge.gif](/docs/_media/objects-gif-example.png)
