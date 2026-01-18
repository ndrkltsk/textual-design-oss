# Design System

## 1. Design & Brand Identity

### Design Philosophy
- **Minimalist and Clean**: The design emphasizes whitespace and clarity, allowing content to breathe
- **Trust and Intelligence**: The visual language conveys reliability and sophistication through refined typography and subtle color choices
- **Research-Focused**: UI elements support deep reading and exploration with clear information hierarchy
- **Conversational Interface**: The primary interaction model is conversational, with a prominent search/input area

### Visual Style Direction
- Modern, minimal aesthetic with organic warmth
- Soft, muted color palette with strategic use of teal accent
- Generous whitespace creating a calm, focused environment
- Rounded corners throughout for approachability
- Subtle shadows and borders for depth without heaviness

### Overall Mood and Tone
- Professional yet approachable
- Intelligent and trustworthy
- Clean and uncluttered
- Warm neutrals balanced with cool teal accents

### Brand Personality Expressed Through UI
- Sophisticated serif typography for headlines conveys authority and intelligence
- Teal accent color suggests knowledge, clarity, and innovation
- Cream/beige backgrounds create warmth and reduce eye strain for long reading sessions
- Minimalist icon style reinforces simplicity and focus

---

## 2. Design Tokens

### Colors

#### Primary Palette
```css
--color-primary: #1B9B8C;           /* Teal - primary brand color */
--color-primary-hover: #178A7C;     /* Teal - darker hover state */
--color-primary-light: #E8F5F3;     /* Teal - light background variant */
```

#### Secondary/Accent Colors
```css
--color-accent-olive: #5C6B4A;      /* Olive green - API platform buttons */
--color-accent-olive-dark: #3D4A2F; /* Dark olive - dark theme elements */
--color-accent-gold: #C9A227;       /* Gold/yellow - badges, highlights */
```

#### Neutral/Grayscale Scale
```css
--color-white: #FFFFFF;
--color-gray-50: #FAFAF8;           /* Off-white, main background */
--color-gray-100: #F5F5F0;          /* Light cream background */
--color-gray-150: #EEEEE8;          /* Card backgrounds, input backgrounds */
--color-gray-200: #E5E5E0;          /* Borders, dividers */
--color-gray-300: #D4D4D0;          /* Disabled borders */
--color-gray-400: #A3A3A0;          /* Placeholder text */
--color-gray-500: #737370;          /* Secondary text */
--color-gray-600: #525250;          /* Body text */
--color-gray-700: #404040;          /* Primary text */
--color-gray-800: #262626;          /* Headings */
--color-gray-900: #171717;          /* High contrast text */
--color-black: #000000;
```

#### Semantic Colors
```css
/* Success */
--color-success: #22C55E;
--color-success-light: #DCFCE7;
--color-success-dark: #16A34A;

/* Warning */
--color-warning: #F59E0B;
--color-warning-light: #FEF3C7;
--color-warning-dark: #D97706;

/* Error/Destructive */
--color-error: #991B1B;             /* Dark red for destructive actions */
--color-error-light: #FEE2E2;
--color-error-text: #DC2626;        /* Error text color */

/* Info */
--color-info: #3B82F6;
--color-info-light: #DBEAFE;
```

#### Background Colors
```css
--bg-page: #FAFAF8;                 /* Main page background */
--bg-surface: #FFFFFF;              /* Cards, modals */
--bg-surface-secondary: #F5F5F0;    /* Secondary surfaces */
--bg-input: #EEEEE8;                /* Input field backgrounds */
--bg-overlay: rgba(0, 0, 0, 0.5);   /* Modal overlay */
--bg-sidebar: #FFFFFF;              /* Sidebar background */
--bg-dark: #1A1F1E;                 /* Dark theme background */
--bg-dark-surface: #252B2A;         /* Dark theme cards */
```

#### Text Colors
```css
--text-primary: #262626;            /* Primary text */
--text-secondary: #525250;          /* Secondary text */
--text-muted: #737370;              /* Muted/helper text */
--text-placeholder: #A3A3A0;        /* Placeholder text */
--text-disabled: #D4D4D0;           /* Disabled text */
--text-inverse: #FFFFFF;            /* Text on dark backgrounds */
--text-link: #1B9B8C;               /* Link color */
--text-link-hover: #178A7C;         /* Link hover */
```

#### Border Colors
```css
--border-default: #E5E5E0;          /* Default borders */
--border-light: #EEEEE8;            /* Light borders */
--border-focus: #1B9B8C;            /* Focus ring color */
--border-error: #DC2626;            /* Error state borders */
```

#### Gradients
```css
/* Dark hero gradient (API landing) */
--gradient-dark-hero: linear-gradient(135deg, #1A1F1E 0%, #2D3532 100%);

/* Light cream gradient */
--gradient-light: linear-gradient(180deg, #FAFAF8 0%, #F5F5F0 100%);
```

### Typography

#### Font Families
```css
--font-primary: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
--font-display: 'Times New Roman', 'Georgia', serif;  /* For large headlines */
--font-mono: 'SF Mono', 'Monaco', 'Inconsolata', monospace;
```

#### Font Weights
```css
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
```

#### Type Scale
```css
/* Display - Serif headlines */
--text-display-xl: 72px;    /* Hero headlines */
--text-display-lg: 56px;    /* Large headlines */
--text-display-md: 44px;    /* Medium headlines */
--text-display-sm: 36px;    /* Small display */

/* Headings - Sans-serif */
--text-h1: 32px;
--text-h2: 24px;
--text-h3: 20px;
--text-h4: 18px;
--text-h5: 16px;
--text-h6: 14px;

/* Body */
--text-body-lg: 18px;
--text-body-md: 16px;
--text-body-sm: 14px;

/* Small */
--text-caption: 13px;
--text-label: 12px;
--text-micro: 11px;
```

#### Line Heights
```css
--leading-display: 1.1;     /* Display text */
--leading-tight: 1.25;      /* Headings */
--leading-normal: 1.5;      /* Body text */
--leading-relaxed: 1.625;   /* Long-form content */
--leading-loose: 1.75;      /* Extra spacing */
```

#### Letter Spacing
```css
--tracking-tighter: -0.02em;  /* Display headlines */
--tracking-tight: -0.01em;    /* Headings */
--tracking-normal: 0;         /* Body */
--tracking-wide: 0.025em;     /* Labels, uppercase */
--tracking-wider: 0.05em;     /* Small caps, buttons */
--tracking-widest: 0.1em;     /* All caps labels */
```

#### Text Styles Catalog
```css
/* Display Headline (Serif) */
.text-display-hero {
  font-family: var(--font-display);
  font-size: 72px;
  font-weight: 400;
  line-height: 1.1;
  letter-spacing: -0.02em;
  color: var(--text-primary);
}

/* Page Title */
.text-page-title {
  font-family: var(--font-primary);
  font-size: 32px;
  font-weight: 600;
  line-height: 1.25;
  color: var(--text-primary);
}

/* Section Header */
.text-section-header {
  font-family: var(--font-primary);
  font-size: 20px;
  font-weight: 600;
  line-height: 1.4;
  color: var(--text-primary);
}

/* Body Large */
.text-body-lg {
  font-family: var(--font-primary);
  font-size: 18px;
  font-weight: 400;
  line-height: 1.6;
  color: var(--text-secondary);
}

/* Body Default */
.text-body {
  font-family: var(--font-primary);
  font-size: 16px;
  font-weight: 400;
  line-height: 1.5;
  color: var(--text-secondary);
}

/* Body Small */
.text-body-sm {
  font-family: var(--font-primary);
  font-size: 14px;
  font-weight: 400;
  line-height: 1.5;
  color: var(--text-secondary);
}

/* Label */
.text-label {
  font-family: var(--font-primary);
  font-size: 12px;
  font-weight: 500;
  line-height: 1.4;
  letter-spacing: 0.025em;
  color: var(--text-muted);
}

/* Overline/Eyebrow */
.text-overline {
  font-family: var(--font-primary);
  font-size: 12px;
  font-weight: 500;
  line-height: 1.4;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--text-muted);
}

/* Code/Mono */
.text-code {
  font-family: var(--font-mono);
  font-size: 14px;
  font-weight: 400;
  line-height: 1.6;
  color: var(--text-primary);
}
```

### Spacing

#### Base Unit
```css
--spacing-unit: 4px;
```

#### Spacing Scale
```css
--space-0: 0;
--space-1: 4px;
--space-2: 8px;
--space-3: 12px;
--space-4: 16px;
--space-5: 20px;
--space-6: 24px;
--space-8: 32px;
--space-10: 40px;
--space-12: 48px;
--space-16: 64px;
--space-20: 80px;
--space-24: 96px;
--space-32: 128px;
```

#### Component Internal Padding
```css
--padding-button-sm: 8px 12px;
--padding-button-md: 10px 16px;
--padding-button-lg: 12px 24px;
--padding-input: 12px 16px;
--padding-card: 24px;
--padding-modal: 32px;
--padding-section: 48px;
```

#### Layout Margins and Gaps
```css
--gap-xs: 4px;
--gap-sm: 8px;
--gap-md: 16px;
--gap-lg: 24px;
--gap-xl: 32px;
--gap-2xl: 48px;
```

### Effects

#### Shadow Definitions
```css
/* Elevation Level 1 - Subtle */
--shadow-xs: 0 1px 2px rgba(0, 0, 0, 0.05);

/* Elevation Level 2 - Cards */
--shadow-sm: 0 1px 3px rgba(0, 0, 0, 0.08), 0 1px 2px rgba(0, 0, 0, 0.04);

/* Elevation Level 3 - Dropdowns */
--shadow-md: 0 4px 6px rgba(0, 0, 0, 0.07), 0 2px 4px rgba(0, 0, 0, 0.05);

/* Elevation Level 4 - Modals */
--shadow-lg: 0 10px 15px rgba(0, 0, 0, 0.1), 0 4px 6px rgba(0, 0, 0, 0.05);

/* Elevation Level 5 - Popovers */
--shadow-xl: 0 20px 25px rgba(0, 0, 0, 0.1), 0 10px 10px rgba(0, 0, 0, 0.04);

/* Focus ring */
--shadow-focus: 0 0 0 3px rgba(27, 155, 140, 0.25);
```

#### Blur Effects
```css
--blur-sm: 4px;
--blur-md: 8px;
--blur-lg: 16px;
--blur-overlay: 8px;  /* Backdrop blur for modals */
```

#### Opacity Values
```css
--opacity-disabled: 0.5;
--opacity-muted: 0.7;
--opacity-hover: 0.9;
--opacity-overlay: 0.5;
```

### Borders

#### Border Widths
```css
--border-width-none: 0;
--border-width-thin: 1px;
--border-width-medium: 2px;
--border-width-thick: 3px;
```

#### Border Radius Scale
```css
--radius-none: 0;
--radius-sm: 4px;
--radius-md: 8px;
--radius-lg: 12px;
--radius-xl: 16px;
--radius-2xl: 24px;
--radius-pill: 9999px;
--radius-circle: 50%;
```

#### Border Styles
```css
--border-default: 1px solid var(--border-default);
--border-light: 1px solid var(--border-light);
--border-focus: 2px solid var(--border-focus);
--border-error: 1px solid var(--color-error-text);
```

### Iconography

#### Icon Style
- **Style**: Outlined (line icons)
- **Stroke Weight**: 1.5px - 2px
- **Corner Style**: Rounded

#### Icon Sizes
```css
--icon-xs: 12px;
--icon-sm: 16px;
--icon-md: 20px;
--icon-lg: 24px;
--icon-xl: 32px;
--icon-2xl: 48px;
```

#### Icon Library
- Primary: Custom icon set with outlined style
- Fallback: Similar to Lucide Icons or Heroicons (outline variant)
- Characteristics: 24x24 viewbox, 1.5-2px stroke, rounded line caps

### Motion & Animation

#### Easing Curves
```css
--ease-default: cubic-bezier(0.4, 0, 0.2, 1);     /* Standard */
--ease-in: cubic-bezier(0.4, 0, 1, 1);            /* Acceleration */
--ease-out: cubic-bezier(0, 0, 0.2, 1);           /* Deceleration */
--ease-in-out: cubic-bezier(0.4, 0, 0.2, 1);      /* Standard */
--ease-bounce: cubic-bezier(0.68, -0.55, 0.265, 1.55);
```

#### Duration Scale
```css
--duration-instant: 0ms;
--duration-fast: 100ms;
--duration-normal: 200ms;
--duration-slow: 300ms;
--duration-slower: 400ms;
--duration-slowest: 500ms;
```

#### Transition Properties
```css
--transition-colors: color, background-color, border-color, fill, stroke;
--transition-transform: transform;
--transition-opacity: opacity;
--transition-shadow: box-shadow;
--transition-all: all;
```

#### Common Transitions
```css
--transition-button: background-color 200ms var(--ease-default),
                     border-color 200ms var(--ease-default),
                     color 200ms var(--ease-default);
--transition-input: border-color 200ms var(--ease-default),
                    box-shadow 200ms var(--ease-default);
--transition-card: box-shadow 200ms var(--ease-default),
                   transform 200ms var(--ease-default);
```

#### Animation Patterns
```css
/* Fade In */
@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

/* Slide Up */
@keyframes slideUp {
  from {
    opacity: 0;
    transform: translateY(8px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* Scale In */
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

/* Spinner */
@keyframes spin {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}
```

---

## 3. Components

### Buttons

#### Primary Button
```css
.button-primary {
  /* Dimensions */
  height: 40px;
  min-width: 80px;
  padding: 10px 20px;

  /* Visual */
  background-color: #1B9B8C;
  color: #FFFFFF;
  border: none;
  border-radius: 8px;

  /* Typography */
  font-family: var(--font-primary);
  font-size: 14px;
  font-weight: 500;

  /* States */
  cursor: pointer;
  transition: background-color 200ms ease;
}

.button-primary:hover {
  background-color: #178A7C;
}

.button-primary:active {
  background-color: #15756A;
}

.button-primary:focus-visible {
  outline: none;
  box-shadow: 0 0 0 3px rgba(27, 155, 140, 0.25);
}

.button-primary:disabled {
  background-color: #D4D4D0;
  color: #A3A3A0;
  cursor: not-allowed;
}
```

#### Secondary Button (Outline)
```css
.button-secondary {
  height: 40px;
  min-width: 80px;
  padding: 10px 20px;

  background-color: transparent;
  color: #262626;
  border: 1px solid #E5E5E0;
  border-radius: 8px;

  font-size: 14px;
  font-weight: 500;
}

.button-secondary:hover {
  background-color: #F5F5F0;
  border-color: #D4D4D0;
}
```

#### Destructive Button
```css
.button-destructive {
  height: 40px;
  padding: 10px 20px;

  background-color: #991B1B;
  color: #FFFFFF;
  border: none;
  border-radius: 8px;

  font-size: 14px;
  font-weight: 500;
}

.button-destructive:hover {
  background-color: #7F1D1D;
}
```

#### Ghost Button
```css
.button-ghost {
  height: 40px;
  padding: 10px 16px;

  background-color: transparent;
  color: #525250;
  border: none;
  border-radius: 8px;

  font-size: 14px;
  font-weight: 500;
}

.button-ghost:hover {
  background-color: #F5F5F0;
}
```

#### Icon Button
```css
.button-icon {
  width: 40px;
  height: 40px;
  padding: 8px;

  background-color: transparent;
  color: #525250;
  border: none;
  border-radius: 8px;

  display: flex;
  align-items: center;
  justify-content: center;
}

.button-icon:hover {
  background-color: #F5F5F0;
}
```

#### Button Sizes
```css
/* Small */
.button-sm {
  height: 32px;
  padding: 6px 12px;
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
  padding: 12px 24px;
  font-size: 16px;
}
```

### Inputs

#### Text Input
```css
.input {
  /* Dimensions */
  height: 44px;
  width: 100%;
  padding: 12px 16px;

  /* Visual */
  background-color: #EEEEE8;
  border: 1px solid transparent;
  border-radius: 8px;

  /* Typography */
  font-size: 15px;
  color: #262626;
}

.input::placeholder {
  color: #A3A3A0;
}

.input:hover {
  border-color: #D4D4D0;
}

.input:focus {
  outline: none;
  border-color: #1B9B8C;
  box-shadow: 0 0 0 3px rgba(27, 155, 140, 0.1);
}

.input:disabled {
  background-color: #F5F5F0;
  color: #A3A3A0;
  cursor: not-allowed;
}

.input--error {
  border-color: #DC2626;
}

.input--error:focus {
  box-shadow: 0 0 0 3px rgba(220, 38, 38, 0.1);
}
```

#### Textarea
```css
.textarea {
  min-height: 100px;
  padding: 12px 16px;
  resize: vertical;

  background-color: #EEEEE8;
  border: 1px solid transparent;
  border-radius: 8px;

  font-size: 15px;
  line-height: 1.5;
}
```

#### Select Dropdown
```css
.select {
  height: 44px;
  padding: 12px 40px 12px 16px;

  background-color: #EEEEE8;
  background-image: url("chevron-down.svg");
  background-repeat: no-repeat;
  background-position: right 12px center;
  background-size: 20px;

  border: 1px solid transparent;
  border-radius: 8px;

  font-size: 15px;
  appearance: none;
}
```

#### Checkbox
```css
.checkbox {
  width: 18px;
  height: 18px;

  border: 2px solid #D4D4D0;
  border-radius: 4px;

  appearance: none;
  cursor: pointer;
}

.checkbox:checked {
  background-color: #1B9B8C;
  border-color: #1B9B8C;
  background-image: url("check.svg");
  background-repeat: no-repeat;
  background-position: center;
}

.checkbox:focus-visible {
  box-shadow: 0 0 0 3px rgba(27, 155, 140, 0.25);
}
```

#### Radio Button
```css
.radio {
  width: 18px;
  height: 18px;

  border: 2px solid #D4D4D0;
  border-radius: 50%;

  appearance: none;
  cursor: pointer;
}

.radio:checked {
  border-color: #1B9B8C;
  border-width: 5px;
}
```

#### Toggle Switch
```css
.toggle {
  width: 44px;
  height: 24px;
  padding: 2px;

  background-color: #D4D4D0;
  border-radius: 12px;

  cursor: pointer;
  transition: background-color 200ms ease;
}

.toggle::after {
  content: '';
  width: 20px;
  height: 20px;
  background-color: #FFFFFF;
  border-radius: 50%;

  display: block;
  transition: transform 200ms ease;
}

.toggle:checked {
  background-color: #1B9B8C;
}

.toggle:checked::after {
  transform: translateX(20px);
}
```

### Search Bar (Main Component)
```css
.search-bar {
  /* Container */
  width: 100%;
  max-width: 680px;
  padding: 16px 20px;

  background-color: #FFFFFF;
  border: 1px solid #E5E5E0;
  border-radius: 16px;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.08);
}

.search-bar__input {
  width: 100%;
  border: none;
  background: transparent;

  font-size: 17px;
  color: #262626;
}

.search-bar__input::placeholder {
  color: #A3A3A0;
}

.search-bar__actions {
  display: flex;
  align-items: center;
  gap: 8px;
  margin-top: 12px;
  padding-top: 12px;
  border-top: 1px solid #EEEEE8;
}

.search-bar__submit {
  width: 44px;
  height: 44px;

  background-color: #1B9B8C;
  border-radius: 12px;

  display: flex;
  align-items: center;
  justify-content: center;
}
```

### Cards

#### Basic Card
```css
.card {
  padding: 24px;

  background-color: #FFFFFF;
  border: 1px solid #E5E5E0;
  border-radius: 12px;
}

.card:hover {
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.07);
}
```

#### Content Card (Discover Feed)
```css
.card-content {
  overflow: hidden;

  background-color: #FFFFFF;
  border-radius: 16px;

  transition: transform 200ms ease, box-shadow 200ms ease;
}

.card-content:hover {
  transform: translateY(-2px);
  box-shadow: 0 10px 15px rgba(0, 0, 0, 0.1);
}

.card-content__image {
  width: 100%;
  aspect-ratio: 16/9;
  object-fit: cover;
}

.card-content__body {
  padding: 16px 20px;
}

.card-content__title {
  font-size: 17px;
  font-weight: 600;
  color: #262626;
  line-height: 1.4;
}

.card-content__meta {
  display: flex;
  align-items: center;
  gap: 8px;
  margin-top: 8px;

  font-size: 13px;
  color: #737370;
}
```

#### Template Card
```css
.card-template {
  padding: 24px;

  background-color: #FFFFFF;
  border: 1px solid #E5E5E0;
  border-radius: 12px;

  cursor: pointer;
}

.card-template__icon {
  font-size: 32px;
  margin-bottom: 16px;
}

.card-template__title {
  font-size: 18px;
  font-weight: 600;
  color: #262626;
  margin-bottom: 8px;
}

.card-template__description {
  font-size: 14px;
  color: #525250;
  line-height: 1.5;
}
```

### Modals/Dialogs

#### Modal Container
```css
.modal-overlay {
  position: fixed;
  inset: 0;

  background-color: rgba(0, 0, 0, 0.5);
  backdrop-filter: blur(4px);

  display: flex;
  align-items: center;
  justify-content: center;

  z-index: 1000;
}

.modal {
  width: 100%;
  max-width: 560px;
  max-height: 90vh;

  background-color: #FFFFFF;
  border-radius: 16px;
  box-shadow: 0 20px 25px rgba(0, 0, 0, 0.1);

  overflow: hidden;
}

.modal__header {
  padding: 24px 24px 0;

  display: flex;
  align-items: center;
  justify-content: space-between;
}

.modal__title {
  font-size: 20px;
  font-weight: 600;
  color: #262626;
}

.modal__close {
  width: 32px;
  height: 32px;

  color: #737370;
  background: transparent;
  border: none;
  border-radius: 6px;

  cursor: pointer;
}

.modal__close:hover {
  background-color: #F5F5F0;
}

.modal__body {
  padding: 16px 24px 24px;
}

.modal__footer {
  padding: 16px 24px 24px;

  display: flex;
  justify-content: flex-end;
  gap: 12px;
}
```

### Dropdowns/Menus

#### Dropdown Menu
```css
.dropdown {
  min-width: 200px;
  padding: 8px 0;

  background-color: #FFFFFF;
  border: 1px solid #E5E5E0;
  border-radius: 12px;
  box-shadow: 0 10px 15px rgba(0, 0, 0, 0.1);
}

.dropdown__item {
  padding: 10px 16px;

  display: flex;
  align-items: center;
  gap: 12px;

  font-size: 14px;
  color: #262626;

  cursor: pointer;
  transition: background-color 150ms ease;
}

.dropdown__item:hover {
  background-color: #F5F5F0;
}

.dropdown__item--selected {
  color: #1B9B8C;
}

.dropdown__item--selected::after {
  content: '✓';
  margin-left: auto;
  color: #1B9B8C;
}

.dropdown__divider {
  height: 1px;
  margin: 8px 0;
  background-color: #E5E5E0;
}
```

#### Popover (Upgrade/Feature)
```css
.popover {
  width: 280px;
  padding: 20px;

  background-color: #1A1F1E;
  border-radius: 12px;
  box-shadow: 0 20px 25px rgba(0, 0, 0, 0.2);

  color: #FFFFFF;
}

.popover__title {
  font-size: 16px;
  font-weight: 600;
  margin-bottom: 4px;
}

.popover__description {
  font-size: 14px;
  color: rgba(255, 255, 255, 0.7);
  line-height: 1.5;
  margin-bottom: 16px;
}

.popover__cta {
  width: 100%;
  padding: 12px;

  background-color: #1B9B8C;
  border-radius: 8px;

  font-size: 14px;
  font-weight: 500;
  color: #FFFFFF;
  text-align: center;
}
```

### Navigation

#### Sidebar Navigation
```css
.sidebar {
  width: 72px;
  height: 100vh;
  padding: 16px 12px;

  background-color: #FFFFFF;
  border-right: 1px solid #E5E5E0;

  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 8px;
}

.sidebar__logo {
  width: 40px;
  height: 40px;
  margin-bottom: 16px;
}

.sidebar__item {
  width: 48px;
  height: 48px;

  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 4px;

  color: #737370;
  border-radius: 8px;

  cursor: pointer;
  transition: background-color 150ms ease;
}

.sidebar__item:hover {
  background-color: #F5F5F0;
}

.sidebar__item--active {
  color: #1B9B8C;
  background-color: #E8F5F3;
}

.sidebar__item-icon {
  width: 20px;
  height: 20px;
}

.sidebar__item-label {
  font-size: 10px;
  font-weight: 500;
}
```

#### Header Navigation (Enterprise)
```css
.header {
  height: 64px;
  padding: 0 24px;

  background-color: #FFFFFF;
  border-bottom: 1px solid #E5E5E0;

  display: flex;
  align-items: center;
  justify-content: space-between;
}

.header__logo {
  display: flex;
  align-items: center;
  gap: 8px;

  font-size: 18px;
  font-weight: 600;
  color: #262626;
}

.header__nav {
  display: flex;
  align-items: center;
  gap: 32px;
}

.header__nav-item {
  font-size: 15px;
  font-weight: 500;
  color: #525250;

  transition: color 150ms ease;
}

.header__nav-item:hover {
  color: #262626;
}

.header__cta {
  padding: 10px 20px;

  background-color: #1B9B8C;
  border-radius: 24px;

  font-size: 14px;
  font-weight: 500;
  color: #FFFFFF;
}
```

#### Tabs
```css
.tabs {
  display: flex;
  gap: 4px;
  padding: 4px;

  background-color: #F5F5F0;
  border-radius: 10px;
}

.tab {
  padding: 8px 16px;

  font-size: 14px;
  font-weight: 500;
  color: #737370;

  border-radius: 8px;
  cursor: pointer;
  transition: all 150ms ease;
}

.tab:hover {
  color: #525250;
}

.tab--active {
  background-color: #FFFFFF;
  color: #262626;
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.05);
}
```

#### Underline Tabs
```css
.tabs-underline {
  display: flex;
  gap: 24px;
  border-bottom: 1px solid #E5E5E0;
}

.tab-underline {
  padding: 12px 0;

  font-size: 15px;
  font-weight: 500;
  color: #737370;

  border-bottom: 2px solid transparent;
  margin-bottom: -1px;

  cursor: pointer;
}

.tab-underline:hover {
  color: #525250;
}

.tab-underline--active {
  color: #262626;
  border-bottom-color: #1B9B8C;
}
```

### Badges/Tags/Chips

#### Badge
```css
.badge {
  display: inline-flex;
  align-items: center;
  padding: 2px 8px;

  font-size: 11px;
  font-weight: 500;
  text-transform: uppercase;
  letter-spacing: 0.5px;

  border-radius: 4px;
}

.badge--new {
  background-color: #E8F5F3;
  color: #1B9B8C;
}

.badge--max {
  background-color: #FEF3C7;
  color: #92400E;
}

.badge--pro {
  background-color: #1B9B8C;
  color: #FFFFFF;
}
```

#### Chip (Category)
```css
.chip {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  padding: 8px 16px;

  background-color: #FFFFFF;
  border: 1px solid #E5E5E0;
  border-radius: 24px;

  font-size: 14px;
  font-weight: 500;
  color: #525250;

  cursor: pointer;
  transition: all 150ms ease;
}

.chip:hover {
  background-color: #F5F5F0;
  border-color: #D4D4D0;
}

.chip--selected {
  background-color: #E8F5F3;
  border-color: #1B9B8C;
  color: #1B9B8C;
}

.chip__icon {
  width: 16px;
  height: 16px;
}
```

#### Source Citation Tag
```css
.source-tag {
  display: inline-flex;
  align-items: center;
  padding: 2px 8px;

  background-color: #EEEEE8;
  border-radius: 4px;

  font-family: var(--font-mono);
  font-size: 12px;
  color: #525250;
}

.source-tag--count {
  margin-left: 4px;
  color: #737370;
}
```

### Avatars
```css
.avatar {
  width: 32px;
  height: 32px;

  background-color: #E5E5E0;
  border-radius: 50%;

  display: flex;
  align-items: center;
  justify-content: center;

  font-size: 14px;
  font-weight: 500;
  color: #525250;
}

.avatar--sm { width: 24px; height: 24px; font-size: 11px; }
.avatar--md { width: 32px; height: 32px; font-size: 14px; }
.avatar--lg { width: 40px; height: 40px; font-size: 16px; }
.avatar--xl { width: 48px; height: 48px; font-size: 18px; }

.avatar__image {
  width: 100%;
  height: 100%;
  border-radius: 50%;
  object-fit: cover;
}
```

### Tooltips
```css
.tooltip {
  padding: 8px 12px;

  background-color: #262626;
  border-radius: 6px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);

  font-size: 13px;
  color: #FFFFFF;

  max-width: 250px;
}

.tooltip--light {
  background-color: #FFFFFF;
  border: 1px solid #E5E5E0;
  color: #262626;
}
```

### Alerts/Banners

#### Info Banner
```css
.banner {
  padding: 12px 16px;

  display: flex;
  align-items: center;
  gap: 12px;

  border-radius: 8px;
}

.banner--info {
  background-color: #E8F5F3;
  color: #1B9B8C;
}

.banner--warning {
  background-color: #FEF3C7;
  color: #92400E;
}

.banner--error {
  background-color: #FEE2E2;
  color: #991B1B;
}

.banner--success {
  background-color: #DCFCE7;
  color: #166534;
}
```

#### Toast Notification
```css
.toast {
  min-width: 300px;
  padding: 16px 20px;

  background-color: #FFFFFF;
  border: 1px solid #E5E5E0;
  border-radius: 12px;
  box-shadow: 0 10px 15px rgba(0, 0, 0, 0.1);

  display: flex;
  align-items: flex-start;
  gap: 12px;
}

.toast__icon {
  width: 20px;
  height: 20px;
  flex-shrink: 0;
}

.toast__icon--success { color: #22C55E; }
.toast__icon--error { color: #DC2626; }
.toast__icon--warning { color: #F59E0B; }
.toast__icon--info { color: #1B9B8C; }

.toast__content {
  flex: 1;
}

.toast__title {
  font-size: 14px;
  font-weight: 500;
  color: #262626;
}

.toast__message {
  font-size: 14px;
  color: #525250;
  margin-top: 4px;
}
```

### Progress Indicators

#### Spinner
```css
.spinner {
  width: 20px;
  height: 20px;

  border: 2px solid #E5E5E0;
  border-top-color: #1B9B8C;
  border-radius: 50%;

  animation: spin 600ms linear infinite;
}

.spinner--sm { width: 16px; height: 16px; border-width: 2px; }
.spinner--md { width: 20px; height: 20px; border-width: 2px; }
.spinner--lg { width: 32px; height: 32px; border-width: 3px; }
```

#### Progress Bar
```css
.progress-bar {
  height: 4px;
  background-color: #E5E5E0;
  border-radius: 2px;
  overflow: hidden;
}

.progress-bar__fill {
  height: 100%;
  background-color: #1B9B8C;
  border-radius: 2px;
  transition: width 300ms ease;
}
```

### Form Components

#### Form Field
```css
.form-field {
  margin-bottom: 20px;
}

.form-field__label {
  display: block;
  margin-bottom: 8px;

  font-size: 14px;
  font-weight: 500;
  color: #262626;
}

.form-field__required {
  color: #DC2626;
  margin-left: 2px;
}

.form-field__helper {
  margin-top: 6px;

  font-size: 13px;
  color: #737370;
}

.form-field__error {
  margin-top: 6px;

  font-size: 13px;
  color: #DC2626;
}
```

#### Selection Option (Checkbox/Radio Card)
```css
.selection-option {
  padding: 16px;

  display: flex;
  align-items: center;
  gap: 12px;

  background-color: #FFFFFF;
  border: 1px solid #E5E5E0;
  border-radius: 8px;

  cursor: pointer;
  transition: all 150ms ease;
}

.selection-option:hover {
  border-color: #D4D4D0;
}

.selection-option--selected {
  border-color: #1B9B8C;
  background-color: #FAFAF8;
}

.selection-option__icon {
  width: 20px;
  height: 20px;
  color: #737370;
}

.selection-option--selected .selection-option__icon {
  color: #1B9B8C;
}

.selection-option__label {
  font-size: 14px;
  color: #262626;
}
```

### Stock/Finance Components

#### Stock Ticker
```css
.stock-ticker {
  padding: 16px;

  background-color: #FFFFFF;
  border: 1px solid #E5E5E0;
  border-radius: 8px;
}

.stock-ticker__symbol {
  font-size: 14px;
  font-weight: 600;
  color: #262626;
}

.stock-ticker__price {
  font-size: 24px;
  font-weight: 600;
  color: #262626;
  margin-top: 4px;
}

.stock-ticker__change {
  display: inline-flex;
  align-items: center;
  gap: 4px;

  font-size: 13px;
  font-family: var(--font-mono);
}

.stock-ticker__change--positive {
  color: #22C55E;
}

.stock-ticker__change--negative {
  color: #DC2626;
}
```

### Announcement Banner
```css
.announcement-banner {
  height: 40px;
  padding: 0 16px;

  background-color: #1B9B8C;
  color: #FFFFFF;

  display: flex;
  align-items: center;
  justify-content: center;
  gap: 8px;

  font-size: 14px;
  font-weight: 500;
}

.announcement-banner__link {
  color: #FFFFFF;
  text-decoration: underline;
  font-weight: 600;
}

.announcement-banner__icon {
  width: 16px;
  height: 16px;
}
```

### Sign-In Panel (Side Panel)
```css
.sign-in-panel {
  width: 380px;
  padding: 32px;

  background-color: #FFFFFF;
  border-radius: 16px;
  box-shadow: 0 20px 25px rgba(0, 0, 0, 0.1);
}

.sign-in-panel__logo {
  width: 48px;
  height: 48px;
  margin: 0 auto 24px;
  color: #1B9B8C;
}

.sign-in-panel__title {
  font-size: 20px;
  font-weight: 600;
  color: #262626;
  text-align: center;
  margin-bottom: 8px;
}

.sign-in-panel__subtitle {
  font-size: 14px;
  color: #737370;
  text-align: center;
  margin-bottom: 24px;
}

.sign-in-panel__divider {
  display: flex;
  align-items: center;
  gap: 16px;
  margin: 20px 0;

  font-size: 13px;
  color: #737370;
}

.sign-in-panel__divider::before,
.sign-in-panel__divider::after {
  content: '';
  flex: 1;
  height: 1px;
  background-color: #E5E5E0;
}
```

### Social Login Buttons
```css
.social-button {
  width: 100%;
  height: 48px;
  padding: 12px 20px;

  display: flex;
  align-items: center;
  justify-content: center;
  gap: 12px;

  border-radius: 8px;
  font-size: 15px;
  font-weight: 500;

  cursor: pointer;
  transition: all 200ms ease;
}

.social-button--google {
  background-color: #1B9B8C;
  color: #FFFFFF;
  border: none;
}

.social-button--google:hover {
  background-color: #178A7C;
}

.social-button--apple {
  background-color: #FFFFFF;
  color: #262626;
  border: 1px solid #E5E5E0;
}

.social-button--apple:hover {
  background-color: #F5F5F0;
}

.social-button__icon {
  width: 20px;
  height: 20px;
}
```

### OTP/Code Input
```css
.otp-input {
  display: flex;
  gap: 8px;
  justify-content: center;
}

.otp-input__digit {
  width: 48px;
  height: 56px;

  background-color: #EEEEE8;
  border: 1px solid transparent;
  border-radius: 8px;

  font-size: 24px;
  font-weight: 600;
  text-align: center;
  color: #262626;
}

.otp-input__digit:focus {
  border-color: #1B9B8C;
  box-shadow: 0 0 0 3px rgba(27, 155, 140, 0.1);
}
```

### Segmented Control
```css
.segmented-control {
  display: inline-flex;
  padding: 4px;

  background-color: #EEEEE8;
  border-radius: 8px;
}

.segmented-control__option {
  padding: 8px 16px;

  font-size: 14px;
  font-weight: 500;
  color: #737370;

  border-radius: 6px;
  cursor: pointer;
  transition: all 150ms ease;
}

.segmented-control__option:hover {
  color: #525250;
}

.segmented-control__option--active {
  background-color: #FFFFFF;
  color: #262626;
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.05);
}
```

### Calendar/Date Picker
```css
.calendar {
  width: 280px;
  padding: 16px;

  background-color: #FFFFFF;
  border: 1px solid #E5E5E0;
  border-radius: 12px;
  box-shadow: 0 10px 15px rgba(0, 0, 0, 0.1);
}

.calendar__header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-bottom: 16px;
}

.calendar__title {
  font-size: 16px;
  font-weight: 600;
  color: #262626;
}

.calendar__nav-button {
  width: 32px;
  height: 32px;

  display: flex;
  align-items: center;
  justify-content: center;

  color: #737370;
  border: 1px solid #E5E5E0;
  border-radius: 8px;

  cursor: pointer;
}

.calendar__weekdays {
  display: grid;
  grid-template-columns: repeat(7, 1fr);
  gap: 4px;
  margin-bottom: 8px;
}

.calendar__weekday {
  font-size: 12px;
  font-weight: 500;
  color: #737370;
  text-align: center;
  padding: 4px;
}

.calendar__days {
  display: grid;
  grid-template-columns: repeat(7, 1fr);
  gap: 4px;
}

.calendar__day {
  width: 36px;
  height: 36px;

  display: flex;
  align-items: center;
  justify-content: center;

  font-size: 14px;
  color: #262626;
  border-radius: 8px;

  cursor: pointer;
  transition: background-color 150ms ease;
}

.calendar__day:hover {
  background-color: #F5F5F0;
}

.calendar__day--today {
  background-color: #E8F5F3;
  color: #1B9B8C;
  font-weight: 600;
}

.calendar__day--selected {
  background-color: #1B9B8C;
  color: #FFFFFF;
}

.calendar__day--outside {
  color: #A3A3A0;
}
```

### Related Questions List
```css
.related-questions {
  margin-top: 32px;
}

.related-questions__title {
  font-size: 18px;
  font-weight: 600;
  color: #262626;
  margin-bottom: 16px;
}

.related-question {
  padding: 12px 0;

  display: flex;
  align-items: center;
  gap: 12px;

  border-bottom: 1px solid #EEEEE8;
  cursor: pointer;
  transition: color 150ms ease;
}

.related-question:hover {
  color: #1B9B8C;
}

.related-question__icon {
  width: 16px;
  height: 16px;
  color: #A3A3A0;
  flex-shrink: 0;
}

.related-question__text {
  font-size: 15px;
  color: #262626;
}

.related-question:hover .related-question__text {
  color: #1B9B8C;
}
```

### Action Bar (Answer Actions)
```css
.action-bar {
  display: flex;
  align-items: center;
  gap: 4px;
  padding: 8px 0;
}

.action-bar__button {
  width: 36px;
  height: 36px;

  display: flex;
  align-items: center;
  justify-content: center;

  color: #737370;
  background: transparent;
  border: none;
  border-radius: 8px;

  cursor: pointer;
  transition: all 150ms ease;
}

.action-bar__button:hover {
  background-color: #F5F5F0;
  color: #525250;
}

.action-bar__button--active {
  color: #1B9B8C;
}

.action-bar__divider {
  width: 1px;
  height: 24px;
  background-color: #E5E5E0;
  margin: 0 8px;
}

.action-bar__sources {
  display: flex;
  align-items: center;
  gap: 4px;
  padding: 4px 8px;

  font-size: 13px;
  color: #737370;
}
```

### Keyboard Shortcut Badge
```css
.kbd {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  min-width: 24px;
  height: 24px;
  padding: 0 6px;

  background-color: #EEEEE8;
  border: 1px solid #E5E5E0;
  border-radius: 4px;

  font-family: var(--font-mono);
  font-size: 12px;
  font-weight: 500;
  color: #525250;
}
```

### Place Card (Maps)
```css
.place-card {
  display: flex;
  gap: 12px;
  padding: 12px;

  background-color: #FFFFFF;
  border: 1px solid #E5E5E0;
  border-radius: 12px;

  cursor: pointer;
  transition: box-shadow 200ms ease;
}

.place-card:hover {
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.07);
}

.place-card__image {
  width: 80px;
  height: 80px;
  border-radius: 8px;
  object-fit: cover;
  flex-shrink: 0;
}

.place-card__content {
  flex: 1;
  min-width: 0;
}

.place-card__name {
  font-size: 16px;
  font-weight: 600;
  color: #1B9B8C;
  margin-bottom: 4px;
}

.place-card__address {
  font-size: 13px;
  color: #737370;
  margin-bottom: 8px;
}

.place-card__rating {
  display: flex;
  align-items: center;
  gap: 4px;

  font-size: 13px;
  color: #262626;
}

.place-card__rating-star {
  color: #F59E0B;
}

.place-card__rating-count {
  color: #737370;
}
```

### Expanded Sidebar (with Library)
```css
.sidebar-expanded {
  width: 260px;
  height: 100vh;
  padding: 16px;

  background-color: #FFFFFF;
  border-right: 1px solid #E5E5E0;

  display: flex;
  flex-direction: column;
}

.sidebar-expanded__section {
  margin-bottom: 24px;
}

.sidebar-expanded__section-title {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 8px 12px;

  font-size: 12px;
  font-weight: 600;
  color: #737370;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}

.sidebar-expanded__item {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 10px 12px;

  font-size: 14px;
  color: #262626;
  border-radius: 8px;

  cursor: pointer;
  transition: background-color 150ms ease;
}

.sidebar-expanded__item:hover {
  background-color: #F5F5F0;
}

.sidebar-expanded__item--active {
  background-color: #E8F5F3;
  color: #1B9B8C;
}

.sidebar-expanded__item-icon {
  width: 20px;
  height: 20px;
  color: #737370;
}

.sidebar-expanded__item--active .sidebar-expanded__item-icon {
  color: #1B9B8C;
}
```

### Context Menu
```css
.context-menu {
  min-width: 180px;
  padding: 6px 0;

  background-color: #FFFFFF;
  border: 1px solid #E5E5E0;
  border-radius: 10px;
  box-shadow: 0 10px 15px rgba(0, 0, 0, 0.1);
}

.context-menu__item {
  display: flex;
  align-items: center;
  gap: 10px;
  padding: 8px 14px;

  font-size: 14px;
  color: #262626;

  cursor: pointer;
  transition: background-color 150ms ease;
}

.context-menu__item:hover {
  background-color: #F5F5F0;
}

.context-menu__item--destructive {
  color: #DC2626;
}

.context-menu__item-icon {
  width: 16px;
  height: 16px;
  color: #737370;
}

.context-menu__item--destructive .context-menu__item-icon {
  color: #DC2626;
}

.context-menu__separator {
  height: 1px;
  margin: 6px 0;
  background-color: #E5E5E0;
}
```

### Share Popover
```css
.share-popover {
  width: 320px;
  padding: 20px;

  background-color: #FFFFFF;
  border: 1px solid #E5E5E0;
  border-radius: 12px;
  box-shadow: 0 10px 15px rgba(0, 0, 0, 0.1);
}

.share-popover__title {
  font-size: 16px;
  font-weight: 600;
  color: #262626;
  margin-bottom: 16px;
}

.share-popover__option {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 10px 12px;
  margin-bottom: 4px;

  border-radius: 8px;
  cursor: pointer;
  transition: background-color 150ms ease;
}

.share-popover__option:hover {
  background-color: #F5F5F0;
}

.share-popover__option--selected {
  background-color: #E8F5F3;
}

.share-popover__option-icon {
  width: 20px;
  height: 20px;
  color: #737370;
}

.share-popover__option--selected .share-popover__option-icon {
  color: #1B9B8C;
}

.share-popover__option-text {
  flex: 1;
}

.share-popover__option-label {
  font-size: 14px;
  font-weight: 500;
  color: #262626;
}

.share-popover__option-description {
  font-size: 12px;
  color: #737370;
}

.share-popover__check {
  width: 16px;
  height: 16px;
  color: #1B9B8C;
}

.share-popover__success {
  display: flex;
  align-items: center;
  gap: 8px;
  padding: 8px 12px;
  margin-top: 12px;

  background-color: #E8F5F3;
  border-radius: 6px;

  font-size: 13px;
  color: #1B9B8C;
}

.share-popover__copy-button {
  width: 100%;
  margin-top: 16px;
}
```

---

## 4. Layout System

### Grid System
```css
/* 12-column grid */
.grid {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  gap: 24px;
}

/* Column spans */
.col-1 { grid-column: span 1; }
.col-2 { grid-column: span 2; }
.col-3 { grid-column: span 3; }
.col-4 { grid-column: span 4; }
.col-6 { grid-column: span 6; }
.col-8 { grid-column: span 8; }
.col-12 { grid-column: span 12; }
```

### Container Max-Widths
```css
--container-sm: 640px;
--container-md: 768px;
--container-lg: 1024px;
--container-xl: 1280px;
--container-2xl: 1440px;

.container {
  width: 100%;
  max-width: var(--container-xl);
  margin: 0 auto;
  padding: 0 24px;
}

.container--narrow {
  max-width: 768px;
}

.container--wide {
  max-width: 1440px;
}
```

### Breakpoints
```css
--breakpoint-sm: 640px;
--breakpoint-md: 768px;
--breakpoint-lg: 1024px;
--breakpoint-xl: 1280px;
--breakpoint-2xl: 1536px;

/* Mobile first approach */
@media (min-width: 640px) { /* sm */ }
@media (min-width: 768px) { /* md */ }
@media (min-width: 1024px) { /* lg */ }
@media (min-width: 1280px) { /* xl */ }
@media (min-width: 1536px) { /* 2xl */ }
```

### Page Layout Templates

#### App Layout (with Sidebar)
```css
.app-layout {
  display: flex;
  min-height: 100vh;
}

.app-layout__sidebar {
  width: 72px;
  flex-shrink: 0;
  position: fixed;
  left: 0;
  top: 0;
  height: 100vh;
}

.app-layout__main {
  flex: 1;
  margin-left: 72px;
  min-height: 100vh;
  background-color: var(--bg-page);
}

.app-layout__content {
  max-width: 900px;
  margin: 0 auto;
  padding: 40px 24px;
}
```

#### Marketing Layout
```css
.marketing-layout {
  min-height: 100vh;
}

.marketing-layout__header {
  position: sticky;
  top: 0;
  z-index: 100;
  background-color: #FFFFFF;
}

.marketing-layout__main {
  background-color: var(--bg-page);
}

.marketing-layout__footer {
  background-color: #1A1F1E;
  color: #FFFFFF;
}
```

### Content Width Constraints
```css
/* Reading width for long-form content */
.content-readable {
  max-width: 680px;
}

/* Search bar width */
.content-search {
  max-width: 680px;
}

/* Card grid container */
.content-grid {
  max-width: 1200px;
}
```

### Vertical Rhythm
```css
/* Section spacing */
--section-gap-sm: 48px;
--section-gap-md: 80px;
--section-gap-lg: 120px;

/* Content spacing */
--content-gap-xs: 8px;
--content-gap-sm: 16px;
--content-gap-md: 24px;
--content-gap-lg: 32px;
```

---

## 5. Patterns

### Navigation Patterns

#### Header Behavior
- Fixed/sticky on scroll for marketing pages
- Static for app pages
- Height: 64px
- Background: White with subtle bottom border

#### Mobile Navigation
- Hamburger menu icon (3 horizontal lines)
- Full-screen overlay navigation
- Slide-in animation from right

#### Sidebar Behavior
- Fixed position on left
- Collapsed width: 72px
- Icon + label layout
- Active state: teal background highlight

### Form Patterns

#### Form Layout
- Labels positioned above inputs
- 8px gap between label and input
- 20px gap between form fields
- Error messages appear below inputs
- Required indicator: red asterisk after label

#### Validation Display
- Real-time validation on blur
- Error text in red (#DC2626)
- Error border on input
- Helper text in gray below inputs
- Error icon optional

#### Input Group Patterns
```css
/* Side-by-side inputs */
.input-group {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 16px;
}

/* Input with button */
.input-with-action {
  display: flex;
  gap: 8px;
}
```

### Content Patterns

#### Card Grid Layouts
```css
/* 3-column cards */
.card-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 24px;
}

/* 2-column with sidebar */
.card-grid--with-sidebar {
  display: grid;
  grid-template-columns: 2fr 1fr;
  gap: 32px;
}

/* Auto-fit responsive grid */
.card-grid--responsive {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 24px;
}
```

#### Empty States
```css
.empty-state {
  text-align: center;
  padding: 48px 24px;
}

.empty-state__icon {
  width: 64px;
  height: 64px;
  margin: 0 auto 16px;
  color: #A3A3A0;
}

.empty-state__title {
  font-size: 18px;
  font-weight: 500;
  color: #262626;
  margin-bottom: 8px;
}

.empty-state__description {
  font-size: 14px;
  color: #737370;
  max-width: 320px;
  margin: 0 auto;
}
```

#### Loading States
```css
/* Skeleton loading */
.skeleton {
  background: linear-gradient(90deg, #EEEEE8 25%, #F5F5F0 50%, #EEEEE8 75%);
  background-size: 200% 100%;
  animation: shimmer 1.5s infinite;
  border-radius: 4px;
}

@keyframes shimmer {
  0% { background-position: 200% 0; }
  100% { background-position: -200% 0; }
}

.skeleton--text {
  height: 16px;
  width: 80%;
}

.skeleton--title {
  height: 24px;
  width: 60%;
}

.skeleton--avatar {
  width: 40px;
  height: 40px;
  border-radius: 50%;
}
```

### Feedback Patterns

#### Toast/Notification Positioning
- Position: fixed, bottom-right
- Offset: 24px from edges
- Stack multiple toasts vertically with 8px gap
- Auto-dismiss after 5 seconds
- Slide-up animation on entry, slide-down on exit

#### Modal Overlay
- Background: rgba(0, 0, 0, 0.5)
- Backdrop blur: 4px
- Modal scales up from 95% to 100% on open
- Click outside to close (unless destructive action)

#### Confirmation Dialogs
- Centered modal
- Clear destructive action in red
- Primary action on right
- "Cancel" / "Nevermind" as secondary action

---

## 6. Page Templates

### Home/Search Page
```
┌────────────────────────────────────────────────────────┐
│  Sidebar  │                                            │
│  (72px)   │              Logo/Brand                    │
│           │                                            │
│  [Home]   │         ┌────────────────────┐             │
│  [Disc]   │         │   Search Input     │             │
│  [Space]  │         │   [Actions Row]    │             │
│  [Fin]    │         └────────────────────┘             │
│           │                                            │
│           │       [Chip] [Chip] [Chip] [Chip]          │
│           │                                            │
│  ───────  │                                            │
│  [Notif]  │                                            │
│  [Acct]   │                                            │
│  [Upgr]   │                                            │
│  [Inst]   │                                            │
└────────────────────────────────────────────────────────┘
```

### Search Results/Answer Page
```
┌────────────────────────────────────────────────────────┐
│  Sidebar  │  Title                       [Share]       │
│           │  ─────────────────────────────────────     │
│           │  [Answer] [Images] [Places]                │
│           │                                            │
│           │  Answer content with citations...          │
│           │  [source] [source] ...                     │
│           │                                            │
│           │  [Actions: Share, Copy, Export, Vote]      │
│           │                                            │
│           │  Related                                   │
│           │  └─ Question 1                             │
│           │  └─ Question 2                             │
│           │                                            │
│           │  ┌────────────────────┐                    │
│           │  │   Follow-up input   │                   │
│           │  └────────────────────┘                    │
└────────────────────────────────────────────────────────┘
```

### Discover/Feed Page
```
┌────────────────────────────────────────────────────────┐
│  Sidebar  │  Discover                    [Share]       │
│           │  ─────────────────────────────────────     │
│           │  [For You] [Top] [Topics ▼]                │
│           │                                            │
│           │  ┌─────────────────────┐  ┌───────────┐   │
│           │  │                     │  │ Weather   │   │
│           │  │   Featured Card     │  │           │   │
│           │  │                     │  │ Markets   │   │
│           │  └─────────────────────┘  │           │   │
│           │                           │ Trending  │   │
│           │  ┌───────┐ ┌───────┐ ┌───│           │   │
│           │  │ Card  │ │ Card  │ │ Ca└───────────┘   │
│           │  └───────┘ └───────┘ └───────┘           │
└────────────────────────────────────────────────────────┘
```

### Settings Page
```
┌────────────────────────────────────────────────────────┐
│  ← Back                                                │
│                                                        │
│  Account                                               │
│  ├─ Account                                            │
│  ├─ Preferences                                        │
│  ├─ Personalization                                    │
│  ├─ Assistant                                          │
│  ├─ Tasks                                              │
│  └─ ...                                                │
│                                                        │
│  Workspace                                             │
│  ├─ API                                                │
│  └─ Enterprise                                         │
│                                                        │
│  [User] ✓                                              │
│  [Incognito]                                           │
└────────────────────────────────────────────────────────┘
```

### Hero Section (Marketing)
- Full-width section
- Large serif headline (display text)
- Subheadline in regular body text
- 1-2 CTA buttons
- Background: light cream or dark with gradient
- Optional: decorative illustration or product screenshot

---

## 7. Imagery & Media

### Image Aspect Ratios
```css
--aspect-hero: 16 / 9;      /* Hero images */
--aspect-card: 16 / 9;      /* Card thumbnails */
--aspect-square: 1 / 1;     /* Avatars, icons */
--aspect-portrait: 3 / 4;   /* Profile images */
--aspect-landscape: 4 / 3;  /* Gallery images */
```

### Image Border Treatments
```css
.image-default {
  border-radius: 12px;
  overflow: hidden;
}

.image-card {
  border-radius: 12px 12px 0 0;
}

.image-avatar {
  border-radius: 50%;
}
```

### Placeholder/Fallback Styles
```css
.image-placeholder {
  background-color: #EEEEE8;
  display: flex;
  align-items: center;
  justify-content: center;
}

.image-placeholder__icon {
  color: #A3A3A0;
  width: 48px;
  height: 48px;
}
```

### Avatar Sizes and Fallbacks
```css
/* Fallback initials */
.avatar-fallback {
  background-color: #E8F5F3;
  color: #1B9B8C;
  font-weight: 500;
}

/* Company logos in lists */
.logo-thumbnail {
  width: 40px;
  height: 40px;
  border-radius: 8px;
  background-color: #FFFFFF;
  border: 1px solid #E5E5E0;
  object-fit: contain;
  padding: 4px;
}
```

---

## 8. Accessibility

### Color Contrast Ratios
- Text on light backgrounds: minimum 4.5:1 (AA)
- Large text (18px+): minimum 3:1
- UI components: minimum 3:1
- Primary text (#262626) on cream (#FAFAF8): ~14:1 ✓
- Secondary text (#525250) on white: ~7:1 ✓
- Teal (#1B9B8C) on white: ~4.6:1 ✓

### Focus Indicator Styles
```css
/* Visible focus ring for keyboard navigation */
:focus-visible {
  outline: none;
  box-shadow: 0 0 0 3px rgba(27, 155, 140, 0.4);
}

/* Remove focus for mouse users */
:focus:not(:focus-visible) {
  outline: none;
  box-shadow: none;
}

/* High contrast focus for buttons */
.button:focus-visible {
  box-shadow: 0 0 0 3px rgba(27, 155, 140, 0.4),
              0 0 0 5px rgba(27, 155, 140, 0.1);
}
```

### Touch Target Sizes
```css
/* Minimum touch target: 44x44px */
--touch-target-min: 44px;

/* Interactive elements should have adequate hit areas */
.touch-target {
  min-width: 44px;
  min-height: 44px;
}

/* For smaller visual elements, use padding */
.icon-button {
  width: 32px;
  height: 32px;
  padding: 6px;
  /* Creates 44x44 touch area with the visual being 32x32 */
}
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
  padding: 8px 16px;
  background-color: #1B9B8C;
  color: #FFFFFF;
  z-index: 9999;
}

.skip-link:focus {
  top: 0;
}
```

---

## Quick Reference: CSS Variables

```css
:root {
  /* Colors */
  --color-primary: #1B9B8C;
  --color-primary-hover: #178A7C;
  --color-error: #991B1B;
  --color-success: #22C55E;

  --bg-page: #FAFAF8;
  --bg-surface: #FFFFFF;
  --bg-input: #EEEEE8;

  --text-primary: #262626;
  --text-secondary: #525250;
  --text-muted: #737370;
  --text-placeholder: #A3A3A0;

  --border-default: #E5E5E0;
  --border-light: #EEEEE8;

  /* Typography */
  --font-primary: 'Inter', sans-serif;
  --font-display: 'Times New Roman', serif;
  --font-mono: 'SF Mono', monospace;

  /* Spacing */
  --space-1: 4px;
  --space-2: 8px;
  --space-3: 12px;
  --space-4: 16px;
  --space-6: 24px;
  --space-8: 32px;

  /* Borders */
  --radius-sm: 4px;
  --radius-md: 8px;
  --radius-lg: 12px;
  --radius-xl: 16px;
  --radius-pill: 9999px;

  /* Shadows */
  --shadow-sm: 0 1px 3px rgba(0, 0, 0, 0.08);
  --shadow-md: 0 4px 6px rgba(0, 0, 0, 0.07);
  --shadow-lg: 0 10px 15px rgba(0, 0, 0, 0.1);

  /* Animation */
  --duration-fast: 100ms;
  --duration-normal: 200ms;
  --duration-slow: 300ms;
  --ease-default: cubic-bezier(0.4, 0, 0.2, 1);
}
```
