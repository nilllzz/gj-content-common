# Object: Media Item

| Field                   | Value       |
| ----------------------- | ----------- |
| **Content Object Type** | `mediaItem` |
| **Group**               | `block`     |
| **Valid children**      | (none)      |

---

Displays a Game Jolt Media Item.

## Attributes

| Name      | Description                                                                           |
| --------- | ------------------------------------------------------------------------------------- |
| `id`      | Numeric id of the Game Jolt Media Item                                                |
| `width`   | The assumed width the Media Item will take up                                         |
| `height`  | The assumed height the Media Item will take up                                        |
| `caption` | Alt text that will show up when the Media Item cannot be loaded, or when hovered over |
| `align`   | Alignment options. Can be `"left"`, `"center"` or `"right"`                           |
| `href`    | An optional hyperlink that will be followed when this object is clicked               |

## Example

```
{
    "type": "mediaItem",
    "attrs": {
        "id": 1234,
        "width": 1280,
        "height": 720,
        "caption": "This is a Media Item caption!",
        "align": "center",
        "href: "https://gamejolt.com",
    }
}
```

#### Produces:

[![This is a Media Item caption!](/docs/_media/objects-mediaItem-example.png "This is a Media Item caption!")](https://gamejolt.com)
