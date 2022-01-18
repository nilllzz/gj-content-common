# Mark: Tag

| Field                | Value |
| -------------------- | ----- |
| **Mark Object Type** | `tag` |

---

Text decorated with this mark represents a clickable "hashtag".

The text that is decorated with this mark should always start with a "#" symbol. There are also additional constraints placed on which characters can appear in a tag.

The `tag` attribute on this mark has to match the decorated text, minus the "#" symbol.

## Attributes

| Name  | Description                   |
| ----- | ----------------------------- |
| `tag` | The tag (without leading "#") |

## Example

```
{
    "type": "text",
    "text": "#helloworld",
    "marks: [
        {
            "type": "tag",
            "attrs": {
                "tag": "helloworld"
            }
        }
    ],
}
```

#### Produces:

[#helloworld](https://gamejolt.com/search?q=#helloworld)
