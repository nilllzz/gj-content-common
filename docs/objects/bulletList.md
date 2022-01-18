# Object: Bullet List

| Field                   | Value                                |
| ----------------------- | ------------------------------------ |
| **Content Object Type** | `bulletList`                         |
| **Group**               | `block`                              |
| **Valid children**      | at least 1 object of type `listItem` |

---

Defines an unordered list with each list item being prefaced by a bullet character.

## Attributes

(none)

## Example

```
{
    "type": "bulletList",
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

-   Hello,
-   World!
