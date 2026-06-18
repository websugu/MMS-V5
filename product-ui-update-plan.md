# Product page UI/UX modernization plan

## Goal

Improve `product.html` look/feel using modern design patterns while staying compatible with your existing `JS/product.js` (which renders almost all content dynamically).

## What we’ll change

1. Add modern gallery thumbnail styles + spacing.
2. Add styling for gallery zoom/modal injected by `JS/product.js` (modal overlay, stage, arrows, thumb active state).
3. Add better selected variant box visuals.
4. Add skeleton improvements (already partly present).
5. Improve action buttons layout (subtle elevation/hover, consistent responsive behavior).
6. Add sticky “bottom action bar” on mobile.

## Files to edit

- `product.html` (CSS only + small static HTML container if needed)

## Implementation details

- CSS: define classes/IDs used by `JS/product.js`:
  - `#product-thumbs`, `.product-thumb-btn`
  - `#gallery-modal-overlay` and modal classes created in JS
  - `.selected-info-box`, `.action-buttons`, `.btn*`
- Mobile bar:
  - Add a `<div id="mobile-action-bar">` with Add-to-cart / Buy-now buttons.
  - JS will keep using existing buttons; bar will mirror their disabled/enabled state using event listeners.

## Follow-up

After UI patch, verify:

- Product page loads (no blank)
- Gallery thumbs appear when `galleryUrls` exists
- Clicking thumbnail opens modal and arrows work
- Mobile bar doesn’t overlap toast/WhatsApp fab
