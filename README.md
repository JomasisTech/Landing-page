# DetroPick — AI Product Promotion Masterclass Landing Page

Version 1.8.0 — September 19, 2026.

## What changed in 1.8.0
- Replaced the static hero promotional image with a featured real-brand Vimeo example.
- Featured video: Hussy Footwear — `https://vimeo.com/1228383355`.
- Added clear labeling: “Real brand example” and “Promotional video created for Hussy Footwear.”
- The Hussy Footwear example is now the first visual proof visitors see after the hero copy.
- Updated the following sample-video section to “More examples” so the page hierarchy is clear and the Hussy Footwear project is treated as the featured example.
- Removed the old hero promotional image asset because it is no longer used.
- Preserved the existing three additional Vimeo examples, Selar checkout, curriculum, course-preview screenshot, responsive layout, one-video-at-a-time playback, fullscreen behavior, lazy Vimeo loading, and accessibility behavior.

## Files
- `index.html` — complete landing page
- `course-modules-preview.jpg` — genuine course-module preview screenshot supplied for the landing page

## Deployment
Upload the contents of this ZIP directly to the site root. There is no wrapping folder.

## Featured brand example
- Hussy Footwear — `https://vimeo.com/1228383355`

## Additional sample videos
1. CeraVe — `https://vimeo.com/1225432485`
2. EltaMD — `https://vimeo.com/1225432483`
3. ELEMIS — `https://vimeo.com/1225432482`

## Checkout
The landing page uses the existing Selar checkout URL for the ₦3,800 masterclass.

## QA notes
- Featured Hussy Footwear video uses the same Vimeo player implementation as the existing sample videos.
- The hero video is a `.video-card`, so it receives the existing lazy Vimeo API loading, play/pause, one-video-at-a-time behavior, fullscreen support, and highest-available-quality request.
- No static hero image remains referenced in `index.html`.
- The old hero image asset is intentionally omitted from the deployment ZIP.
- All local assets referenced by the page are included in the ZIP.
- Internal links and Selar checkout links are preserved.
