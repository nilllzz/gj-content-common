# Object: Embed

| Field                   | Value   |
| ----------------------- | ------- |
| **Content Object Type** | `embed` |
| **Group**               | `block` |
| **Valid children**      | (none)  |

---

Embeds some kind of resource from a 3rd party source.

## Attributes

| Name     | Description                                                   |
| -------- | ------------------------------------------------------------- |
| `type`   | The identifier for the type of resource                       |
| `source` | The referenced source of the resource that should be embedded |

## Example

```
{
    "type": "embed",
    "attrs": {
        "type": "youtube-video",
        "source": "dQw4w9WgXcQ",
    }
}
```

#### Produces:

(An embedded YouTube video from https://youtube.com/watch?v=dQw4w9WgXcQ)
