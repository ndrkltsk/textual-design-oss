# Design System Documentation

## 1. Design & Brand Identity

### Design Philosophy and Guiding Principles
- **Simplicity First**: Clean, uncluttered interfaces that prioritize content and functionality
- **Approachable Technology**: Making complex app-building feel accessible and friendly
- **Warmth Through Color**: Using warm gradients and orange accents to create an inviting atmosphere
- **Progressive Disclosure**: Revealing complexity only when needed

### Visual Style Direction
- Modern, clean, and minimal with warm accents
- Soft, organic feeling through gradient backgrounds and rounded shapes
- Professional yet approachable - balancing corporate reliability with startup energy
- Light and airy with generous whitespace

### Overall Mood and Tone
- Optimistic and encouraging
- Professional but not cold
- Innovative yet trustworthy
- Welcoming to non-technical users

### Brand Personality Expressed Through UI
- Friendly: Warm orange tones and soft gradients
- Capable: Clean typography and structured layouts
- Modern: Contemporary design patterns and smooth animations
- Accessible: Clear hierarchy and intuitive navigation

### Visual Language Consistency
- Consistent use of rounded corners across all elements
- Unified color palette with orange as the primary accent
- Consistent spacing rhythm throughout
- Predictable component behavior and placement

---

## 2. Design Tokens

### Colors

#### Primary Palette
```css
--color-primary-orange: #F97316;
--color-primary-orange-light: #FB923C;
--color-primary-orange-dark: #EA580C;
--color-primary-orange-50: #FFF7ED;
--color-primary-orange-100: #FFEDD5;
--color-primary-orange-200: #FED7AA;
--color-primary-orange-300: #FDBA74;
--color-primary-orange-400: #FB923C;
--color-primary-orange-500: #F97316;
--color-primary-orange-600: #EA580C;
--color-primary-orange-700: #C2410C;
```

#### Secondary/Accent Colors
```css
--color-accent-lime: #D4F94E;
--color-accent-lime-light: #E4FF6B;
--color-accent-lime-dark: #BEF026;
--color-accent-yellow: #FEF08A;
--color-accent-peach: #FECACA;
--color-accent-mint: #A7F3D0;
--color-accent-lavender: #DDD6FE;
--color-accent-sky: #BAE6FD;
```

#### Neutral/Grayscale Scale
```css
--color-gray-50: #FAFAFA;
--color-gray-100: #F4F4F5;
--color-gray-200: #E4E4E7;
--color-gray-300: #D4D4D8;
--color-gray-400: #A1A1AA;
--color-gray-500: #71717A;
--color-gray-600: #52525B;
--color-gray-700: #3F3F46;
--color-gray-800: #27272A;
--color-gray-900: #18181B;
--color-gray-950: #09090B;
```

#### Semantic Colors
```css
/* Success */
--color-success: #22C55E;
--color-success-light: #86EFAC;
--color-success-dark: #16A34A;
--color-success-bg: #DCFCE7;

/* Warning */
--color-warning: #F59E0B;
--color-warning-light: #FCD34D;
--color-warning-dark: #D97706;
--color-warning-bg: #FEF3C7;

/* Error */
--color-error: #EF4444;
--color-error-light: #FCA5A5;
--color-error-dark: #DC2626;
--color-error-bg: #FEE2E2;

/* Info */
--color-info: #3B82F6;
--color-info-light: #93C5FD;
--color-info-dark: #2563EB;
--color-info-bg: #DBEAFE;
```

#### Background Colors
```css
--bg-primary: #FFFFFF;
--bg-secondary: #FAFAFA;
--bg-tertiary: #F4F4F5;
--bg-card: #FFFFFF;
--bg-sidebar: #FFFFFF;
--bg-overlay: rgba(0, 0, 0, 0.5);
--bg-modal: #FFFFFF;
--bg-input: #FFFFFF;
--bg-input-disabled: #F4F4F5;
--bg-hover: #F4F4F5;
--bg-active: #E4E4E7;
--bg-selected: #FFF7ED;
```

#### Text Colors
```css
--text-primary: #18181B;
--text-secondary: #52525B;
--text-muted: #71717A;
--text-disabled: #A1A1AA;
--text-inverse: #FFFFFF;
--text-link: #F97316;
--text-link-hover: #EA580C;
--text-error: #DC2626;
--text-success: #16A34A;
```

#### Border Colors
```css
--border-default: #E4E4E7;
--border-light: #F4F4F5;
--border-dark: #D4D4D8;
--border-focus: #F97316;
--border-error: #EF4444;
--border-success: #22C55E;
```

#### Gradient Definitions
```css
/* Hero Gradient - Orange to Lavender */
--gradient-hero-1: linear-gradient(135deg, #FDBA74 0%, #FED7AA 25%, #DDD6FE 75%, #A7F3D0 100%);

/* Hero Gradient - Peach to Mint */
--gradient-hero-2: linear-gradient(135deg, #FECACA 0%, #FED7AA 30%, #FEF08A 50%, #A7F3D0 100%);

/* Hero Gradient - Orange Dominant */
--gradient-hero-3: linear-gradient(180deg, #FB923C 0%, #F97316 50%, #EA580C 100%);

/* Hero Gradient - Sky to Mint */
--gradient-hero-4: linear-gradient(135deg, #BAE6FD 0%, #A7F3D0 100%);

/* Card Gradient - Soft Orange */
--gradient-card-orange: linear-gradient(135deg, #FFEDD5 0%, #FED7AA 100%);

/* Card Gradient - Soft Yellow */
--gradient-card-yellow: linear-gradient(135deg, #FEF9C3 0%, #FEF08A 100%);

/* Card Gradient - Soft Mint */
--gradient-card-mint: linear-gradient(135deg, #D1FAE5 0%, #A7F3D0 100%);

/* Card Gradient - Soft Sky */
--gradient-card-sky: linear-gradient(135deg, #E0F2FE 0%, #BAE6FD 100%);

/* Overlay Gradient */
--gradient-overlay: linear-gradient(180deg, rgba(255,255,255,0) 0%, rgba(255,255,255,0.8) 100%);
```

### Typography

#### Font Families
```css
--font-primary: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
--font-secondary: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
--font-monospace: 'SF Mono', 'Monaco', 'Inconsolata', 'Fira Code', monospace;
--font-display: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
```

#### Font Weights
```css
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--font-weight-extrabold: 800;
```

#### Type Scale
```css
/* Display sizes - for hero headings */
--font-size-display-2xl: 72px;   /* 4.5rem */
--font-size-display-xl: 60px;    /* 3.75rem */
--font-size-display-lg: 48px;    /* 3rem */
--font-size-display-md: 36px;    /* 2.25rem */

/* Heading sizes */
--font-size-h1: 36px;   /* 2.25rem */
--font-size-h2: 30px;   /* 1.875rem */
--font-size-h3: 24px;   /* 1.5rem */
--font-size-h4: 20px;   /* 1.25rem */
--font-size-h5: 18px;   /* 1.125rem */
--font-size-h6: 16px;   /* 1rem */

/* Body sizes */
--font-size-body-lg: 18px;   /* 1.125rem */
--font-size-body-md: 16px;   /* 1rem */
--font-size-body-sm: 14px;   /* 0.875rem */
--font-size-body-xs: 12px;   /* 0.75rem */

/* Utility sizes */
--font-size-caption: 12px;   /* 0.75rem */
--font-size-label: 14px;     /* 0.875rem */
--font-size-overline: 11px;  /* 0.6875rem */
```

#### Line Heights
```css
--line-height-display: 1.1;
--line-height-heading: 1.2;
--line-height-body: 1.5;
--line-height-relaxed: 1.625;
--line-height-loose: 1.75;
--line-height-tight: 1.25;
```

#### Letter Spacing
```css
--letter-spacing-tighter: -0.05em;
--letter-spacing-tight: -0.025em;
--letter-spacing-normal: 0;
--letter-spacing-wide: 0.025em;
--letter-spacing-wider: 0.05em;
--letter-spacing-widest: 0.1em;
```

#### Paragraph Spacing
```css
--paragraph-spacing-sm: 12px;
--paragraph-spacing-md: 16px;
--paragraph-spacing-lg: 24px;
```

#### Text Styles Catalog
```css
/* Display - Hero Headlines */
.text-display-2xl {
  font-size: 72px;
  font-weight: 700;
  line-height: 1.1;
  letter-spacing: -0.025em;
}

.text-display-xl {
  font-size: 60px;
  font-weight: 700;
  line-height: 1.1;
  letter-spacing: -0.025em;
}

.text-display-lg {
  font-size: 48px;
  font-weight: 700;
  line-height: 1.1;
  letter-spacing: -0.02em;
}

/* Headings */
.text-h1 {
  font-size: 36px;
  font-weight: 700;
  line-height: 1.2;
  letter-spacing: -0.02em;
}

.text-h2 {
  font-size: 30px;
  font-weight: 600;
  line-height: 1.2;
  letter-spacing: -0.015em;
}

.text-h3 {
  font-size: 24px;
  font-weight: 600;
  line-height: 1.25;
  letter-spacing: -0.01em;
}

.text-h4 {
  font-size: 20px;
  font-weight: 600;
  line-height: 1.3;
}

.text-h5 {
  font-size: 18px;
  font-weight: 600;
  line-height: 1.4;
}

.text-h6 {
  font-size: 16px;
  font-weight: 600;
  line-height: 1.4;
}

/* Body Text */
.text-body-lg {
  font-size: 18px;
  font-weight: 400;
  line-height: 1.625;
}

.text-body-md {
  font-size: 16px;
  font-weight: 400;
  line-height: 1.5;
}

.text-body-sm {
  font-size: 14px;
  font-weight: 400;
  line-height: 1.5;
}

/* Utility Text */
.text-caption {
  font-size: 12px;
  font-weight: 400;
  line-height: 1.4;
  color: var(--text-muted);
}

.text-label {
  font-size: 14px;
  font-weight: 500;
  line-height: 1.4;
}

.text-overline {
  font-size: 11px;
  font-weight: 600;
  line-height: 1.4;
  letter-spacing: 0.1em;
  text-transform: uppercase;
}
```

### Spacing

#### Base Unit
```css
--spacing-unit: 4px;
```

#### Spacing Scale
```css
--spacing-0: 0;
--spacing-0.5: 2px;
--spacing-1: 4px;
--spacing-1.5: 6px;
--spacing-2: 8px;
--spacing-2.5: 10px;
--spacing-3: 12px;
--spacing-3.5: 14px;
--spacing-4: 16px;
--spacing-5: 20px;
--spacing-6: 24px;
--spacing-7: 28px;
--spacing-8: 32px;
--spacing-9: 36px;
--spacing-10: 40px;
--spacing-11: 44px;
--spacing-12: 48px;
--spacing-14: 56px;
--spacing-16: 64px;
--spacing-20: 80px;
--spacing-24: 96px;
--spacing-28: 112px;
--spacing-32: 128px;
--spacing-36: 144px;
--spacing-40: 160px;
--spacing-44: 176px;
--spacing-48: 192px;
```

#### Component Internal Padding Patterns
```css
/* Button padding */
--padding-button-sm: 8px 16px;
--padding-button-md: 10px 20px;
--padding-button-lg: 12px 24px;
--padding-button-xl: 14px 28px;

/* Card padding */
--padding-card-sm: 16px;
--padding-card-md: 24px;
--padding-card-lg: 32px;

/* Input padding */
--padding-input-sm: 8px 12px;
--padding-input-md: 10px 14px;
--padding-input-lg: 12px 16px;

/* Modal padding */
--padding-modal-header: 24px;
--padding-modal-body: 24px;
--padding-modal-footer: 16px 24px;
```

#### Layout Margins and Gaps
```css
/* Section spacing */
--section-gap-sm: 48px;
--section-gap-md: 64px;
--section-gap-lg: 96px;
--section-gap-xl: 128px;

/* Content gaps */
--gap-xs: 8px;
--gap-sm: 12px;
--gap-md: 16px;
--gap-lg: 24px;
--gap-xl: 32px;

/* Grid gaps */
--grid-gap-sm: 16px;
--grid-gap-md: 24px;
--grid-gap-lg: 32px;
```

### Effects

#### Shadow Definitions
```css
/* Elevation levels */
--shadow-none: none;

--shadow-xs: 0 1px 2px 0 rgba(0, 0, 0, 0.05);

--shadow-sm: 0 1px 3px 0 rgba(0, 0, 0, 0.1),
             0 1px 2px -1px rgba(0, 0, 0, 0.1);

--shadow-md: 0 4px 6px -1px rgba(0, 0, 0, 0.1),
             0 2px 4px -2px rgba(0, 0, 0, 0.1);

--shadow-lg: 0 10px 15px -3px rgba(0, 0, 0, 0.1),
             0 4px 6px -4px rgba(0, 0, 0, 0.1);

--shadow-xl: 0 20px 25px -5px rgba(0, 0, 0, 0.1),
             0 8px 10px -6px rgba(0, 0, 0, 0.1);

--shadow-2xl: 0 25px 50px -12px rgba(0, 0, 0, 0.25);

/* Specific component shadows */
--shadow-card: 0 1px 3px 0 rgba(0, 0, 0, 0.08),
               0 1px 2px -1px rgba(0, 0, 0, 0.08);

--shadow-card-hover: 0 10px 15px -3px rgba(0, 0, 0, 0.08),
                     0 4px 6px -4px rgba(0, 0, 0, 0.08);

--shadow-dropdown: 0 4px 6px -1px rgba(0, 0, 0, 0.1),
                   0 2px 4px -2px rgba(0, 0, 0, 0.1);

--shadow-modal: 0 25px 50px -12px rgba(0, 0, 0, 0.25);

--shadow-button: 0 1px 2px 0 rgba(0, 0, 0, 0.05);

/* Focus ring shadow */
--shadow-focus: 0 0 0 3px rgba(249, 115, 22, 0.2);
--shadow-focus-error: 0 0 0 3px rgba(239, 68, 68, 0.2);
```

#### Blur Effects
```css
--blur-none: 0;
--blur-sm: 4px;
--blur-md: 8px;
--blur-lg: 16px;
--blur-xl: 24px;
--blur-2xl: 40px;
--blur-backdrop: 8px;
```

#### Opacity Values
```css
--opacity-0: 0;
--opacity-5: 0.05;
--opacity-10: 0.1;
--opacity-20: 0.2;
--opacity-25: 0.25;
--opacity-30: 0.3;
--opacity-40: 0.4;
--opacity-50: 0.5;
--opacity-60: 0.6;
--opacity-70: 0.7;
--opacity-75: 0.75;
--opacity-80: 0.8;
--opacity-90: 0.9;
--opacity-95: 0.95;
--opacity-100: 1;

/* Specific uses */
--opacity-disabled: 0.5;
--opacity-placeholder: 0.5;
--opacity-overlay: 0.5;
--opacity-hover: 0.8;
```

### Borders

#### Border Widths
```css
--border-width-0: 0;
--border-width-1: 1px;
--border-width-2: 2px;
--border-width-4: 4px;
--border-width-8: 8px;
```

#### Border Radius Scale
```css
--radius-none: 0;
--radius-sm: 4px;
--radius-md: 6px;
--radius-lg: 8px;
--radius-xl: 12px;
--radius-2xl: 16px;
--radius-3xl: 24px;
--radius-full: 9999px;  /* Pill shape */

/* Component-specific */
--radius-button: 9999px;    /* Pill buttons */
--radius-button-square: 8px;
--radius-card: 12px;
--radius-modal: 16px;
--radius-input: 8px;
--radius-badge: 9999px;
--radius-avatar: 9999px;
--radius-tooltip: 6px;
--radius-dropdown: 8px;
```

#### Border Styles
```css
--border-solid: solid;
--border-dashed: dashed;
--border-dotted: dotted;
```

### Iconography

#### Icon Style
- Primary style: **Outlined** (stroke-based icons)
- Secondary style: **Filled** for active/selected states
- Consistent 1.5px or 2px stroke weight

#### Icon Sizes
```css
--icon-size-xs: 12px;
--icon-size-sm: 16px;
--icon-size-md: 20px;
--icon-size-lg: 24px;
--icon-size-xl: 32px;
--icon-size-2xl: 40px;
--icon-size-3xl: 48px;
```

#### Icon Stroke Weights
```css
--icon-stroke-thin: 1px;
--icon-stroke-normal: 1.5px;
--icon-stroke-medium: 2px;
--icon-stroke-bold: 2.5px;
```

#### Icon Library
- Primary: **Lucide Icons** (based on Feather Icons)
- Alternative: Heroicons (outline variant)
- Custom brand icons for logo and specific features

### Motion & Animation

#### Easing Curves
```css
--ease-linear: linear;
--ease-in: cubic-bezier(0.4, 0, 1, 1);
--ease-out: cubic-bezier(0, 0, 0.2, 1);
--ease-in-out: cubic-bezier(0.4, 0, 0.2, 1);
--ease-bounce: cubic-bezier(0.68, -0.55, 0.265, 1.55);
--ease-spring: cubic-bezier(0.175, 0.885, 0.32, 1.275);
```

#### Duration Scale
```css
--duration-instant: 0ms;
--duration-fast: 100ms;
--duration-normal: 200ms;
--duration-moderate: 300ms;
--duration-slow: 400ms;
--duration-slower: 500ms;
--duration-slowest: 700ms;
```

#### Transition Properties
```css
--transition-colors: color, background-color, border-color, fill, stroke;
--transition-opacity: opacity;
--transition-transform: transform;
--transition-shadow: box-shadow;
--transition-all: all;
```

#### Animation Patterns
```css
/* Fade in */
@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

/* Fade in up */
@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* Scale in */
@keyframes scaleIn {
  from {
    opacity: 0;
    transform: scale(0.95);
  }
  to {
    opacity: 1;
    transform: scale(1);
  }
}

/* Slide in from right */
@keyframes slideInRight {
  from {
    opacity: 0;
    transform: translateX(20px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

/* Spin (for loaders) */
@keyframes spin {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}

/* Pulse */
@keyframes pulse {
  0%, 100% { opacity: 1; }
  50% { opacity: 0.5; }
}
```

---

## 3. Components

### Buttons

#### Primary Button (Lime/Yellow-Green)
```css
.button-primary {
  /* Dimensions */
  height: 44px;
  min-width: 120px;
  padding: 10px 24px;

  /* Visual */
  background-color: #D4F94E;
  color: #18181B;
  border: none;
  border-radius: 9999px;

  /* Typography */
  font-size: 14px;
  font-weight: 500;
  line-height: 1.4;

  /* Effects */
  box-shadow: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
  cursor: pointer;
  transition: all 200ms ease-in-out;
}

.button-primary:hover {
  background-color: #BEF026;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
}

.button-primary:active {
  background-color: #A8E600;
  transform: scale(0.98);
}

.button-primary:focus {
  outline: none;
  box-shadow: 0 0 0 3px rgba(212, 249, 78, 0.4);
}

.button-primary:disabled {
  background-color: #E4E4E7;
  color: #A1A1AA;
  cursor: not-allowed;
  box-shadow: none;
}
```

#### Secondary Button (Black)
```css
.button-secondary {
  height: 44px;
  min-width: 120px;
  padding: 10px 24px;
  background-color: #18181B;
  color: #FFFFFF;
  border: none;
  border-radius: 9999px;
  font-size: 14px;
  font-weight: 500;
  transition: all 200ms ease-in-out;
}

.button-secondary:hover {
  background-color: #27272A;
}

.button-secondary:active {
  background-color: #3F3F46;
}

.button-secondary:disabled {
  background-color: #D4D4D8;
  color: #A1A1AA;
}
```

#### Tertiary Button (Outline)
```css
.button-tertiary {
  height: 44px;
  min-width: 120px;
  padding: 10px 24px;
  background-color: #FFFFFF;
  color: #18181B;
  border: 1px solid #E4E4E7;
  border-radius: 9999px;
  font-size: 14px;
  font-weight: 500;
  transition: all 200ms ease-in-out;
}

.button-tertiary:hover {
  background-color: #F4F4F5;
  border-color: #D4D4D8;
}

.button-tertiary:active {
  background-color: #E4E4E7;
}
```

#### Ghost Button
```css
.button-ghost {
  height: 44px;
  padding: 10px 16px;
  background-color: transparent;
  color: #52525B;
  border: none;
  border-radius: 8px;
  font-size: 14px;
  font-weight: 500;
  transition: all 200ms ease-in-out;
}

.button-ghost:hover {
  background-color: #F4F4F5;
  color: #18181B;
}
```

#### Icon Button (Orange Circle)
```css
.button-icon-orange {
  width: 48px;
  height: 48px;
  padding: 12px;
  background-color: #F97316;
  color: #FFFFFF;
  border: none;
  border-radius: 9999px;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: all 200ms ease-in-out;
}

.button-icon-orange:hover {
  background-color: #EA580C;
  transform: scale(1.05);
}
```

#### Orange CTA Button
```css
.button-cta-orange {
  height: 48px;
  padding: 12px 32px;
  background-color: #F97316;
  color: #FFFFFF;
  border: none;
  border-radius: 9999px;
  font-size: 16px;
  font-weight: 500;
  transition: all 200ms ease-in-out;
}

.button-cta-orange:hover {
  background-color: #EA580C;
}
```

#### Button Sizes
```css
/* Small */
.button-sm {
  height: 32px;
  padding: 6px 14px;
  font-size: 13px;
}

/* Medium (default) */
.button-md {
  height: 40px;
  padding: 10px 20px;
  font-size: 14px;
}

/* Large */
.button-lg {
  height: 48px;
  padding: 12px 28px;
  font-size: 16px;
}

/* Extra Large */
.button-xl {
  height: 56px;
  padding: 14px 32px;
  font-size: 18px;
}
```

### Inputs

#### Text Input
```css
.input-text {
  /* Dimensions */
  width: 100%;
  height: 44px;
  padding: 10px 14px;

  /* Visual */
  background-color: #FFFFFF;
  border: 1px solid #E4E4E7;
  border-radius: 8px;

  /* Typography */
  font-size: 14px;
  font-weight: 400;
  color: #18181B;

  /* Transition */
  transition: border-color 200ms ease, box-shadow 200ms ease;
}

.input-text::placeholder {
  color: #A1A1AA;
}

.input-text:hover {
  border-color: #D4D4D8;
}

.input-text:focus {
  outline: none;
  border-color: #F97316;
  box-shadow: 0 0 0 3px rgba(249, 115, 22, 0.1);
}

.input-text:disabled {
  background-color: #F4F4F5;
  color: #A1A1AA;
  cursor: not-allowed;
}

.input-text.error {
  border-color: #EF4444;
}

.input-text.error:focus {
  box-shadow: 0 0 0 3px rgba(239, 68, 68, 0.1);
}
```

#### Textarea
```css
.textarea {
  width: 100%;
  min-height: 120px;
  padding: 12px 14px;
  background-color: #FFFFFF;
  border: 1px solid #E4E4E7;
  border-radius: 8px;
  font-size: 14px;
  font-family: inherit;
  color: #18181B;
  resize: vertical;
  transition: border-color 200ms ease, box-shadow 200ms ease;
}

.textarea:focus {
  outline: none;
  border-color: #F97316;
  box-shadow: 0 0 0 3px rgba(249, 115, 22, 0.1);
}
```

#### Select Dropdown
```css
.select {
  width: 100%;
  height: 44px;
  padding: 10px 40px 10px 14px;
  background-color: #FFFFFF;
  background-image: url("data:image/svg+xml,..."); /* Chevron down icon */
  background-repeat: no-repeat;
  background-position: right 14px center;
  background-size: 16px;
  border: 1px solid #E4E4E7;
  border-radius: 8px;
  font-size: 14px;
  color: #18181B;
  appearance: none;
  cursor: pointer;
  transition: border-color 200ms ease;
}

.select:focus {
  outline: none;
  border-color: #F97316;
  box-shadow: 0 0 0 3px rgba(249, 115, 22, 0.1);
}
```

#### Checkbox
```css
.checkbox {
  width: 18px;
  height: 18px;
  border: 1.5px solid #D4D4D8;
  border-radius: 4px;
  background-color: #FFFFFF;
  cursor: pointer;
  transition: all 150ms ease;
}

.checkbox:checked {
  background-color: #18181B;
  border-color: #18181B;
  background-image: url("data:image/svg+xml,..."); /* Checkmark */
  background-repeat: no-repeat;
  background-position: center;
}

.checkbox:focus {
  box-shadow: 0 0 0 3px rgba(24, 24, 27, 0.1);
}
```

#### Toggle Switch
```css
.toggle {
  position: relative;
  width: 44px;
  height: 24px;
  background-color: #E4E4E7;
  border-radius: 9999px;
  cursor: pointer;
  transition: background-color 200ms ease;
}

.toggle::after {
  content: '';
  position: absolute;
  top: 2px;
  left: 2px;
  width: 20px;
  height: 20px;
  background-color: #FFFFFF;
  border-radius: 9999px;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.1);
  transition: transform 200ms ease;
}

.toggle.checked {
  background-color: #18181B;
}

.toggle.checked::after {
  transform: translateX(20px);
}
```

### Cards

#### Default Card
```css
.card {
  background-color: #FFFFFF;
  border: 1px solid #E4E4E7;
  border-radius: 12px;
  padding: 24px;
  box-shadow: 0 1px 3px 0 rgba(0, 0, 0, 0.08);
  transition: box-shadow 200ms ease, transform 200ms ease;
}

.card:hover {
  box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.08);
}

.card-clickable:hover {
  transform: translateY(-2px);
  cursor: pointer;
}
```

#### Gradient Card (Soft Orange)
```css
.card-gradient-orange {
  background: linear-gradient(135deg, #FFEDD5 0%, #FED7AA 100%);
  border: none;
  border-radius: 16px;
  padding: 24px;
}
```

#### Gradient Card (Soft Yellow)
```css
.card-gradient-yellow {
  background: linear-gradient(135deg, #FEF9C3 0%, #FEF08A 100%);
  border: none;
  border-radius: 16px;
  padding: 24px;
}
```

#### Gradient Card (Soft Mint)
```css
.card-gradient-mint {
  background: linear-gradient(135deg, #D1FAE5 0%, #A7F3D0 100%);
  border: none;
  border-radius: 16px;
  padding: 24px;
}
```

#### Gradient Card (Soft Sky)
```css
.card-gradient-sky {
  background: linear-gradient(135deg, #E0F2FE 0%, #BAE6FD 100%);
  border: none;
  border-radius: 16px;
  padding: 24px;
}
```

### Modals/Dialogs

#### Modal Container
```css
.modal-overlay {
  position: fixed;
  inset: 0;
  background-color: rgba(0, 0, 0, 0.5);
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 1000;
  animation: fadeIn 200ms ease;
}

.modal {
  background-color: #FFFFFF;
  border-radius: 16px;
  max-width: 560px;
  width: 90%;
  max-height: 90vh;
  overflow: hidden;
  box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.25);
  animation: scaleIn 200ms ease;
}

.modal-header {
  padding: 24px 24px 0;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.modal-title {
  font-size: 20px;
  font-weight: 600;
  color: #18181B;
}

.modal-close {
  width: 32px;
  height: 32px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 8px;
  color: #71717A;
  cursor: pointer;
  transition: background-color 150ms ease;
}

.modal-close:hover {
  background-color: #F4F4F5;
}

.modal-body {
  padding: 24px;
}

.modal-footer {
  padding: 16px 24px;
  background-color: #FAFAFA;
  display: flex;
  gap: 12px;
  justify-content: flex-end;
}
```

### Dropdowns/Menus

#### Dropdown Menu
```css
.dropdown {
  position: relative;
  display: inline-block;
}

.dropdown-menu {
  position: absolute;
  top: 100%;
  left: 0;
  margin-top: 8px;
  min-width: 200px;
  background-color: #FFFFFF;
  border: 1px solid #E4E4E7;
  border-radius: 8px;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
  padding: 4px;
  z-index: 100;
  animation: fadeInUp 150ms ease;
}

.dropdown-item {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 10px 12px;
  border-radius: 6px;
  font-size: 14px;
  color: #18181B;
  cursor: pointer;
  transition: background-color 150ms ease;
}

.dropdown-item:hover {
  background-color: #F4F4F5;
}

.dropdown-divider {
  height: 1px;
  background-color: #E4E4E7;
  margin: 4px 0;
}
```

### Navigation

#### Header Navigation
```css
.header {
  position: sticky;
  top: 0;
  z-index: 100;
  background-color: rgba(255, 255, 255, 0.9);
  backdrop-filter: blur(8px);
  border-bottom: 1px solid #E4E4E7;
}

.header-inner {
  max-width: 1280px;
  margin: 0 auto;
  padding: 0 24px;
  height: 64px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.header-logo {
  display: flex;
  align-items: center;
  gap: 8px;
}

.header-logo-icon {
  width: 32px;
  height: 32px;
}

.header-logo-text {
  font-size: 20px;
  font-weight: 700;
  color: #18181B;
}

.header-nav {
  display: flex;
  align-items: center;
  gap: 32px;
}

.header-nav-item {
  font-size: 14px;
  font-weight: 500;
  color: #52525B;
  text-decoration: none;
  transition: color 150ms ease;
}

.header-nav-item:hover {
  color: #18181B;
}

.header-actions {
  display: flex;
  align-items: center;
  gap: 16px;
}
```

#### Sidebar Navigation
```css
.sidebar {
  width: 260px;
  height: 100vh;
  background-color: #FFFFFF;
  border-right: 1px solid #E4E4E7;
  padding: 16px 12px;
  overflow-y: auto;
}

.sidebar-section {
  margin-bottom: 24px;
}

.sidebar-section-title {
  font-size: 11px;
  font-weight: 600;
  color: #71717A;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  padding: 8px 12px;
  margin-bottom: 4px;
}

.sidebar-item {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 10px 12px;
  border-radius: 8px;
  font-size: 14px;
  font-weight: 500;
  color: #52525B;
  cursor: pointer;
  transition: all 150ms ease;
}

.sidebar-item:hover {
  background-color: #F4F4F5;
  color: #18181B;
}

.sidebar-item.active {
  background-color: #F4F4F5;
  color: #18181B;
}

.sidebar-item-icon {
  width: 20px;
  height: 20px;
  color: inherit;
}

.sidebar-badge {
  margin-left: auto;
  font-size: 11px;
  font-weight: 500;
  color: #71717A;
  background-color: #F4F4F5;
  padding: 2px 8px;
  border-radius: 9999px;
}
```

#### Tab Navigation
```css
.tabs {
  display: flex;
  border-bottom: 1px solid #E4E4E7;
}

.tab {
  padding: 12px 16px;
  font-size: 14px;
  font-weight: 500;
  color: #71717A;
  border-bottom: 2px solid transparent;
  cursor: pointer;
  transition: all 150ms ease;
}

.tab:hover {
  color: #18181B;
}

.tab.active {
  color: #18181B;
  border-bottom-color: #18181B;
}

/* Pill Tabs */
.tabs-pill {
  display: inline-flex;
  background-color: #F4F4F5;
  border-radius: 9999px;
  padding: 4px;
}

.tab-pill {
  padding: 8px 20px;
  font-size: 14px;
  font-weight: 500;
  color: #52525B;
  border-radius: 9999px;
  cursor: pointer;
  transition: all 150ms ease;
}

.tab-pill.active {
  background-color: #FFFFFF;
  color: #18181B;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.1);
}
```

#### Breadcrumbs
```css
.breadcrumbs {
  display: flex;
  align-items: center;
  gap: 8px;
  font-size: 14px;
}

.breadcrumb-item {
  color: #71717A;
  text-decoration: none;
  transition: color 150ms ease;
}

.breadcrumb-item:hover {
  color: #18181B;
}

.breadcrumb-item.active {
  color: #18181B;
  font-weight: 500;
}

.breadcrumb-separator {
  color: #D4D4D8;
}
```

### Tables

#### Data Table
```css
.table {
  width: 100%;
  border-collapse: collapse;
}

.table thead {
  background-color: #FAFAFA;
}

.table th {
  padding: 12px 16px;
  text-align: left;
  font-size: 12px;
  font-weight: 600;
  color: #71717A;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  border-bottom: 1px solid #E4E4E7;
}

.table td {
  padding: 16px;
  font-size: 14px;
  color: #18181B;
  border-bottom: 1px solid #E4E4E7;
}

.table tbody tr:hover {
  background-color: #FAFAFA;
}
```

### Badges/Tags/Chips

#### Badge
```css
.badge {
  display: inline-flex;
  align-items: center;
  padding: 4px 10px;
  font-size: 12px;
  font-weight: 500;
  border-radius: 9999px;
}

.badge-default {
  background-color: #F4F4F5;
  color: #52525B;
}

.badge-orange {
  background-color: #FFEDD5;
  color: #C2410C;
}

.badge-green {
  background-color: #DCFCE7;
  color: #16A34A;
}

.badge-blue {
  background-color: #DBEAFE;
  color: #2563EB;
}

.badge-red {
  background-color: #FEE2E2;
  color: #DC2626;
}

.badge-yellow {
  background-color: #FEF3C7;
  color: #D97706;
}
```

#### HTTP Method Badges
```css
.badge-get {
  background-color: #DCFCE7;
  color: #16A34A;
  font-family: monospace;
  font-size: 11px;
  font-weight: 600;
  text-transform: lowercase;
}

.badge-post {
  background-color: #DBEAFE;
  color: #2563EB;
  font-family: monospace;
  font-size: 11px;
  font-weight: 600;
  text-transform: lowercase;
}

.badge-put {
  background-color: #FFEDD5;
  color: #C2410C;
  font-family: monospace;
  font-size: 11px;
  font-weight: 600;
  text-transform: lowercase;
}

.badge-delete {
  background-color: #FEE2E2;
  color: #DC2626;
  font-family: monospace;
  font-size: 11px;
  font-weight: 600;
  text-transform: lowercase;
}
```

#### Chip (Interactive Tag)
```css
.chip {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 8px 16px;
  background-color: #FFFFFF;
  border: 1px solid #E4E4E7;
  border-radius: 9999px;
  font-size: 14px;
  font-weight: 500;
  color: #18181B;
  cursor: pointer;
  transition: all 150ms ease;
}

.chip:hover {
  background-color: #F4F4F5;
  border-color: #D4D4D8;
}

.chip.selected {
  background-color: #18181B;
  border-color: #18181B;
  color: #FFFFFF;
}
```

### Avatars

#### Avatar
```css
.avatar {
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 9999px;
  overflow: hidden;
  background-color: #F4F4F5;
  color: #52525B;
  font-weight: 600;
}

.avatar img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.avatar-xs { width: 24px; height: 24px; font-size: 10px; }
.avatar-sm { width: 32px; height: 32px; font-size: 12px; }
.avatar-md { width: 40px; height: 40px; font-size: 14px; }
.avatar-lg { width: 48px; height: 48px; font-size: 16px; }
.avatar-xl { width: 64px; height: 64px; font-size: 20px; }
.avatar-2xl { width: 80px; height: 80px; font-size: 24px; }
```

### Tooltips

#### Tooltip
```css
.tooltip {
  position: relative;
}

.tooltip-content {
  position: absolute;
  bottom: 100%;
  left: 50%;
  transform: translateX(-50%);
  margin-bottom: 8px;
  padding: 8px 12px;
  background-color: #18181B;
  color: #FFFFFF;
  font-size: 13px;
  border-radius: 6px;
  white-space: nowrap;
  z-index: 1000;
  animation: fadeIn 150ms ease;
}

.tooltip-content::after {
  content: '';
  position: absolute;
  top: 100%;
  left: 50%;
  transform: translateX(-50%);
  border: 6px solid transparent;
  border-top-color: #18181B;
}
```

### Alerts/Banners

#### Alert
```css
.alert {
  display: flex;
  gap: 12px;
  padding: 16px;
  border-radius: 8px;
  font-size: 14px;
}

.alert-icon {
  flex-shrink: 0;
  width: 20px;
  height: 20px;
}

.alert-success {
  background-color: #DCFCE7;
  color: #16A34A;
}

.alert-warning {
  background-color: #FEF3C7;
  color: #D97706;
}

.alert-error {
  background-color: #FEE2E2;
  color: #DC2626;
}

.alert-info {
  background-color: #DBEAFE;
  color: #2563EB;
}

/* Tip Box - Green */
.alert-tip {
  background-color: #DCFCE7;
  border-left: 4px solid #22C55E;
}
```

### Progress Indicators

#### Progress Bar
```css
.progress-bar {
  width: 100%;
  height: 8px;
  background-color: #E4E4E7;
  border-radius: 9999px;
  overflow: hidden;
}

.progress-bar-fill {
  height: 100%;
  background-color: #F97316;
  border-radius: 9999px;
  transition: width 300ms ease;
}
```

#### Spinner
```css
.spinner {
  width: 24px;
  height: 24px;
  border: 2px solid #E4E4E7;
  border-top-color: #F97316;
  border-radius: 9999px;
  animation: spin 600ms linear infinite;
}

.spinner-sm { width: 16px; height: 16px; border-width: 2px; }
.spinner-md { width: 24px; height: 24px; border-width: 2px; }
.spinner-lg { width: 32px; height: 32px; border-width: 3px; }
.spinner-xl { width: 48px; height: 48px; border-width: 3px; }
```

#### Loading Animation (Orange Circles)
```css
.loading-dots {
  display: flex;
  gap: 8px;
}

.loading-dot {
  width: 12px;
  height: 12px;
  background-color: #F97316;
  border-radius: 9999px;
  animation: pulse 1.4s ease-in-out infinite;
}

.loading-dot:nth-child(2) { animation-delay: 0.2s; }
.loading-dot:nth-child(3) { animation-delay: 0.4s; }
```

#### Skeleton Screen
```css
.skeleton {
  background: linear-gradient(90deg, #F4F4F5 25%, #E4E4E7 50%, #F4F4F5 75%);
  background-size: 200% 100%;
  animation: shimmer 1.5s infinite;
  border-radius: 4px;
}

@keyframes shimmer {
  0% { background-position: 200% 0; }
  100% { background-position: -200% 0; }
}

.skeleton-text { height: 16px; }
.skeleton-title { height: 24px; width: 60%; }
.skeleton-avatar { width: 40px; height: 40px; border-radius: 9999px; }
.skeleton-button { height: 40px; width: 120px; border-radius: 9999px; }
```

### Pricing Cards

#### Pricing Card
```css
.pricing-card {
  background-color: #FFFFFF;
  border: 1px solid #E4E4E7;
  border-radius: 12px;
  padding: 32px 24px;
  display: flex;
  flex-direction: column;
}

.pricing-card-name {
  font-size: 18px;
  font-weight: 600;
  color: #18181B;
  margin-bottom: 8px;
}

.pricing-card-description {
  font-size: 14px;
  color: #71717A;
  margin-bottom: 24px;
}

.pricing-card-price {
  display: flex;
  align-items: baseline;
  gap: 4px;
  margin-bottom: 4px;
}

.pricing-card-amount {
  font-size: 48px;
  font-weight: 700;
  color: #18181B;
}

.pricing-card-period {
  font-size: 14px;
  color: #71717A;
}

.pricing-card-billing {
  font-size: 13px;
  color: #71717A;
  margin-bottom: 24px;
}

.pricing-card-features {
  list-style: none;
  padding: 0;
  margin: 0 0 24px 0;
}

.pricing-card-feature {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 8px 0;
  font-size: 14px;
  color: #52525B;
}

.pricing-card-feature-icon {
  width: 16px;
  height: 16px;
  color: #22C55E;
}
```

---

## 4. Layout System

### Grid System
```css
/* 12-column grid */
.container {
  width: 100%;
  max-width: 1280px;
  margin: 0 auto;
  padding: 0 24px;
}

.grid {
  display: grid;
  gap: var(--grid-gap-md, 24px);
}

.grid-cols-1 { grid-template-columns: repeat(1, 1fr); }
.grid-cols-2 { grid-template-columns: repeat(2, 1fr); }
.grid-cols-3 { grid-template-columns: repeat(3, 1fr); }
.grid-cols-4 { grid-template-columns: repeat(4, 1fr); }
.grid-cols-5 { grid-template-columns: repeat(5, 1fr); }
.grid-cols-6 { grid-template-columns: repeat(6, 1fr); }
.grid-cols-12 { grid-template-columns: repeat(12, 1fr); }
```

### Container Max-Widths
```css
--container-sm: 640px;
--container-md: 768px;
--container-lg: 1024px;
--container-xl: 1280px;
--container-2xl: 1440px;
--container-prose: 65ch;  /* For article content */
```

### Breakpoints
```css
--breakpoint-sm: 640px;
--breakpoint-md: 768px;
--breakpoint-lg: 1024px;
--breakpoint-xl: 1280px;
--breakpoint-2xl: 1536px;
```

### Responsive Behavior Rules
```css
/* Mobile first approach */
@media (min-width: 640px) { /* sm */ }
@media (min-width: 768px) { /* md */ }
@media (min-width: 1024px) { /* lg */ }
@media (min-width: 1280px) { /* xl */ }
@media (min-width: 1536px) { /* 2xl */ }
```

### Page Structure Templates

#### Marketing Page Layout
```css
.page-marketing {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

.page-marketing-header {
  position: sticky;
  top: 0;
  z-index: 100;
}

.page-marketing-content {
  flex: 1;
}

.page-marketing-footer {
  margin-top: auto;
}
```

#### Dashboard Layout
```css
.page-dashboard {
  display: flex;
  min-height: 100vh;
}

.page-dashboard-sidebar {
  width: 260px;
  flex-shrink: 0;
  position: sticky;
  top: 0;
  height: 100vh;
}

.page-dashboard-main {
  flex: 1;
  display: flex;
  flex-direction: column;
}

.page-dashboard-header {
  height: 64px;
  border-bottom: 1px solid #E4E4E7;
  position: sticky;
  top: 0;
  background-color: #FFFFFF;
  z-index: 50;
}

.page-dashboard-content {
  flex: 1;
  padding: 32px;
  background-color: #FAFAFA;
}
```

### Content Width Constraints
```css
--content-width-narrow: 640px;
--content-width-default: 768px;
--content-width-wide: 1024px;
--content-width-full: 100%;
```

### Vertical Rhythm Patterns
```css
/* Section spacing */
.section { padding: 64px 0; }
.section-lg { padding: 96px 0; }
.section-xl { padding: 128px 0; }

/* Element spacing within sections */
.stack-xs > * + * { margin-top: 8px; }
.stack-sm > * + * { margin-top: 12px; }
.stack-md > * + * { margin-top: 16px; }
.stack-lg > * + * { margin-top: 24px; }
.stack-xl > * + * { margin-top: 32px; }
```

---

## 5. Patterns

### Navigation Patterns

#### Header Structure and Behavior
- Fixed/sticky header with backdrop blur
- Height: 64px
- Logo on left, navigation center, CTA on right
- Transparent on hero sections, white with border on scroll
- Mobile: Hamburger menu triggers slide-out drawer

#### Mobile Navigation
```css
.mobile-menu {
  position: fixed;
  inset: 0;
  background-color: #FFFFFF;
  z-index: 200;
  transform: translateX(-100%);
  transition: transform 300ms ease;
}

.mobile-menu.open {
  transform: translateX(0);
}

.mobile-menu-item {
  padding: 16px 24px;
  font-size: 18px;
  font-weight: 500;
  border-bottom: 1px solid #E4E4E7;
}
```

#### Sidebar Patterns
- Collapsible sections with chevron indicators
- Active state with background highlight
- Beta/New badges for new features
- Nested items with left indentation (16px)

### Form Patterns

#### Form Layout
- Labels positioned above inputs
- Label font-size: 14px, font-weight: 500
- Gap between label and input: 6px
- Gap between form fields: 20px
- Inline helper text below input: 12px, color: muted

#### Validation Display
```css
.form-field {
  display: flex;
  flex-direction: column;
  gap: 6px;
}

.form-label {
  font-size: 14px;
  font-weight: 500;
  color: #18181B;
}

.form-error {
  font-size: 12px;
  color: #DC2626;
  display: flex;
  align-items: center;
  gap: 6px;
}

.form-helper {
  font-size: 12px;
  color: #71717A;
}
```

#### Required Field Indication
- Red asterisk (*) after label
- Color: #EF4444

### Content Patterns

#### Card Grid Arrangements
```css
/* 3-column card grid */
.card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 24px;
}
```

#### Empty States
```css
.empty-state {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 64px 24px;
  text-align: center;
}

.empty-state-icon {
  width: 64px;
  height: 64px;
  color: #D4D4D8;
  margin-bottom: 16px;
}

.empty-state-title {
  font-size: 18px;
  font-weight: 600;
  color: #18181B;
  margin-bottom: 8px;
}

.empty-state-description {
  font-size: 14px;
  color: #71717A;
  max-width: 360px;
  margin-bottom: 24px;
}
```

### Feedback Patterns

#### Toast Notifications
```css
.toast-container {
  position: fixed;
  bottom: 24px;
  right: 24px;
  z-index: 1000;
  display: flex;
  flex-direction: column;
  gap: 12px;
}

.toast {
  min-width: 320px;
  padding: 16px;
  background-color: #FFFFFF;
  border-radius: 8px;
  box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
  display: flex;
  align-items: flex-start;
  gap: 12px;
  animation: slideInRight 300ms ease;
}
```

---

## 6. Page Templates

### Landing Page / Marketing Page
```
┌─────────────────────────────────────────────────┐
│ Header (Sticky)                                  │
│ [Logo]    [Nav Items]           [Globe] [CTA]   │
├─────────────────────────────────────────────────┤
│                                                  │
│              Hero Section                        │
│         (Gradient Background)                    │
│                                                  │
│         Large Display Heading                    │
│         Subheading paragraph                     │
│                                                  │
│    [Prompt Input]          [Orange Submit]       │
│                                                  │
│         [Chip] [Chip] [Chip]                    │
│                                                  │
├─────────────────────────────────────────────────┤
│                                                  │
│           Features Section                       │
│                                                  │
│    ┌─────────┐  ┌─────────┐  ┌─────────┐       │
│    │  Card   │  │  Card   │  │  Card   │       │
│    │(Gradient)│  │(Gradient)│  │(Gradient)│       │
│    └─────────┘  └─────────┘  └─────────┘       │
│                                                  │
├─────────────────────────────────────────────────┤
│                                                  │
│           Testimonials / Social Proof            │
│                                                  │
├─────────────────────────────────────────────────┤
│                                                  │
│           CTA Section                            │
│                                                  │
├─────────────────────────────────────────────────┤
│                 Footer                           │
│    [Logo]  [Links]  [Links]  [Links]  [Social]  │
└─────────────────────────────────────────────────┘
```

### Dashboard Page
```
┌──────────────────────────────────────────────────────────┐
│ ┌─────────────┐                                          │
│ │             │  [Dashboard]  [Preview]     [Actions]    │
│ │  Sidebar    │ ─────────────────────────────────────────│
│ │             │                                          │
│ │  Overview   │   Page Title                             │
│ │  Users      │   Description text                       │
│ │  Data ▼     │                                          │
│ │   - Table1  │   ┌────────────────────────────────────┐│
│ │   - Table2  │   │                                    ││
│ │  Analytics  │   │         Main Content Area          ││
│ │  Domains    │   │                                    ││
│ │  Security   │   │    Cards / Tables / Forms          ││
│ │  Code       │   │                                    ││
│ │  Agents     │   │                                    ││
│ │  Logs       │   │                                    ││
│ │  API        │   │                                    ││
│ │  Settings ▼ │   │                                    ││
│ │             │   └────────────────────────────────────┘│
│ │             │                                          │
│ └─────────────┘                                          │
└──────────────────────────────────────────────────────────┘
```

### Login/Auth Page
```
┌─────────────────────────────────────────────────┐
│ [Logo]                                           │
├───────────────────────┬─────────────────────────┤
│                       │                          │
│    Welcome to         │     Gradient             │
│    [Product]          │     Background           │
│                       │                          │
│  [Google Sign In]     │     Prompt Input         │
│                       │     "Turn your ideas     │
│  ─────── OR ──────    │      into apps"          │
│                       │                          │
│  Email                │                          │
│  [____________]       │                          │
│                       │                          │
│  [Continue]           │                          │
│                       │                          │
│  Don't have account?  │                          │
│  Sign up              │                          │
│                       │                          │
│  Terms | Privacy      │                          │
│                       │                          │
└───────────────────────┴─────────────────────────┘
```

---

## 7. Imagery & Media

### Image Aspect Ratios
```css
--aspect-square: 1 / 1;
--aspect-video: 16 / 9;
--aspect-wide: 21 / 9;
--aspect-portrait: 3 / 4;
--aspect-card: 4 / 3;
--aspect-hero: 16 / 7;
```

### Image Border Treatments
```css
.image-rounded { border-radius: 8px; }
.image-rounded-lg { border-radius: 16px; }
.image-circle { border-radius: 9999px; }
.image-bordered { border: 1px solid #E4E4E7; }
```

### Placeholder/Fallback Styles
```css
.image-placeholder {
  background-color: #F4F4F5;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #A1A1AA;
}
```

### Avatar Fallbacks
- Display initials on colored background
- Background color derived from name hash
- Default: Gray background with icon

---

## 8. Accessibility

### Color Contrast Ratios
- Primary text (#18181B) on white: 16.1:1 ✓
- Secondary text (#52525B) on white: 7.5:1 ✓
- Muted text (#71717A) on white: 4.7:1 ✓
- Primary button text on lime (#D4F94E): 4.5:1 ✓ (just meeting AA)
- White text on orange (#F97316): 3.1:1 (large text only)
- White text on black (#18181B): 16.1:1 ✓

### Focus Indicator Styles
```css
/* Default focus ring */
:focus-visible {
  outline: 2px solid #F97316;
  outline-offset: 2px;
}

/* Alternative focus ring for dark backgrounds */
.focus-white:focus-visible {
  outline-color: #FFFFFF;
}

/* Box-shadow based focus for inputs */
.input:focus {
  border-color: #F97316;
  box-shadow: 0 0 0 3px rgba(249, 115, 22, 0.2);
}
```

### Touch Target Sizes
```css
/* Minimum touch target: 44x44px */
--touch-target-min: 44px;

/* Interactive elements */
.button { min-height: 44px; min-width: 44px; }
.checkbox-wrapper { min-height: 44px; padding: 10px 0; }
.link-touchable { padding: 10px; margin: -10px; }
```

### Screen Reader Considerations
```css
/* Visually hidden but accessible */
.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  white-space: nowrap;
  border: 0;
}

/* Skip link */
.skip-link {
  position: absolute;
  top: -40px;
  left: 0;
  background: #18181B;
  color: #FFFFFF;
  padding: 8px 16px;
  z-index: 1000;
}

.skip-link:focus {
  top: 0;
}
```

---

## 9. Additional Components

### Color Picker

#### Color Picker Panel
```css
.color-picker {
  width: 280px;
  background-color: #FFFFFF;
  border: 1px solid #E4E4E7;
  border-radius: 12px;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
  overflow: hidden;
}

.color-picker-tabs {
  display: flex;
  border-bottom: 1px solid #E4E4E7;
}

.color-picker-tab {
  flex: 1;
  padding: 12px 16px;
  font-size: 14px;
  font-weight: 500;
  color: #71717A;
  background: none;
  border: none;
  cursor: pointer;
  transition: all 150ms ease;
}

.color-picker-tab.active {
  color: #18181B;
  border-bottom: 2px solid #18181B;
}

.color-picker-palette {
  display: grid;
  grid-template-columns: repeat(8, 1fr);
  gap: 4px;
  padding: 16px;
}

.color-picker-swatch {
  width: 28px;
  height: 28px;
  border-radius: 6px;
  cursor: pointer;
  border: 2px solid transparent;
  transition: transform 100ms ease;
}

.color-picker-swatch:hover {
  transform: scale(1.1);
}

.color-picker-swatch.selected {
  border-color: #18181B;
}

.color-picker-custom {
  padding: 16px;
}

.color-picker-gradient {
  width: 100%;
  height: 160px;
  border-radius: 8px;
  margin-bottom: 12px;
  cursor: crosshair;
}

.color-picker-hue {
  width: 100%;
  height: 12px;
  border-radius: 6px;
  background: linear-gradient(to right, #ff0000, #ffff00, #00ff00, #00ffff, #0000ff, #ff00ff, #ff0000);
  cursor: pointer;
}

.color-picker-input {
  display: flex;
  align-items: center;
  gap: 8px;
  margin-top: 12px;
}

.color-picker-hex {
  flex: 1;
  height: 40px;
  padding: 8px 12px;
  font-family: monospace;
  font-size: 14px;
  border: 1px solid #E4E4E7;
  border-radius: 8px;
}
```

### OTP/Verification Input

#### OTP Input Group
```css
.otp-input-group {
  display: flex;
  gap: 12px;
  justify-content: center;
}

.otp-input {
  width: 48px;
  height: 56px;
  text-align: center;
  font-size: 24px;
  font-weight: 600;
  border: 1px solid #E4E4E7;
  border-radius: 8px;
  background-color: #FFFFFF;
  transition: border-color 200ms ease, box-shadow 200ms ease;
}

.otp-input:focus {
  outline: none;
  border-color: #F97316;
  box-shadow: 0 0 0 3px rgba(249, 115, 22, 0.1);
}

.otp-input.filled {
  border-color: #18181B;
  background-color: #F4F4F5;
}

.otp-input.error {
  border-color: #EF4444;
  background-color: #FEE2E2;
}
```

### Referral Modal

#### Referral Share Component
```css
.referral-modal {
  max-width: 480px;
  text-align: center;
}

.referral-icon {
  width: 64px;
  height: 64px;
  margin: 0 auto 24px;
  background: linear-gradient(135deg, #FFEDD5 0%, #FED7AA 100%);
  border-radius: 16px;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #F97316;
}

.referral-title {
  font-size: 24px;
  font-weight: 700;
  color: #18181B;
  margin-bottom: 8px;
}

.referral-description {
  font-size: 14px;
  color: #71717A;
  margin-bottom: 24px;
}

.referral-link-box {
  display: flex;
  align-items: center;
  gap: 8px;
  padding: 12px;
  background-color: #F4F4F5;
  border-radius: 8px;
  margin-bottom: 16px;
}

.referral-link-text {
  flex: 1;
  font-size: 14px;
  font-family: monospace;
  color: #52525B;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}

.referral-copy-btn {
  padding: 8px 16px;
  background-color: #18181B;
  color: #FFFFFF;
  border-radius: 6px;
  font-size: 14px;
  font-weight: 500;
}
```

### Security Scan Results

#### Security Scan Card
```css
.security-scan-card {
  background-color: #FFFFFF;
  border: 1px solid #E4E4E7;
  border-radius: 12px;
  overflow: hidden;
}

.security-scan-header {
  padding: 20px 24px;
  border-bottom: 1px solid #E4E4E7;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.security-scan-status {
  display: flex;
  align-items: center;
  gap: 12px;
}

.security-scan-icon {
  width: 40px;
  height: 40px;
  border-radius: 10px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.security-scan-icon.success {
  background-color: #DCFCE7;
  color: #16A34A;
}

.security-scan-icon.warning {
  background-color: #FEF3C7;
  color: #D97706;
}

.security-scan-icon.error {
  background-color: #FEE2E2;
  color: #DC2626;
}

.security-scan-title {
  font-size: 16px;
  font-weight: 600;
  color: #18181B;
}

.security-scan-subtitle {
  font-size: 13px;
  color: #71717A;
}

.security-scan-body {
  padding: 24px;
}

.security-scan-item {
  display: flex;
  align-items: flex-start;
  gap: 12px;
  padding: 12px 0;
  border-bottom: 1px solid #F4F4F5;
}

.security-scan-item:last-child {
  border-bottom: none;
}

.security-scan-item-icon {
  width: 20px;
  height: 20px;
  flex-shrink: 0;
}

.security-scan-item-icon.pass {
  color: #22C55E;
}

.security-scan-item-icon.fail {
  color: #EF4444;
}

.security-scan-item-icon.warn {
  color: #F59E0B;
}
```

### AI Model Selector

#### Model Dropdown
```css
.model-selector {
  position: relative;
  width: 200px;
}

.model-selector-trigger {
  width: 100%;
  height: 40px;
  padding: 8px 12px;
  display: flex;
  align-items: center;
  gap: 8px;
  background-color: #FFFFFF;
  border: 1px solid #E4E4E7;
  border-radius: 8px;
  cursor: pointer;
  transition: border-color 150ms ease;
}

.model-selector-trigger:hover {
  border-color: #D4D4D8;
}

.model-selector-icon {
  width: 20px;
  height: 20px;
  color: #71717A;
}

.model-selector-label {
  flex: 1;
  font-size: 14px;
  font-weight: 500;
  color: #18181B;
  text-align: left;
}

.model-selector-chevron {
  width: 16px;
  height: 16px;
  color: #A1A1AA;
}

.model-selector-dropdown {
  position: absolute;
  top: 100%;
  left: 0;
  right: 0;
  margin-top: 4px;
  background-color: #FFFFFF;
  border: 1px solid #E4E4E7;
  border-radius: 8px;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
  z-index: 100;
}

.model-selector-option {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 12px 16px;
  cursor: pointer;
  transition: background-color 150ms ease;
}

.model-selector-option:hover {
  background-color: #F4F4F5;
}

.model-selector-option.selected {
  background-color: #FFF7ED;
}

.model-selector-option-name {
  font-size: 14px;
  font-weight: 500;
  color: #18181B;
}

.model-selector-option-desc {
  font-size: 12px;
  color: #71717A;
}
```

### Password Strength Indicator

#### Password Strength
```css
.password-strength {
  margin-top: 8px;
}

.password-strength-bar {
  display: flex;
  gap: 4px;
  margin-bottom: 6px;
}

.password-strength-segment {
  flex: 1;
  height: 4px;
  background-color: #E4E4E7;
  border-radius: 2px;
  transition: background-color 200ms ease;
}

.password-strength.weak .password-strength-segment:nth-child(1) {
  background-color: #EF4444;
}

.password-strength.fair .password-strength-segment:nth-child(1),
.password-strength.fair .password-strength-segment:nth-child(2) {
  background-color: #F59E0B;
}

.password-strength.good .password-strength-segment:nth-child(1),
.password-strength.good .password-strength-segment:nth-child(2),
.password-strength.good .password-strength-segment:nth-child(3) {
  background-color: #22C55E;
}

.password-strength.strong .password-strength-segment {
  background-color: #22C55E;
}

.password-strength-label {
  font-size: 12px;
  font-weight: 500;
}

.password-strength.weak .password-strength-label { color: #EF4444; }
.password-strength.fair .password-strength-label { color: #F59E0B; }
.password-strength.good .password-strength-label { color: #22C55E; }
.password-strength.strong .password-strength-label { color: #22C55E; }
```

### Publish Modal

#### Publish/Deploy Modal
```css
.publish-modal {
  max-width: 520px;
}

.publish-modal-header {
  display: flex;
  align-items: center;
  gap: 16px;
  margin-bottom: 24px;
}

.publish-modal-icon {
  width: 48px;
  height: 48px;
  background-color: #DCFCE7;
  border-radius: 12px;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #16A34A;
}

.publish-modal-title {
  font-size: 20px;
  font-weight: 600;
  color: #18181B;
}

.publish-modal-subtitle {
  font-size: 14px;
  color: #71717A;
}

.publish-domain-input {
  display: flex;
  align-items: center;
  background-color: #F4F4F5;
  border-radius: 8px;
  overflow: hidden;
  margin-bottom: 24px;
}

.publish-domain-prefix {
  padding: 12px 16px;
  font-size: 14px;
  color: #71717A;
  background-color: #E4E4E7;
  border-right: 1px solid #D4D4D8;
}

.publish-domain-field {
  flex: 1;
  padding: 12px 16px;
  font-size: 14px;
  border: none;
  background: transparent;
  outline: none;
}

.publish-domain-suffix {
  padding: 12px 16px;
  font-size: 14px;
  color: #71717A;
}

.publish-loading {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 48px 24px;
  text-align: center;
}

.publish-loading-spinner {
  width: 48px;
  height: 48px;
  border: 3px solid #E4E4E7;
  border-top-color: #F97316;
  border-radius: 50%;
  animation: spin 800ms linear infinite;
  margin-bottom: 16px;
}

.publish-loading-text {
  font-size: 14px;
  color: #71717A;
}
```

### Contact Form Modal

#### Contact Modal
```css
.contact-modal {
  max-width: 560px;
}

.contact-modal-header {
  text-align: center;
  margin-bottom: 32px;
}

.contact-modal-title {
  font-size: 28px;
  font-weight: 700;
  color: #18181B;
  margin-bottom: 8px;
}

.contact-modal-subtitle {
  font-size: 16px;
  color: #71717A;
}

.contact-form {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.contact-form-row {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 16px;
}

.contact-form-field textarea {
  min-height: 120px;
  resize: vertical;
}
```

### Feature Request / Roadmap Page

#### Feature Request Card (Canny-style)
```css
.feature-request-card {
  display: flex;
  gap: 16px;
  padding: 20px;
  background-color: #FFFFFF;
  border: 1px solid #E4E4E7;
  border-radius: 12px;
  transition: box-shadow 200ms ease;
}

.feature-request-card:hover {
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.08);
}

.feature-request-votes {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 4px;
  min-width: 48px;
}

.feature-vote-btn {
  width: 40px;
  height: 40px;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #F4F4F5;
  border: 1px solid #E4E4E7;
  border-radius: 8px;
  color: #71717A;
  cursor: pointer;
  transition: all 150ms ease;
}

.feature-vote-btn:hover {
  background-color: #E4E4E7;
  color: #18181B;
}

.feature-vote-btn.voted {
  background-color: #F97316;
  border-color: #F97316;
  color: #FFFFFF;
}

.feature-vote-count {
  font-size: 14px;
  font-weight: 600;
  color: #18181B;
}

.feature-request-content {
  flex: 1;
}

.feature-request-title {
  font-size: 16px;
  font-weight: 600;
  color: #18181B;
  margin-bottom: 4px;
  cursor: pointer;
}

.feature-request-title:hover {
  color: #F97316;
}

.feature-request-description {
  font-size: 14px;
  color: #71717A;
  line-height: 1.5;
  margin-bottom: 12px;
}

.feature-request-meta {
  display: flex;
  align-items: center;
  gap: 16px;
  font-size: 13px;
  color: #A1A1AA;
}

.feature-request-comments {
  display: flex;
  align-items: center;
  gap: 4px;
}

.feature-request-status {
  padding: 4px 10px;
  font-size: 11px;
  font-weight: 600;
  text-transform: uppercase;
  border-radius: 9999px;
}

.feature-request-status.planned {
  background-color: #DBEAFE;
  color: #2563EB;
}

.feature-request-status.in-progress {
  background-color: #FEF3C7;
  color: #D97706;
}

.feature-request-status.completed {
  background-color: #DCFCE7;
  color: #16A34A;
}

.feature-request-status.under-review {
  background-color: #F4F4F5;
  color: #52525B;
}
```

### Visual Editor Controls

#### Spacing Input Group
```css
.spacing-input-group {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 8px;
  padding: 12px;
  background-color: #F4F4F5;
  border-radius: 8px;
}

.spacing-input-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 4px;
}

.spacing-input-label {
  font-size: 10px;
  font-weight: 500;
  color: #71717A;
  text-transform: uppercase;
}

.spacing-input-field {
  width: 48px;
  height: 32px;
  text-align: center;
  font-size: 13px;
  font-weight: 500;
  border: 1px solid #E4E4E7;
  border-radius: 6px;
  background-color: #FFFFFF;
}

.spacing-input-field:focus {
  outline: none;
  border-color: #F97316;
}
```

### Code Editor

#### Code Editor Panel
```css
.code-editor {
  background-color: #1E1E1E;
  border-radius: 12px;
  overflow: hidden;
  font-family: 'SF Mono', 'Monaco', 'Inconsolata', 'Fira Code', monospace;
}

.code-editor-tabs {
  display: flex;
  background-color: #252526;
  border-bottom: 1px solid #3C3C3C;
}

.code-editor-tab {
  padding: 10px 16px;
  font-size: 13px;
  color: #8C8C8C;
  cursor: pointer;
  border-bottom: 2px solid transparent;
  transition: all 150ms ease;
}

.code-editor-tab:hover {
  color: #CCCCCC;
}

.code-editor-tab.active {
  color: #FFFFFF;
  background-color: #1E1E1E;
  border-bottom-color: #F97316;
}

.code-editor-content {
  padding: 16px;
  overflow-x: auto;
}

.code-editor-line {
  display: flex;
  line-height: 1.6;
}

.code-editor-line-number {
  width: 40px;
  text-align: right;
  padding-right: 16px;
  color: #5A5A5A;
  user-select: none;
}

.code-editor-line-content {
  flex: 1;
  color: #D4D4D4;
}

/* Syntax highlighting */
.code-keyword { color: #569CD6; }
.code-string { color: #CE9178; }
.code-number { color: #B5CEA8; }
.code-comment { color: #6A9955; }
.code-function { color: #DCDCAA; }
.code-variable { color: #9CDCFE; }
.code-type { color: #4EC9B0; }
.code-operator { color: #D4D4D4; }
```

### 404 Error Page

#### Error Page Layout
```css
.error-page {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 48px 24px;
  text-align: center;
  background: linear-gradient(135deg, #FAFAFA 0%, #F4F4F5 100%);
}

.error-page-code {
  font-size: 120px;
  font-weight: 800;
  color: #E4E4E7;
  line-height: 1;
  margin-bottom: 16px;
}

.error-page-title {
  font-size: 28px;
  font-weight: 700;
  color: #18181B;
  margin-bottom: 8px;
}

.error-page-description {
  font-size: 16px;
  color: #71717A;
  max-width: 400px;
  margin-bottom: 32px;
}

.error-page-actions {
  display: flex;
  gap: 12px;
}
```

### Authentication Settings

#### Auth Method Toggle Card
```css
.auth-method-card {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 20px;
  background-color: #FFFFFF;
  border: 1px solid #E4E4E7;
  border-radius: 12px;
  margin-bottom: 12px;
}

.auth-method-info {
  display: flex;
  align-items: center;
  gap: 16px;
}

.auth-method-icon {
  width: 40px;
  height: 40px;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #F4F4F5;
  border-radius: 10px;
}

.auth-method-name {
  font-size: 15px;
  font-weight: 600;
  color: #18181B;
  margin-bottom: 2px;
}

.auth-method-description {
  font-size: 13px;
  color: #71717A;
}

.auth-method-toggle {
  /* Uses standard toggle switch styles */
}
```

### Instruction Modal (Neo-Brutalism Style)

#### Instruction Card
```css
.instruction-card {
  background-color: #FEF9C3;
  border: 3px solid #18181B;
  border-radius: 16px;
  padding: 24px;
  box-shadow: 6px 6px 0 #18181B;
  max-width: 480px;
}

.instruction-card-header {
  display: flex;
  align-items: center;
  gap: 12px;
  margin-bottom: 16px;
}

.instruction-card-icon {
  width: 32px;
  height: 32px;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #18181B;
  color: #FEF9C3;
  border-radius: 8px;
}

.instruction-card-title {
  font-size: 18px;
  font-weight: 700;
  color: #18181B;
}

.instruction-card-content {
  font-size: 14px;
  line-height: 1.6;
  color: #52525B;
}

.instruction-card-steps {
  list-style: none;
  padding: 0;
  margin: 0;
}

.instruction-card-step {
  display: flex;
  gap: 12px;
  padding: 8px 0;
}

.instruction-card-step-number {
  width: 24px;
  height: 24px;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #18181B;
  color: #FEF9C3;
  border-radius: 6px;
  font-size: 12px;
  font-weight: 700;
  flex-shrink: 0;
}
```

### AI Chat Panel

#### Chat Message History
```css
.chat-panel {
  display: flex;
  flex-direction: column;
  height: 100%;
  background-color: #FFFFFF;
  border-left: 1px solid #E4E4E7;
}

.chat-messages {
  flex: 1;
  overflow-y: auto;
  padding: 16px;
}

.chat-message {
  margin-bottom: 16px;
}

.chat-message-user {
  display: flex;
  justify-content: flex-end;
}

.chat-message-user .chat-message-bubble {
  background-color: #18181B;
  color: #FFFFFF;
  border-radius: 16px 16px 4px 16px;
  padding: 12px 16px;
  max-width: 80%;
}

.chat-message-ai {
  display: flex;
  gap: 12px;
}

.chat-message-ai-avatar {
  width: 32px;
  height: 32px;
  background-color: #F97316;
  border-radius: 8px;
  flex-shrink: 0;
}

.chat-message-ai .chat-message-bubble {
  background-color: #F4F4F5;
  color: #18181B;
  border-radius: 16px 16px 16px 4px;
  padding: 12px 16px;
  max-width: 80%;
}

.chat-file-edit {
  display: flex;
  align-items: center;
  gap: 8px;
  padding: 8px 12px;
  background-color: #FFF7ED;
  border: 1px solid #FED7AA;
  border-radius: 8px;
  margin-top: 8px;
  font-size: 13px;
}

.chat-file-edit-icon {
  width: 16px;
  height: 16px;
  color: #F97316;
}

.chat-file-edit-name {
  font-weight: 500;
  color: #C2410C;
}

.chat-input-area {
  padding: 16px;
  border-top: 1px solid #E4E4E7;
}

.chat-input {
  width: 100%;
  padding: 12px 16px;
  border: 1px solid #E4E4E7;
  border-radius: 12px;
  font-size: 14px;
  resize: none;
}

.chat-input:focus {
  outline: none;
  border-color: #F97316;
}
```
