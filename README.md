# flyfag-shorts

Rendered explainer shorts for the M01 flyfag theory app: one 8–19 second clip per
memorization fact, in Norwegian and English, 151 facts × 2 languages = 302 MP4s.

The app plays these straight from this repository with a plain `<video>` tag:

```
https://raw.githubusercontent.com/alsosocial/flyfag-shorts/main/<factId>.<lang>.mp4
```

Naming is fixed: `<factId>.<lang>.mp4` where `lang` is `no` or `en`, and
`factId` is the same id the app uses for the flashcard.

## Generated, do not edit

These files are produced, not authored. The source of truth for facts, narration
and scene definitions is the JSON specs in the app repository; the videos come
from `tools/video/shorts/fast_render.py`, and `publish_github.sh` copies
`dist/*.mp4` here and pushes.

To change a video, fix the spec or the renderer and re-publish. Editing an MP4
here directly will be overwritten on the next publish.

Everything here is unlisted in spirit — public only because the app needs a
stable, cheap file URL, not because it is a channel.
