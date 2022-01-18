# Mark: Link

| Field                | Value  |
| -------------------- | ------ |
| **Mark Object Type** | `link` |

---

Text decorated with this mark should appear as a hyperlink.

There are two different kinds of links: a "custom link", and an "autolink"

-   For custom links, the decorated text may differ from the hyperlink target, and can be set to anything.<br>
    A custom link is created when a user manually decorates non-hyperlink text with a link. For this case, the `autolink` attribute is set to `false`.

-   For autolinks, the decorated text has to match the hyperlink target exactly.<br>
    Autolinks are created when a user inserts text that looks like a hyperlink. In that case, the `autolink` attribute is set to `true`.

## Attributes

| Name       | Description                                                                                       |
| ---------- | ------------------------------------------------------------------------------------------------- |
| `href`     | The hyperlink target                                                                              |
| `title`    | Displayed title when hovering over the link with a mouse cursor. Can be empty                     |
| `autolink` | `true` if this link mark was added to the text automatically or `false` if a user did so manually |

## Example

### Custom link

```
{
    "type": "text",
    "text": "Look at my website!",
    "marks: [
        {
            "type": "link",
            "attrs": {
                "href": "https://nilllzz.indie.af",
                "title": "",
                "autolink": false,
            }
        }
    ],
}
```

#### Produces:

[Look at my website!](https://nilllzz.indie.af)

### Autolink

```
{
    "type": "text",
    "text": "https://nilllzz.indie.af",
    "marks: [
        {
            "type": "link",
            "attrs": {
                "href": "https://nilllzz.indie.af",
                "title": "https://nilllzz.indie.af",
                "autolink": true,
            }
        }
    ],
}
```

#### Produces:

[https://nilllzz.indie.af](https://nilllzz.indie.af)

### Custom link on a hyperlink text

```
{
    "type": "text",
    "text": "https://google.com",
    "marks: [
        {
            "type": "link",
            "attrs": {
                "href": "https://nilllzz.indie.af",
                "title": "",
                "autolink": false,
            }
        }
    ],
}
```

#### Produces:

[https://google.com](https://nilllzz.indie.af)
