# Fixing AI Hallucinations With Kakeya Logic

**Goal:** host the PeAIce / Love Labs index page with its slide deck and recordings so it can be embedded on lovelabslca.com.

**Why:** the site editor can't host a 166 MB bundle of slides and audio. GitHub Pages serves it as static files at a stable URL that can be embedded with an iframe.

**How it's checked:** the Pages URL returns 200, and curl confirms slides/slide-01.png, slides/slide-22.png, both .m4a recordings (content-length) and the .pptx return 200, with no X-Frame-Options or frame-ancestors header blocking embedding.

`index.html` is published exactly as written.
