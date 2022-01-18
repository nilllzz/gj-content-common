# Mark: Mention

| Field                | Value     |
| -------------------- | --------- |
| **Mark Object Type** | `mention` |

---

Text decorated with this mark represents a "mention" of a user account.

The text that is decorated with this mark should always start with an "@" symbol. There are also additional constraints placed on which characters can appear in a mentioned user account name.

The `username` attribute on this mark has to match the decorated text, minus the "@" symbol.

## Attributes

| Name       | Description                                                  |
| ---------- | ------------------------------------------------------------ |
| `username` | The name of the mentioned user account (without leading "@") |

## Example

```
{
    "type": "text",
    "text": "@nilllzz",
    "marks: [
        {
            "type": "mention",
            "attrs": {
                "username": "nilllzz"
            }
        }
    ],
}
```

#### Produces:

[@nilllzz](https://gamejolt.com/@nilllzz)
