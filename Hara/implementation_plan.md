# Custom Dropdown Implementation Plan

This plan aims to replace the native HTML `<select>` inputs with a more professional, formal, and user-friendly custom dropdown UI, completely built using Vanilla JavaScript and CSS as per your rules.

## Proposed Changes

We will build a custom JavaScript class that "wraps" the existing `<select>` elements. This means the underlying logic of your application won't break, but the user will see a beautifully styled, professional dropdown that also includes a search bar for better UX.

### 1. CSS Styling (`Hara/style.css`)
[MODIFY] `style.css`
- Add a professional, brand-compliant color scheme (deep blues, clean whites, subtle shadows) for the custom dropdowns.
- Add styles for:
  - The dropdown trigger (the box you click).
  - The dropdown menu (the list of options with a smooth fade-in animation).
  - A search/filter input inside the menu to easily find a family or registration number.
  - Hover states and selected states.

### 2. JavaScript Logic (`Hara/index.html`)
[MODIFY] `index.html` (Script section)
- Add a new Vanilla JS class `CustomSelect`.
- This script will automatically find your existing `<select>` elements (`familyName`, `familyGender`, `regNumber`, `gender`), hide them, and build the custom UI in their place.
- Whenever the user clicks an option in the new custom UI, it will update the hidden `<select>` and trigger the necessary search functions automatically.
- **Important**: When the registration numbers are dynamically updated (from our previous task), the custom dropdown will also automatically rebuild its list of options.

## User Review Required

> [!IMPORTANT]
> - Do you want a search bar inside the dropdown to filter the options? (Highly recommended for UX, especially for the long list of families and registration numbers).
> - Do you prefer a specific color for the dropdown focus states, or should I stick to the primary `#1a237e` (deep blue) already used in your navigation?

Please approve this plan or let me know if you want any adjustments before I write the code!
