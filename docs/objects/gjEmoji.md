# Object: GJ Emoji

| Field                   | Value     |
| ----------------------- | --------- |
| **Content Object Type** | `gjEmoji` |
| **Group**               | `inline`  |
| **Valid children**      | (none)    |

---

Represents an inline Game Jolt (GJ) Emoji.

## Attributes

| Name   | Description                  |
| ------ | ---------------------------- |
| `type` | The type of emoji to display |

Valid emoji `type`s are:

-   sleeping
-   bucktooth
-   crossed
-   crying
-   dizzy
-   grin
-   guh
-   huh
-   innocent
-   mah
-   ninja
-   ohyou
-   omg
-   ouch
-   psychotic
-   smile
-   snooty
-   tongue
-   wha
-   yush

## Examples

```
{
    "type": "gjEmoji",
    "attrs": {
        "type": "psychotic"
    }
}
```

#### Produces:

![https://tenor.com/8lge.gif](/docs/_media/objects-gjEmoji-example.png)
