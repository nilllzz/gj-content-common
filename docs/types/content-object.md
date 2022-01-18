# Type: Content Object

A Content Object is the fundemental building block of every Game Jolt Content Document. Depending on its `type`, it can perform all sorts of different functions.

## Definition

```
{
    "type": <enum:content-object-type>,
    "text": null,
    "content": [
        <type:content-object>
    ],
    "marks": [
        <type:mark-object>
    ],
    "attrs": { [key: string]: any }
}
```

| Field     | Description                                                                                                                               |
| --------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| `type`    | The type of the object.<br>See [\<enum:content-object-type\>](/docs/enums/content-object-type.md).                                        |
| `text`    | _(For `text`-type objects only)_ The display text of the object.                                                                          |
| `content` | A list of child objects of the object.                                                                                                    |
| `marks`   | _(For `text`-type objects only)_ A list of Marks used to decorate this object.<br>See [\<type:mark-object\>](/docs/types/mark-object.md). |
| `attrs`   | A map (`string` -> `any`) of additional attributes. Accepted attributes depend on the object type.                                        |

---

Do note that any fields except for `type` are optional, and can be left out entirely if they are supposed to be empty.

## List of Content Objects by `type`

These are all possible Objects that can be represented by a Content Object. Which Object is chosen is dependent on the `type` field on the Content Object.

| `type` field value | Object                                                 |
| ------------------ | ------------------------------------------------------ |
| `blockquote`       | [\<object:blockquote\>](/docs/objects/blockquote.md)   |
| `bulletList`       | [\<object:bulletList\>](/docs/objects/bulletList.md)   |
| `codeBlock`        | [\<object:codeBlock\>](/docs/objects/codeBlock.md)     |
| `embed`            | [\<object:embed\>](/docs/objects/embed.md)             |
| `gif`              | [\<object:gif\>](/docs/objects/gif.md)                 |
| `gjEmoji`          | [\<object:gjEmoji\>](/docs/objects/gjEmoji.md)         |
| `hardBreak`        | [\<object:hardBreak\>](/docs/objects/hardBreak.md)     |
| `heading`          | [\<object:heading\>](/docs/objects/heading.md)         |
| `hr`               | [\<object:hr\>](/docs/objects/hr.md)                   |
| `listItem`         | [\<object:listItem\>](/docs/objects/listItem.md)       |
| `mediaItem`        | [\<object:mediaItem\>](/docs/objects/mediaItem.md)     |
| `orderedList`      | [\<object:orderedList\>](/docs/objects/orderedList.md) |
| `paragraph`        | [\<object:paragraph\>](/docs/objects/paragraph.md)     |
| `spoiler`          | [\<object:spoiler\>](/docs/objects/spoiler.md)         |
| `sticker`          | [\<object:sticker\>](/docs/objects/sticker.md)         |
| `text`             | [\<object:text\>](/docs/objects/text.md)               |

## Content Object children

Each Content Object can theoretically contain any number of children that are valid for its `type`. To define which children an object can hold, it either specifies a `group` of objects, or an object `type` specifically. Children are stored in the `content` field as a list.

When looking at an object page, one can find which `group` it belongs to, as well as which `group` or `type` of children it allows.

### Example

(This is the data for the [\<object:paragraph\>](/docs/objects/paragraph.md) object)

| Field                   | Value       |
| ----------------------- | ----------- |
| **Content Object Type** | `paragraph` |
| **Group**               | `block`     |
| **Valid children**      | `inline`    |

It belongs to the `block` group (which is closely equivalent to the `display: block` CSS attribute), so it can be added as a child to any object that requires its children to be of the `block` group.

The paragraph object itself however can only take objects of the `inline` group as its children (also equivalent to the `display: inline` CSS attribute).

Some objects like [\<object:orderedList\>](/docs/objects/orderedList.md) may specify that only a single object type may make up its children, in that case [\<object:listItem\>](/docs/objects/listItem.md).
