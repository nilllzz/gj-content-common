# Object: Spoiler

| Field                   | Value                    |
| ----------------------- | ------------------------ |
| **Content Object Type** | `spoiler`                |
| **Group**               | `block`                  |
| **Valid children**      | objects of group `block` |

---

Similar to a [\<object:blockquote\>](/docs/objects/blockquote.md), but styled to hide its content unless interacted with. Acts like a spoiler-block.

## Attributes

(none)

## Example

```
{
    "type": "spoiler",
    "content": [
        "type": "paragraph",
        "content": [
            {
                "type": "text",
                "text": "Darth Vader is Luke's ... enemy"
            }
        ]
    ]
}
```

#### Produces:

> ! Darth Vader is Luke's ... enemy
