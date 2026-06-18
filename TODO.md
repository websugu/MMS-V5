# TODO - Index UI/UX Modernization

## Step 1

Update `index.html` CSS for a more advanced, modern look:

- Improve hero responsiveness (use clamp-based sizing)
- Ensure hero text remains readable over animated image background

## Step 2

Refine mobile UX:

- Improve navbar mobile menu usability (no clipping, better spacing)
- Add touch-friendly button/card spacing

## Step 3

Accessibility improvements:

- Add `prefers-reduced-motion` support (disable scroll animations)
- Add `:focus-visible` styles for interactive elements

## Step 4

Keep compatibility with existing JS:

- Do not rename IDs/classes used by `JS/app.js` (`#products-container`, `#search-input`, `#product-count`, etc.)

## Step 5

Manual QA checklist:

- Test on mobile widths (~375px / ~414px)
- Verify search, chips, product cards render
- Verify navbar mobile open/close
- Verify toast still shows correctly
