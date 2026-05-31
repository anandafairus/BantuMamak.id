---
name: Accessible Serenity
colors:
  surface: '#f8f9fa'
  surface-dim: '#d9dadb'
  surface-bright: '#f8f9fa'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f4f5'
  surface-container: '#edeeef'
  surface-container-high: '#e7e8e9'
  surface-container-highest: '#e1e3e4'
  on-surface: '#191c1d'
  on-surface-variant: '#434655'
  inverse-surface: '#2e3132'
  inverse-on-surface: '#f0f1f2'
  outline: '#737686'
  outline-variant: '#c3c6d7'
  surface-tint: '#0053db'
  primary: '#004ac6'
  on-primary: '#ffffff'
  primary-container: '#2563eb'
  on-primary-container: '#eeefff'
  inverse-primary: '#b4c5ff'
  secondary: '#006c49'
  on-secondary: '#ffffff'
  secondary-container: '#6cf8bb'
  on-secondary-container: '#00714d'
  tertiary: '#784b00'
  on-tertiary: '#ffffff'
  tertiary-container: '#996100'
  on-tertiary-container: '#ffeedd'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dbe1ff'
  primary-fixed-dim: '#b4c5ff'
  on-primary-fixed: '#00174b'
  on-primary-fixed-variant: '#003ea8'
  secondary-fixed: '#6ffbbe'
  secondary-fixed-dim: '#4edea3'
  on-secondary-fixed: '#002113'
  on-secondary-fixed-variant: '#005236'
  tertiary-fixed: '#ffddb8'
  tertiary-fixed-dim: '#ffb95f'
  on-tertiary-fixed: '#2a1700'
  on-tertiary-fixed-variant: '#653e00'
  background: '#f8f9fa'
  on-background: '#191c1d'
  surface-variant: '#e1e3e4'
typography:
  headline-2xl:
    fontFamily: Plus Jakarta Sans
    fontSize: 48px
    fontWeight: '800'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-xl:
    fontFamily: Plus Jakarta Sans
    fontSize: 36px
    fontWeight: '700'
    lineHeight: 44px
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 30px
    fontWeight: '700'
    lineHeight: 38px
  body-xl:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '500'
    lineHeight: 32px
  body-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 20px
    fontWeight: '400'
    lineHeight: 28px
  label-xl:
    fontFamily: Plus Jakarta Sans
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  touch-target-min: 56px
  margin-edge: 24px
  gutter: 16px
  stack-gap: 24px
---

## Brand & Style
The design system focuses on radical accessibility for an elderly demographic, blending **Glassmorphism** with high-legibility **Minimalism**. The brand personality is patient, reliable, and clear, designed to reduce cognitive load while providing a premium, modern feel. 

The visual mood is "calmly efficient." By utilizing soft blurs and high-contrast color pairings, the interface provides distinct "tactile" layers that help users with diminished visual acuity distinguish between interactive surfaces and background information. The emotional response should be one of confidence and ease—turning the chore of grocery management into a simple, friction-less experience.

## Colors
The palette is rooted in high-contrast functionalism. 

- **Primary (Blue):** Used for navigation and main actions. It provides a sense of institutional trust.
- **Success (Emerald-500):** Exclusively reserved for the 'Bought' action, providing a clear positive signal.
- **Warning (Amber-400):** Used for 'Skip' or 'Modify' actions, offering high visibility without the alarm of red.
- **Background (Gray-50):** A soft, off-white base that reduces screen glare.
- **Surface (Pure White):** All cards and interaction containers are pure white to maximize the contrast against text and background.

## Typography
We use **Plus Jakarta Sans** for its generous x-height and open counters, which significantly improve legibility for older eyes. 

The scale is intentionally oversized. Body text starts at 20px, ensuring that even "fine print" is easily readable. Headlines are massive to provide immediate context upon entering a screen. Line heights are kept loose (minimum 1.4x) to prevent lines of text from blurring together. Avoid all font weights below 400.

## Layout & Spacing
The layout follows a **Fixed Grid** model on mobile to ensure consistent, predictable tap areas. 

- **Touch Targets:** Every interactive element has a minimum height of 56px (`h-14`) to accommodate users with limited dexterity.
- **Margins:** A wide 24px side margin keeps content away from the edges of the device where it might be harder to read or tap.
- **Vertical Rhythm:** Elements are stacked with a generous 24px gap to clearly delineate separate items and avoid accidental multi-taps.
- **Safe Areas:** High-contrast buttons are fixed to the bottom of the viewport using a glassmorphic blur bar to ensure critical actions are always within thumb-reach.

## Elevation & Depth
Depth is created through **Glassmorphism** and **Soft Shadows** rather than complex borders. 

1.  **Base Layer:** Gray-50 background.
2.  **Card Layer:** Pure white surfaces with a subtle 12% opacity soft shadow (Blue-tinted) to "lift" the card off the page.
3.  **Action Layer:** Floating action bars use a `backdrop-blur-md` effect with a 70% white tint. This creates a "frosted glass" look that keeps the focus on the foreground button while maintaining a sense of place within the list.
4.  **Tactile Response:** When pressed, buttons should physically "sink" using a scale-95 transform, providing immediate haptic-visual feedback.

## Shapes
The shape language is **Rounded** (0.5rem base), scaling up to 1.5rem for large cards. This avoids the "aggressive" feel of sharp corners while maintaining more structure than a full pill-shape. 

Large corner radii are used on main product cards to make the interface feel friendly and approachable. Secondary elements like input fields and tags use the 0.5rem base to maintain a clear, geometric distinction from the larger structural cards.

## Components

### Buttons
Primary buttons are high-contrast (Blue-600 with White text) and full-width. They must include a clear icon alongside the text for dual-encoding of meaning. The "Bought" (Emerald) and "Skip" (Amber) buttons should be the largest interactive elements in the app.

### Product Cards
Cards feature a pure white background with a large product image on the left and `headline-lg` text. The card itself acts as the primary "Swipe" container. 

### Input Fields
Inputs use a light gray stroke (Gray-200) that thickens to 3px (Blue-600) when focused. The font size within inputs must be at least `body-xl` (24px) to ensure users can see what they are typing.

### Chips & Badges
Used for categories (e.g., "Dairy", "Produce"). These are non-interactive or toggle-only and use `label-xl` typography. They feature high-contrast background tints (e.g., light blue background with dark blue text) for maximum readability.

### Swipe Indicators
Visible high-contrast "cues" (arrows or icons) should peek from the sides of the product cards to teach the swipe gesture without requiring a tutorial.