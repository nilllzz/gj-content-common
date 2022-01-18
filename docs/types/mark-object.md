# Type: Mark Object

A Mark Object is representing a decoration on a [\<type:content-object\>](/docs/types/content-object.md). They can only be applied to [\<object:text\>](/docs/objects/text.md) objects.

## Definition

```
{
    "type": <enum:mark-object-type>,
    "attrs": { [key: string]: any }
}
```

| Field  | Description                                                                                  |
| ------ | -------------------------------------------------------------------------------------------- |
| `type` | The type of the object.<br>See [\<enum:mark-object-type\>](/docs/enums/mark-object-type.md). |

## List of Mark Objects by `type`

These are all possible Objects that can be represented by a Mark Object. Which Object is chosen is dependent on the `type` field on the Mark Object.

| `type` field value | Object                                     |
| ------------------ | ------------------------------------------ |
| `strong`           | [\<mark:strong\>](/docs/marks/strong.md)   |
| `em`               | [\<mark:italic\>](/docs/marks/italic.md)   |
| `strike`           | [\<mark:strike\>](/docs/marks/strike.md)   |
| `code`             | [\<mark:code\>](/docs/marks/code.md)       |
| `tag`              | [\<mark:tag\>](/docs/marks/tag.md)         |
| `mention`          | [\<mark:mention\>](/docs/marks/mention.md) |
| `link`             | [\<mark:link\>](/docs/marks/link.md)       |
