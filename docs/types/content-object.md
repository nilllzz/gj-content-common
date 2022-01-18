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

| Field     | Description                                                                                        |
| --------- | -------------------------------------------------------------------------------------------------- |
| `type`    | The type of the object.<br>See [\<enum:content-object-type\>](../enums/content-object-type.md).    |
| `text`    | _(For `text`-type objects only)_ The display text of the object.                                   |
| `content` | A list of child objects of the object.                                                             |
| `marks`   | A list of Marks used to decorate this object.<br>See [\<type:mark-object\>](mark-object.md).       |
| `attrs`   | A map (`string` -> `any`) of additional attributes. Accepted attributes depend on the object type. |

---

Do note that any fields except for `type` are optional, and can be left out entirely if they are supposed to be empty.
