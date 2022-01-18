# Object: Code Block

| Field                   | Value                                 |
| ----------------------- | ------------------------------------- |
| **Content Object Type** | `codeBlock`                           |
| **Group**               | `block`                               |
| **Valid children**      | objects of type `text` or `hardBreak` |

---

A block of text formatted to look like programming code.

Only [\<object:text\>](/docs/objects/text.md) and [\<object:hardBreak\>](/docs/objects/hardBreak.md) objects are allowed as children, unlike most other `block` group objects that allow wrapping text in a [\<object:paragraph\>](/docs/objects/paragraph.md).

## Attributes

(none)

## Example

```
{
    "type": "codeBlock",
    "content": [
        {
            "type": "text",
            "text": "Hello,"
        },
        {
            "type": "hardBreak"
        },
        {
            "type": "text",
            "text": "World!"
        }
    ]
}
```

#### Produces:

```
Hello,
World!
```
