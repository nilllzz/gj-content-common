# Object: Ordered List

| Field                   | Value                                |
| ----------------------- | ------------------------------------ |
| **Content Object Type** | `orderedList`                        |
| **Group**               | `block`                              |
| **Valid children**      | at least 1 object of type `listItem` |

---

Defines an ordered list with each list item being prefaced by an order mark (such as a number).

## Attributes

(none)

## Example

```
{
    "type": "orderedList",
    "content": [
        {
            "type": "listItem",
            "content": [
                "type": "paragraph",
                "content": [
                    {
                        "type": "text",
                        "text": "Hello,"
                    }
                ]
            ]
        },
        {
            "type": "listItem",
            "content": [
                "type": "paragraph",
                "content": [
                    {
                        "type": "text",
                        "text": "World!"
                    }
                ]
            ]
        }
    ]
}
```

#### Produces:

1.  Hello,
2.  World!
