# Object: Paragraph

| Field                   | Value                     |
| ----------------------- | ------------------------- |
| **Content Object Type** | `paragraph`               |
| **Group**               | `block`                   |
| **Valid children**      | objects of group `inline` |

---

An object representing a paragraph of text (or other `inline` objects like [\<object:gjEmoji\>](/docs/objects/gjEmoji.md)).

## Attributes

(none)

## Example

```
{
    "type": "paragraph",
    "content": [
        {
            "type": "text",
            "text": "Hello, World!"
        }
    ]
}
```
