# Object: Heading

| Field                   | Value                                 |
| ----------------------- | ------------------------------------- |
| **Content Object Type** | `heading`                             |
| **Group**               | `block`                               |
| **Valid children**      | at least 1 object of type `paragraph` |

---

Represents a larger heading that contains a [\<object:paragraph\>](/docs/objects/paragraph.md) of inline content.

## Attributes

| Name    | Description                                                                                         |
| ------- | --------------------------------------------------------------------------------------------------- |
| `level` | The level/size of the heading. Can be either `1` or `2`. Level `1` heading is larger than level `2` |

## Example

```
{
    "type": "heading",
    "content": [
        "type": "paragraph",
        "content": [
            {
                "type": "text",
                "text": "This is my article"
            }
        ],
        "attrs": {
            "level": 1
        }
    ]
}
```

#### Produces:

# This is my article
