# slides2pdf

Browser-based MP4 slide extractor for research, lectures, webinars, and video review workflows.

`slides2pdf` detects slide-like scene changes in an MP4 video and exports the captured frames as WebP/PNG images or a single PDF. It runs entirely in the browser, so videos are processed locally and are not uploaded to a server.

Live demo: https://lazy3128-design.github.io/slides2pdf/

## Why This Exists

When researching webinars, product demos, online courses, talks, or recorded presentations, it is often useful to turn a long video into a set of reviewable slides. Manual screenshots are slow, and full video transcription does not preserve visual layout.

`slides2pdf` helps convert video-based slide content into lightweight image/PDF materials that can be reviewed, annotated, summarized, or archived.

## Features

- Detects visual changes between video frames and captures likely slide transitions
- Exports captured frames as WebP or PNG
- Generates a PDF from extracted slides
- Downloads extracted images as ZIP files
- Splits large ZIP output into smaller volumes
- Supports multiple videos in one session
- Lets users exclude moving regions such as presenter camera overlays or captions
- Adjustable sensitivity for fewer or more extracted slides
- Runs locally in the browser with no installation

## Use Cases

- Researching webinars, lectures, demos, and conference talks
- Turning recorded presentations into reviewable slide material
- Extracting visual references from product walkthrough videos
- Creating quick PDF summaries from screen-recorded slide decks
- Preparing source material for qualitative analysis or note-taking

## Privacy

The tool processes videos locally in the user's browser. It does not upload video files to a server. The current implementation is a static HTML page using browser APIs.

## How To Use

1. Open the live demo.
2. Drag and drop one or more MP4/video files.
3. Optionally mark areas to ignore, such as a presenter camera overlay.
4. Start analysis.
5. Download extracted images as ZIP or generate a PDF.

## Current Limitations

- Detection is based on visual frame differences, not semantic slide understanding.
- Highly animated slides may produce extra captures.
- Subtle slide changes may require higher sensitivity.
- Very long videos can take time because processing happens in the browser.
- Browser memory limits may affect very large files.

## Roadmap

- Improve slide change detection for animated decks
- Add duplicate slide cleanup
- Add optional OCR-assisted slide naming
- Add a batch summary workflow for research notes
- Add test videos and benchmark examples
- Improve accessibility and keyboard navigation
- Package the tool as an installable PWA

## Maintainer

Maintained by [lazy3128-design](https://github.com/lazy3128-design).

## License

MIT License.
