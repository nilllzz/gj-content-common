# Object: Blockquote

| Field                   | Value                    |
| ----------------------- | ------------------------ |
| **Content Object Type** | `blockquote`             |
| **Group**               | `block`                  |
| **Valid children**      | objects of group `block` |

---

Wraps its contents in a quote.

## Attributes

(none)

## Example

```
{
    "type": "blockquote",
    "content": [
        "type": "paragraph",
        "content": [
            {
                "type": "text",
                "text": "Hello, World!"
            }
        ]
    ]
}
```

#### Produces:

> Hello, World!
