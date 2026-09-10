# DetroPick — AI Product Promotion Masterclass Landing Page

Final deployment-ready landing page with the three selected sample videos embedded from Vimeo.

## Files
- `index.html` — complete landing page

## Deployment
Upload the contents of this ZIP directly to the site root. There is no wrapping folder.

## Sample videos
The landing page uses three dedicated 9:16 video slots in this order:
1. CeraVe — `https://vimeo.com/1225432485`
2. EltaMD — `https://vimeo.com/1225432483`
3. ELEMIS — `https://vimeo.com/1225432482`

## Checkout
The landing page uses the existing Selar checkout URL for the ₦3,800 masterclass.

## Final QA
- Three Vimeo embeds verified and mapped to the selected videos.
- Video frames remain portrait 9:16.
- No external font dependency.
- No unresolved DM Sans/Manrope font references.
- All internal section links resolve.
- Checkout links use the existing Selar URL.
- Core free-access/no-paid-subscription messaging retained.


Final review update (September 2026):
- CTA now says “See the examples” because the page contains three video examples.
- Reviewed the deployed mobile layout and adjusted mobile hero/video spacing slightly for cleaner breathing room.
- Vimeo embeds include inline playback behavior for mobile devices.
- The hero device illustration remains intentionally device-neutral rather than imitating a specific iPhone model, keeping the design evergreen and focused on the AI product-promotion concept.


Final video behavior update:
- Center play control appears before playback.
- While playing, the pause control fades away after a short delay and reappears when the visitor taps the video.
- The center control pauses/resumes playback.
- Only one sample video plays at a time.
- Fullscreen remains available for the complete portrait video.
- Internal navigation no longer leaves the page stuck at the video section after refresh; the landing page returns to the hero on reload.


Duplicate/orphan video fix (September 10, 2026):
- Vimeo iframe positioning is now limited to iframes inside `.video-frame`.
- Any stray iframe inserted directly under a `.video-card` is hidden/removed so it cannot appear over the hero.
- A MutationObserver also cleans up late-injected orphan iframes from third-party video scripts.
- The hero section contains no video iframe and remains unaffected by the sample-video embeds.


Version 1.3.0 (September 10, 2026):
- Added subtle individual cards around the three sample videos so each example is visually separated without introducing heavy divider lines.
- Kept the video frames portrait and preserved the existing Vimeo controls, fullscreen behavior, one-video-at-a-time playback, and highest-available-quality request.
- Optimized the orphan-iframe MutationObserver so it reacts to newly added nodes instead of rescanning the entire document for every DOM mutation.
- Expanded reduced-motion handling to cover video/card hover animations as well as CTA and video controls.

Version 1.4.0 — speed optimization (September 10, 2026):
- Vimeo Player API is no longer loaded during the initial page load; it is fetched only when a sample-video card approaches the viewport.
- Vimeo iframes are created only for cards that are about to be viewed, reducing initial third-party network requests and main-thread work.
- Removed the fixed SVG turbulence/noise overlay to reduce paint and compositing work.
- Removed CSS backdrop blur from the fixed header/mobile CTA and the unnecessary hero glow blur to reduce GPU/compositing cost.
- Added lightweight `content-visibility:auto` containment to video cards so below-the-fold video content is cheaper to render.
- Preserved one-video-at-a-time playback, highest-available-quality selection, fullscreen, orphan-iframe protection, responsive layout, and reduced-motion behavior.
- No external font dependency and no additional image assets were introduced.
