Many social networks display a rich preview for your website when a user shares a link to it.  Using [[Metadata]], you can customize how your notes appear in the preview.

## Description

Obsidian automatically generates a description based on the note content, but you can provide your own using `description`.

```yaml
---
description: An introduction to our solar system.
---
```

> [!note] Meta tags
> `description` overrides the auto-generated description in `<meta name="description" content="...">` and the equivalents for `og:description` and `twitter:description`.

## Image

You can use a custom image for the link preview, by adding `image` or `cover` with a path to the image.

The path can be a relative path within your vault:

```yaml
---
cover: Attachments/Cover.png
---
```

Or, an absolute URL:

```yaml
---
image: https://example.com/image.png
---
```

`image` and `cover` are identical. Only use one of them.

> [!note] Meta tags
> `image` and `cover` overrides the auto-generated image in `<meta property="og:image" content="...">`.
