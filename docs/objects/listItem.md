# Object: List Item

| Field                   | Value                    |
| ----------------------- | ------------------------ |
| **Content Object Type** | `listItem`               |
| **Group**               | `block`                  |
| **Valid children**      | objects of group `block` |

---

Represents an item in a list, such as [\<object:bulletList\>](/docs/objects/bulletList.md) or [\<object:orderedList\>](/docs/objects/orderedList.md).

Note: this object should only ever be used as a direct child within a list object.

## Attributes

(none)

## Example

```
{
    "type": "listItem",
    "content": [
        "type": "paragraph",
        "content": [
            {
                "type": "text",
                "text": "Item"
            }
        ]
    ]
}
```

#### Produces:

_in a [\<object:bulletList\>](/docs/objects/bulletList.md):_

-   Item

_in an [\<object:orderedList\>](/docs/objects/orderedList.md):_

1. Item
