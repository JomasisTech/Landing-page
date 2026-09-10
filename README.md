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


Video card separation update (September 10, 2026):
- Each sample video now sits in a subtle individual card with a light border, soft elevation and consistent spacing.
- The card treatment visually separates the three examples without introducing heavy divider lines or changing the existing visual language.
- Video playback, fullscreen behavior, Vimeo quality selection, one-video-at-a-time playback and the orphan-iframe protection are unchanged.


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

## Final visual separation review (September 10, 2026)
- Each sample video now sits in a subtle individual card with light separation, spacing, rounded corners, and restrained elevation.
- The card styling is CSS-only and does not add JavaScript or external assets.
- The card itself does not use CSS `transform`, preserving the existing fullscreen fallback behavior; only the inner video frame retains its existing hover lift.
- Existing Vimeo quality selection, one-video-at-a-time playback, orphan-iframe protection, and fullscreen behavior remain unchanged.
