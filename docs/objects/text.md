# Object: Text

| Field                   | Value    |
| ----------------------- | -------- |
| **Content Object Type** | `text`   |
| **Group**               | `inline` |
| **Valid children**      | (none)   |

---

Adds plain text to the document. The actual text is contained within the `text` property of the object. This object type is the only one that is allowed to use the `text` property.

This object must not have any child objects.

## Attributes

(none)

## Marks

Mark objects are decorations for displayed text. For a list of valid marks, see [\<type:mark-object\>](/docs/types/mark-object.md).

Only `text`-type objects can have marks.

## Examples

### Plain text

```
{
    "type": "text",
    "text": "Hello, World!"
}
```

#### Produces:

Hello, World!

### Strong (bold) text

```
{
    "type": "text",
    "text": "Hello, World!",
    "marks: [
        {
            "type": "strong",
        }
    ],
}
```

#### Produces:

**Hello, World!**

### Strong (bold) and italic text

```
{
    "type": "text",
    "text": "Hello, World!",
    "marks: [
        {
            "type": "strong",
        },
        {
            "type": "em",
        }
    ],
}
```

#### Produces:

**_Hello, World!_**
