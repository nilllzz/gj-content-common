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

| Field       | Description                                                                                                                                                                                                             |
| ----------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `createdOn` | Millisecond-accurate timestamp dating the creation of this document.                                                                                                                                                    |
| `context`   | The "context" that this document is attached to, which controls which capabilities this document allows.<br>See [\<enum:document-context\>](/docs/enums/document-context.md) and [Capabilities](/docs/capabilities.md). |
| `version`   | A semver version string dictating the version of the Game Jolt Content Document format used for this document. Currently always `"1.0.0"`.<br>See [Versions](/docs/versions.md) for version differences.                |
| `content`   | A list of child objects of the document.<br>See [\<type:content-object\>](/docs/types/content-object.md).                                                                                                               |
| `hydration` | A list of hydration entries for this document.<br>See [\<type:content-hydration-entry\>](/docs/types/content-hydration-entry.md) and [Hydration](/docs/hydration.md).                                                   |
