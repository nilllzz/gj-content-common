# Game Jolt Content Document format

The Game Jolt Content Document is a tree-node based document that stores information about content on Game Jolt.

"Content" includes comments, the lead/article of a post, a user's bio, and more. Content on Game Jolt is also not just rich text, it can include images, videos or even more complex data structures.

For the purposes of this documentation, the document is expressed as a JSON object, but it can theoretically be adapted to any data format that can be serialized/deserialized to/from JSON.

## Example document

This is a simple "Hello World" document that will create a single paragraph with the text "Hello, World!" inside.

```
{
    "createdOn": "1640154652257",
    "context": "game-comment",
    "version": "1.0.0",
    "content": [
        {
            "type": "paragraph",
            "content": [
                {
                    "type": "text",
                    "text": "Hello, World!"
                }
            ]
        }
    ],
    "hydration": []
}
```

An HTML approximation of the above document may look like this:

```
<p>
    <span>Hello, World!</span>
</p>
```

For more details on the Content Document type, see [\<type:content-document\>](types/content-document.md).
