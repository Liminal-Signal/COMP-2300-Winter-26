---
title: "Media Embed Guide"
date: 2026-01-16
publish: false
tags:
  - guide
  - media
---

# Media embed guide

Use this as a copy/paste reference for posts. Paths below are **relative to this file**.

## Images

### Local image

![Sample image placeholder with a frame and label](media/sample-image.svg)

### Bounded image size (recommended)

Use the `post-photo` class so images don't render too large:

```markdown
![Sample image placeholder](media/sample-image.svg){ .post-photo }
```

Size variants:

```markdown
![Small image](media/sample-image.svg){ .post-photo .post-photo--sm }
![Large image](media/sample-image.svg){ .post-photo .post-photo--lg }
```

### Image with caption

<figure>
  <img class="post-photo" src="media/sample-image.svg" alt="Sample image placeholder with a frame and label">
  <figcaption>Caption text for the image.</figcaption>
</figure>

### Link to the image file

[Download the full-resolution image](media/sample-image.svg)

## Links to media files

You can link to any file you include alongside your post:

- [Lab report PDF](media/sample-report.pdf)
- [Dataset ZIP](media/sample-data.zip)

## Video

Video embeds are disabled in this site. Link out instead:

```markdown
[Watch the video on YouTube](https://www.youtube.com/watch?v=LXb3EKWsInQ)
```

## Audio (HTML embed)

```html
<audio controls>
  <source src="media/sample-audio.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
</audio>
```

## Tips

- Keep file sizes small; large files slow the site.
- Use clear, descriptive alt text for images.
- Images open in a lightbox if the site enables `mkdocs-glightbox`.
- Put media files in a `media/` folder next to your post and link them like `media/filename.ext`.
