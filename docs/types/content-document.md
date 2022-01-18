# Type: Content Document

The Content Document object is the root of the a Game Jolt Content Document.

```
{
    "createdOn": "1640154652257",
    "context": <enum:document-context>,
    "version": "1.0.0",
    "content": [
        <type:content-object>
    ],
    "hydration": [
        <type:content-hydration-entry>
    ]
}
```

| Field       | Description                                                                                                                                                                                                       |
| ----------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `createdOn` | Millisecond-accurate timestamp dating the creation of this document.                                                                                                                                              |
| `context`   | The "context" that this document is attached to, which controls which capabilities this document allows.<br>See [\<enum:document-context\>](../enums/document-context.md) and [Capabilities](../capabilities.md). |
| `version`   | A semver version string dictating the version of the Game Jolt Content Document format used for this document. Currently always `"1.0.0"`.<br>See [Versions](../versions.md) for version differences.             |
| `content`   | A list of child objects of the document.<br>See [\<type:content-object\>](content-object.md).                                                                                                                     |
| `hydration` | A list of hydration entries for this document.<br>See [\<type:content-hydration-entry\>](content-hydration-entry.md) and [Hydration](../hydration.md).                                                            |
