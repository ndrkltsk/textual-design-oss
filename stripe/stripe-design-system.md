# Design System Documentation

## 1. Design & Brand Identity

### Design Philosophy
- **Clarity First**: Every element serves a purpose with maximum information density without overwhelming users
- **Professional Elegance**: Sophisticated, trustworthy aesthetic appropriate for financial services
- **Developer-Friendly**: Technical precision with clear documentation patterns
- **Subtle Depth**: Layered interfaces using shadows, borders, and background colors to create hierarchy

### Visual Style Direction
- **Modern Minimalist**: Clean lines, generous white space, restrained color palette
- **Data-Centric**: Optimized for displaying complex financial data, tables, and metrics
- **Gradient Accents**: Strategic use of colorful gradients for marketing pages while maintaining simplicity in dashboard interfaces
- **Geometric Patterns**: Abstract decorative shapes in brand purple/blue tones for visual interest on landing pages

### Overall Mood and Tone
- Professional and trustworthy
- Technical yet approachable
- Premium and sophisticated
- Focused and efficient

### Brand Personality Through UI
- **Precision**: Exact alignments, consistent spacing, mathematical proportions
- **Transparency**: Clear states, visible feedback, honest error messages
- **Innovation**: Modern patterns, smooth transitions, thoughtful interactions
- **Reliability**: Consistent patterns, predictable behaviors, stable foundations

### Visual Language Consistency
- Unified color application across all interfaces
- Consistent component styling from marketing to dashboard
- Coherent iconography and illustration style
- Harmonious typography scale throughout

---

## 2. Design Tokens

### Colors

#### Primary Palette
```css
--color-primary: #635BFF;          /* Main brand purple/indigo - buttons, links, focus states */
--color-primary-dark: #5851EB;     /* Hover state for primary */
--color-primary-darker: #4B45D1;   /* Active/pressed state */
--color-primary-light: #7A73FF;    /* Lighter variant */
--color-primary-lighter: #A5A1FF;  /* Even lighter variant */
--color-primary-bg: #F6F5FF;       /* Very light purple background */
```

#### Secondary/Accent Colors
```css
--color-cyan: #00D4FF;             /* Teal/cyan accent for gradients */
--color-cyan-dark: #0FBEF0;        /* Darker cyan */
--color-green-brand: #00D924;      /* Brand green for success, highlights */
--color-green-teal: #0ACF97;       /* Teal green variant */
--color-blue-link: #0074D4;        /* Link blue */
--color-blue-light: #5469D4;       /* Lighter blue */
```

#### Product-Specific Colors
```css
/* Connect - Teal */
--color-connect: #0FBEF0;
--color-connect-dark: #0AA4D1;

/* Radar/Fraud - Orange */
--color-radar: #F5A623;

/* Capital - Green */
--color-capital: #0ACF97;
--color-capital-dark: #09B384;

/* Issuing - Purple/Blue */
--color-issuing: #635BFF;

/* Climate - Green */
--color-climate: #00D924;

/* Treasury - Blue gradient */
--color-treasury-start: #635BFF;
--color-treasury-end: #0FBEF0;

/* Atlas - Orange */
--color-atlas: #E57B3A;
--color-atlas-dark: #D16A2D;

/* Identity - Purple */
--color-identity: #9B7DFF;
--color-identity-dark: #8A6AEF;

/* Sigma - Blue */
--color-sigma: #5469D4;
--color-sigma-dark: #4355B8;

/* Tax - Green */
--color-tax: #1AAB7F;
--color-tax-dark: #158F6A;

/* Revenue Recognition - Purple/Pink */
--color-revenue: #C26DBC;
--color-revenue-dark: #A85BA3;

/* Data Pipeline - Blue */
--color-data-pipeline: #067AB8;
--color-data-pipeline-dark: #05679B;

/* Financial Connections - Blue/Green */
--color-financial-connections: #11A397;
--color-financial-connections-dark: #0E897F;
```

#### Neutral/Grayscale
```css
--color-gray-50: #F7FAFC;          /* Lightest - page backgrounds */
--color-gray-100: #F6F9FC;         /* Light backgrounds */
--color-gray-150: #F1F5F9;         /* Card backgrounds, hover states */
--color-gray-200: #E3E8EE;         /* Borders, dividers */
--color-gray-300: #D8DEE4;         /* Stronger borders */
--color-gray-400: #C1C9D2;         /* Disabled states */
--color-gray-500: #8898AA;         /* Muted text, placeholders */
--color-gray-600: #697386;         /* Secondary text */
--color-gray-700: #545969;         /* Body text */
--color-gray-800: #3C4257;         /* Strong text */
--color-gray-900: #1A1F36;         /* Headings, primary text */
--color-gray-950: #121826;         /* Darkest */
```

#### Semantic Colors
```css
/* Success */
--color-success: #30B130;
--color-success-light: #D4EDDA;
--color-success-dark: #228B22;
--color-success-bg: #ECFDF5;
--color-success-text: #166534;

/* Warning */
--color-warning: #F5A623;
--color-warning-light: #FFF3CD;
--color-warning-dark: #E09800;
--color-warning-bg: #FFFBEB;
--color-warning-text: #B45309;

/* Error */
--color-error: #DF1B41;
--color-error-light: #FECDD3;
--color-error-dark: #BE123C;
--color-error-bg: #FEF2F2;
--color-error-text: #991B1B;

/* Info */
--color-info: #0074D4;
--color-info-light: #DBEAFE;
--color-info-dark: #005EB8;
--color-info-bg: #EFF6FF;
--color-info-text: #1E40AF;
```

#### Background Colors
```css
--bg-primary: #FFFFFF;             /* Main content areas */
--bg-secondary: #F6F9FC;           /* Page backgrounds */
--bg-tertiary: #F1F5F9;            /* Nested cards, sidebars */
--bg-elevated: #FFFFFF;            /* Modals, dropdowns */
--bg-overlay: rgba(0, 0, 0, 0.4);  /* Modal overlays */
--bg-overlay-light: rgba(0, 0, 0, 0.1);
--bg-dark: #1A1F36;                /* Dark sections */
--bg-dark-secondary: #121826;      /* Darker backgrounds */
```

#### Text Colors
```css
--text-primary: #1A1F36;           /* Headings, important text */
--text-secondary: #3C4257;         /* Body text */
--text-tertiary: #697386;          /* Secondary information */
--text-muted: #8898AA;             /* Captions, hints */
--text-disabled: #C1C9D2;          /* Disabled text */
--text-inverse: #FFFFFF;           /* Text on dark backgrounds */
--text-link: #635BFF;              /* Links */
--text-link-hover: #5851EB;        /* Link hover */
```

#### Border Colors
```css
--border-light: #E3E8EE;           /* Default borders */
--border-medium: #D8DEE4;          /* Stronger borders */
--border-dark: #C1C9D2;            /* Dark mode borders */
--border-focus: #635BFF;           /* Focus state borders */
--border-error: #DF1B41;           /* Error state borders */
--border-success: #30B130;         /* Success state borders */
```

#### Gradient Definitions
```css
/* Hero gradient - purple to cyan */
--gradient-hero: linear-gradient(135deg, #635BFF 0%, #0FBEF0 100%);

/* Dashboard card gradient */
--gradient-card: linear-gradient(180deg, #FFFFFF 0%, #F6F9FC 100%);

/* Purple gradient */
--gradient-purple: linear-gradient(135deg, #635BFF 0%, #7A73FF 100%);

/* Teal gradient */
--gradient-teal: linear-gradient(135deg, #0FBEF0 0%, #0ACF97 100%);

/* Dark gradient */
--gradient-dark: linear-gradient(180deg, #1A1F36 0%, #121826 100%);

/* Multicolor hero (marketing pages) */
--gradient-multicolor: linear-gradient(135deg, #80E9FF 0%, #A5B4FC 25%, #C084FC 50%, #F472B6 75%, #FB7185 100%);

/* Decorative background shapes */
--gradient-shape-purple: linear-gradient(135deg, rgba(99, 91, 255, 0.3) 0%, rgba(99, 91, 255, 0.1) 100%);
--gradient-shape-cyan: linear-gradient(135deg, rgba(15, 190, 240, 0.3) 0%, rgba(15, 190, 240, 0.1) 100%);
```

---

### Typography

#### Font Families
```css
--font-primary: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Ubuntu, sans-serif;
--font-heading: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Ubuntu, sans-serif;
--font-mono: 'SFMono-Regular', Consolas, 'Liberation Mono', Menlo, Courier, monospace;
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
/* Display/Hero sizes */
--text-display-2xl: 72px;          /* Hero headlines */
--text-display-xl: 60px;           /* Large hero text */
--text-display-lg: 48px;           /* Section heroes */
--text-display-md: 40px;           /* Page titles */

/* Heading sizes */
--text-h1: 32px;                   /* Page headings */
--text-h2: 24px;                   /* Section headings */
--text-h3: 20px;                   /* Subsection headings */
--text-h4: 18px;                   /* Card headings */
--text-h5: 16px;                   /* Small headings */
--text-h6: 14px;                   /* Tiny headings */

/* Body sizes */
--text-body-lg: 18px;              /* Large body text */
--text-body-md: 16px;              /* Default body */
--text-body-sm: 14px;              /* Small body, UI text */

/* Small sizes */
--text-caption: 13px;              /* Captions */
--text-small: 12px;                /* Small labels, metadata */
--text-tiny: 11px;                 /* Timestamps, badges */
```

#### Line Heights
```css
--leading-none: 1;
--leading-tight: 1.2;              /* Headings */
--leading-snug: 1.375;             /* Subheadings */
--leading-normal: 1.5;             /* Body text */
--leading-relaxed: 1.625;          /* Large body text */
--leading-loose: 1.75;             /* Comfortable reading */
```

#### Letter Spacing
```css
--tracking-tighter: -0.02em;       /* Large display text */
--tracking-tight: -0.01em;         /* Headings */
--tracking-normal: 0;              /* Body text */
--tracking-wide: 0.025em;          /* Small caps, labels */
--tracking-wider: 0.05em;          /* Uppercase labels */
--tracking-widest: 0.1em;          /* All-caps headings */
```

#### Paragraph Spacing
```css
--paragraph-spacing-sm: 12px;
--paragraph-spacing-md: 16px;
--paragraph-spacing-lg: 24px;
```

#### Text Style Catalog

**Display 2XL**
```css
font-size: 72px;
line-height: 1.1;
font-weight: 700;
letter-spacing: -0.02em;
```

**Display XL**
```css
font-size: 60px;
line-height: 1.1;
font-weight: 700;
letter-spacing: -0.02em;
```

**Display LG**
```css
font-size: 48px;
line-height: 1.15;
font-weight: 700;
letter-spacing: -0.01em;
```

**Heading 1**
```css
font-size: 32px;
line-height: 1.25;
font-weight: 600;
letter-spacing: -0.01em;
```

**Heading 2**
```css
font-size: 24px;
line-height: 1.33;
font-weight: 600;
letter-spacing: 0;
```

**Heading 3**
```css
font-size: 20px;
line-height: 1.4;
font-weight: 600;
letter-spacing: 0;
```

**Heading 4**
```css
font-size: 18px;
line-height: 1.44;
font-weight: 600;
letter-spacing: 0;
```

**Body Large**
```css
font-size: 18px;
line-height: 1.6;
font-weight: 400;
```

**Body Default**
```css
font-size: 16px;
line-height: 1.5;
font-weight: 400;
```

**Body Small**
```css
font-size: 14px;
line-height: 1.5;
font-weight: 400;
```

**Caption**
```css
font-size: 13px;
line-height: 1.4;
font-weight: 400;
color: var(--text-tertiary);
```

**Label**
```css
font-size: 14px;
line-height: 1.4;
font-weight: 500;
```

**Label Small**
```css
font-size: 12px;
line-height: 1.33;
font-weight: 500;
letter-spacing: 0.025em;
```

**Overline**
```css
font-size: 12px;
line-height: 1.33;
font-weight: 600;
letter-spacing: 0.1em;
text-transform: uppercase;
```

**Code**
```css
font-family: var(--font-mono);
font-size: 14px;
line-height: 1.5;
```

---

### Spacing

#### Base Unit
```css
--spacing-unit: 4px;
```

#### Spacing Scale
```css
--space-0: 0;
--space-1: 4px;                    /* Tight spacing */
--space-2: 8px;                    /* Default small */
--space-3: 12px;                   /* Medium-small */
--space-4: 16px;                   /* Default medium */
--space-5: 20px;                   /* Medium */
--space-6: 24px;                   /* Default large */
--space-8: 32px;                   /* Large */
--space-10: 40px;                  /* Extra large */
--space-12: 48px;                  /* Section spacing */
--space-16: 64px;                  /* Large sections */
--space-20: 80px;                  /* Hero spacing */
--space-24: 96px;                  /* Major sections */
--space-32: 128px;                 /* Page sections */
```

#### Component Internal Padding
```css
/* Buttons */
--button-padding-sm: 6px 12px;
--button-padding-md: 8px 16px;
--button-padding-lg: 12px 24px;

/* Inputs */
--input-padding-sm: 6px 10px;
--input-padding-md: 8px 12px;
--input-padding-lg: 12px 16px;

/* Cards */
--card-padding-sm: 12px;
--card-padding-md: 16px;
--card-padding-lg: 24px;

/* Modals */
--modal-padding: 24px;

/* Tables */
--table-cell-padding: 12px 16px;
--table-cell-padding-sm: 8px 12px;
```

#### Layout Margins and Gaps
```css
--gap-xs: 4px;
--gap-sm: 8px;
--gap-md: 16px;
--gap-lg: 24px;
--gap-xl: 32px;
--gap-2xl: 48px;

--margin-section: 64px;
--margin-page: 32px;
```

---

### Effects

#### Shadow Definitions
```css
/* Subtle - for slight elevation */
--shadow-xs: 0 1px 2px rgba(0, 0, 0, 0.05);

/* Small - default cards */
--shadow-sm: 0 1px 3px rgba(0, 0, 0, 0.08), 0 1px 2px rgba(0, 0, 0, 0.06);

/* Medium - elevated cards, dropdowns */
--shadow-md: 0 4px 6px -1px rgba(0, 0, 0, 0.08), 0 2px 4px -1px rgba(0, 0, 0, 0.04);

/* Large - modals, popovers */
--shadow-lg: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);

/* Extra large - major overlays */
--shadow-xl: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);

/* 2XL - floating elements */
--shadow-2xl: 0 25px 50px -12px rgba(0, 0, 0, 0.25);

/* Inner shadow */
--shadow-inner: inset 0 2px 4px 0 rgba(0, 0, 0, 0.06);

/* Card with border */
--shadow-card: 0 2px 5px rgba(0, 0, 0, 0.08), 0 0 0 1px rgba(0, 0, 0, 0.05);

/* Focus ring */
--shadow-focus: 0 0 0 3px rgba(99, 91, 255, 0.4);
--shadow-focus-error: 0 0 0 3px rgba(223, 27, 65, 0.4);
--shadow-focus-success: 0 0 0 3px rgba(48, 177, 48, 0.4);

/* Button shadow */
--shadow-button: 0 1px 3px rgba(0, 0, 0, 0.08);
--shadow-button-hover: 0 4px 6px rgba(0, 0, 0, 0.12);
```

#### Blur Effects
```css
--blur-sm: 4px;
--blur-md: 8px;
--blur-lg: 16px;
--blur-xl: 24px;

/* Backdrop blur for overlays */
--backdrop-blur: blur(8px);
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
--opacity-overlay: 0.4;
--opacity-hover: 0.8;
```

---

### Borders

#### Border Widths
```css
--border-width-0: 0;
--border-width-1: 1px;
--border-width-2: 2px;
--border-width-4: 4px;
```

#### Border Radius Scale
```css
--radius-none: 0;
--radius-sm: 4px;                  /* Small elements, inputs */
--radius-md: 6px;                  /* Buttons, cards */
--radius-lg: 8px;                  /* Larger cards */
--radius-xl: 12px;                 /* Modals, large cards */
--radius-2xl: 16px;                /* Hero cards */
--radius-3xl: 24px;                /* Large decorative */
--radius-full: 9999px;             /* Pills, avatars */
```

#### Border Styles
```css
--border-solid: solid;
--border-dashed: dashed;
--border-dotted: dotted;

/* Common border definitions */
--border-default: 1px solid var(--border-light);
--border-strong: 1px solid var(--border-medium);
--border-focus: 2px solid var(--color-primary);
--border-error: 1px solid var(--color-error);
```

---

### Iconography

#### Icon Style
- **Style**: Outlined (stroke-based icons)
- **Stroke Weight**: 1.5px - 2px
- **Line Caps**: Round
- **Corners**: Rounded

#### Icon Sizes
```css
--icon-xs: 12px;
--icon-sm: 16px;
--icon-md: 20px;
--icon-lg: 24px;
--icon-xl: 32px;
--icon-2xl: 40px;
--icon-3xl: 48px;
```

#### Icon Library
- Custom icon set with consistent 24x24 viewBox
- Similar to Heroicons (outline style)
- Monochrome, using currentColor

---

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
--duration-slow: 300ms;
--duration-slower: 400ms;
--duration-slowest: 500ms;
```

#### Transition Definitions
```css
/* Default transition */
--transition-all: all 200ms cubic-bezier(0.4, 0, 0.2, 1);
--transition-colors: color, background-color, border-color 150ms ease;
--transition-opacity: opacity 200ms ease;
--transition-transform: transform 200ms cubic-bezier(0.4, 0, 0.2, 1);
--transition-shadow: box-shadow 200ms ease;
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

/* Spinner rotation */
@keyframes spin {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}

/* Pulse */
@keyframes pulse {
  0%, 100% { opacity: 1; }
  50% { opacity: 0.5; }
}

/* Skeleton shimmer */
@keyframes shimmer {
  0% { background-position: -200% 0; }
  100% { background-position: 200% 0; }
}
```

---

## 3. Components

### Buttons

#### Primary Button
- **Purpose**: Main call-to-action
- **Dimensions**:
  - Small: height 32px, padding 6px 12px
  - Medium: height 36px, padding 8px 16px
  - Large: height 44px, padding 12px 24px
- **Styles**:
  ```css
  background: #635BFF;
  color: #FFFFFF;
  border: none;
  border-radius: 6px;
  font-weight: 500;
  font-size: 14px;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.08);
  ```
- **States**:
  - Default: `background: #635BFF`
  - Hover: `background: #5851EB; box-shadow: 0 4px 6px rgba(0,0,0,0.12)`
  - Active: `background: #4B45D1; transform: translateY(1px)`
  - Focus: `box-shadow: 0 0 0 3px rgba(99, 91, 255, 0.4)`
  - Disabled: `opacity: 0.5; cursor: not-allowed`
  - Loading: Show spinner, text "Processing..."

#### Secondary Button
- **Purpose**: Secondary actions
- **Styles**:
  ```css
  background: #FFFFFF;
  color: #3C4257;
  border: 1px solid #E3E8EE;
  border-radius: 6px;
  font-weight: 500;
  ```
- **States**:
  - Hover: `background: #F6F9FC; border-color: #D8DEE4`
  - Active: `background: #F1F5F9`
  - Focus: `box-shadow: 0 0 0 3px rgba(99, 91, 255, 0.4)`

#### Ghost Button
- **Purpose**: Tertiary actions, links
- **Styles**:
  ```css
  background: transparent;
  color: #635BFF;
  border: none;
  font-weight: 500;
  ```
- **States**:
  - Hover: `background: rgba(99, 91, 255, 0.08)`
  - Active: `background: rgba(99, 91, 255, 0.12)`

#### Outline Button
- **Purpose**: Secondary emphasis
- **Styles**:
  ```css
  background: transparent;
  color: #635BFF;
  border: 1px solid #635BFF;
  border-radius: 6px;
  ```

#### Icon Button
- **Purpose**: Icon-only actions
- **Dimensions**: 32px x 32px (sm), 36px x 36px (md), 44px x 44px (lg)
- **Styles**:
  ```css
  background: transparent;
  border: none;
  border-radius: 6px;
  padding: 8px;
  color: #697386;
  ```
- **States**:
  - Hover: `background: #F6F9FC; color: #3C4257`

#### Button with Icon
- **Spacing**: 8px gap between icon and text
- **Icon size**: 16px (sm), 20px (md)

#### Destructive Button
- **Styles**:
  ```css
  background: #DF1B41;
  color: #FFFFFF;
  ```
- **Hover**: `background: #BE123C`

---

### Inputs

#### Text Input
- **Dimensions**:
  - Height: 40px (default), 36px (small), 44px (large)
  - Padding: 8px 12px
- **Styles**:
  ```css
  background: #FFFFFF;
  border: 1px solid #E3E8EE;
  border-radius: 6px;
  font-size: 14px;
  color: #1A1F36;
  ```
- **States**:
  - Placeholder: `color: #8898AA`
  - Hover: `border-color: #D8DEE4`
  - Focus: `border-color: #635BFF; box-shadow: 0 0 0 3px rgba(99, 91, 255, 0.4)`
  - Error: `border-color: #DF1B41; box-shadow: 0 0 0 3px rgba(223, 27, 65, 0.2)`
  - Disabled: `background: #F6F9FC; color: #8898AA; cursor: not-allowed`
- **With prefix**: Left icon/symbol with padding-left: 36px
- **With suffix**: Right icon/button with padding-right: 36px

#### Textarea
- **Min height**: 80px
- **Resize**: vertical
- **Same border/focus styles as text input

#### Select
- **Appearance**: Custom dropdown arrow (chevron)
- **Styles**: Same as text input
- **Arrow**: 16px chevron-down icon, color #697386

#### Checkbox
- **Dimensions**: 16px x 16px
- **Styles**:
  ```css
  border: 1px solid #D8DEE4;
  border-radius: 4px;
  background: #FFFFFF;
  ```
- **States**:
  - Checked: `background: #635BFF; border-color: #635BFF`
  - Checkmark: White, 2px stroke
  - Indeterminate: Horizontal line instead of checkmark
  - Disabled: `opacity: 0.5`

#### Radio Button
- **Dimensions**: 16px diameter
- **Styles**:
  ```css
  border: 1px solid #D8DEE4;
  border-radius: 50%;
  background: #FFFFFF;
  ```
- **States**:
  - Selected: `border-color: #635BFF; border-width: 5px`
  - Inner dot: 6px, #635BFF

#### Toggle/Switch
- **Dimensions**: 36px x 20px
- **Styles**:
  ```css
  background: #D8DEE4;
  border-radius: 10px;
  ```
- **States**:
  - On: `background: #635BFF`
  - Thumb: 16px circle, white, positioned left (off) or right (on)
  - Transition: 200ms ease

#### Range Slider
- **Track height**: 4px
- **Track color**: #E3E8EE (unfilled), #635BFF (filled)
- **Thumb**: 16px circle, white, border: 2px solid #635BFF
- **Border radius**: 2px (track)

#### Currency Input
- **Structure**: $ prefix + input + currency dropdown
- **Prefix**: Gray background (#F6F9FC), border-right

#### Date Input
- **Format indicator**: MM/DD/YYYY placeholder
- **Calendar icon**: Right side

#### Phone Input with Country Code
- **Structure**: Country selector (flag + code) + phone input
- **Country selector**: Dropdown with flag icons, 80px width
- **Phone input**: Remaining width
- **Border**: Shared container, internal divider

#### Percentage Input
- **Structure**: Number input + % suffix
- **Suffix**: Gray background (#F6F9FC), right-aligned
- **Validation**: 0-100 range

#### OTP/Verification Code Input
- **Structure**: 6 individual input boxes
- **Box dimensions**: 48px x 56px
- **Styles**:
  ```css
  border: 1px solid #E3E8EE;
  border-radius: 6px;
  font-size: 24px;
  font-weight: 600;
  text-align: center;
  ```
- **Gap**: 8px between boxes
- **Focus**: Auto-advance to next box on input
- **Paste**: Distribute pasted code across boxes

#### Color Picker
- **Structure**: Color swatch + hex input
- **Swatch dimensions**: 40px x 40px
- **Hex input**: With # prefix
- **Border radius**: 6px

#### File Upload
- **Button style**:
  ```css
  background: transparent;
  border: 1px solid #E3E8EE;
  border-radius: 6px;
  padding: 8px 16px;
  color: #635BFF;
  ```
- **Icon**: Upload arrow, 16px
- **Drag area**: Dashed border when applicable

---

### Cards

#### Default Card
- **Styles**:
  ```css
  background: #FFFFFF;
  border: 1px solid #E3E8EE;
  border-radius: 8px;
  padding: 16px;
  ```

#### Elevated Card
- **Styles**:
  ```css
  background: #FFFFFF;
  border-radius: 8px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.08), 0 0 0 1px rgba(0, 0, 0, 0.05);
  padding: 16px;
  ```

#### Interactive Card
- **Hover state**:
  ```css
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  transform: translateY(-2px);
  cursor: pointer;
  ```

#### Feature Card (Marketing)
- **Styles**:
  ```css
  background: linear-gradient(180deg, #FFFFFF 0%, #F6F9FC 100%);
  border-radius: 12px;
  padding: 24px;
  ```

#### Pricing Card
- **Highlighted variant**:
  ```css
  border: 2px solid #635BFF;
  ```
- **Badge**: "Most popular" positioned top-right

#### Radio Card (Selectable Card)
- **Purpose**: Large selection options with descriptions
- **Dimensions**: Variable width, min-height 80px
- **Styles**:
  ```css
  background: #FFFFFF;
  border: 1px solid #E3E8EE;
  border-radius: 8px;
  padding: 16px;
  cursor: pointer;
  ```
- **States**:
  - Hover: `border-color: #D8DEE4; background: #F6F9FC`
  - Selected: `border-color: #635BFF; border-width: 2px; background: #F6F5FF`
- **Radio indicator**: Top-left or top-right corner
- **Content**: Title, description, optional badge

#### Selection Card with Icon
- **Structure**: Icon/image + title + description + radio
- **Icon area**: 48px, left-aligned or top
- **Used for**: Payment method selection, plan selection

---

### Modals/Dialogs

#### Modal Container
- **Max-width**: 480px (small), 560px (default), 720px (large), 960px (extra-large)
- **Styles**:
  ```css
  background: #FFFFFF;
  border-radius: 12px;
  box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.25);
  max-height: 90vh;
  overflow: hidden;
  ```

#### Modal Overlay
- **Styles**:
  ```css
  background: rgba(0, 0, 0, 0.4);
  backdrop-filter: blur(4px);
  ```

#### Modal Header
- **Styles**:
  ```css
  padding: 24px 24px 0;
  border-bottom: none;
  ```
- **Title**: font-size 18px, font-weight 600
- **Close button**: Top-right, 32px, icon-only

#### Modal Body
- **Styles**:
  ```css
  padding: 16px 24px;
  overflow-y: auto;
  ```

#### Modal Footer
- **Styles**:
  ```css
  padding: 16px 24px 24px;
  display: flex;
  justify-content: flex-end;
  gap: 12px;
  ```

#### Slide-out Panel (Drawer)
- **Width**: 480px (default), 600px (wide)
- **Position**: Right edge
- **Animation**: Slide in from right, 300ms
- **Overlay**: Same as modal

---

### Dropdowns/Menus

#### Dropdown Menu
- **Styles**:
  ```css
  background: #FFFFFF;
  border: 1px solid #E3E8EE;
  border-radius: 8px;
  box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
  min-width: 180px;
  padding: 4px 0;
  ```

#### Menu Item
- **Styles**:
  ```css
  padding: 8px 16px;
  font-size: 14px;
  color: #3C4257;
  ```
- **Hover**: `background: #F6F9FC`
- **Active**: `background: #F1F5F9; color: #635BFF`
- **With icon**: 8px gap, icon 16px

#### Menu Divider
- **Styles**:
  ```css
  height: 1px;
  background: #E3E8EE;
  margin: 4px 0;
  ```

#### Menu Section Header
- **Styles**:
  ```css
  padding: 8px 16px 4px;
  font-size: 11px;
  font-weight: 600;
  color: #8898AA;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  ```

#### Actions Dropdown (Grouped)
- **Purpose**: Context actions grouped by category
- **Structure**: Button trigger → Dropdown with sections
- **Section headers**: Uppercase, muted color, 11px
- **Example sections**: "PAYMENTS", "RADAR", "ACCOUNT"
- **Keyboard shortcuts**: Right-aligned, muted text

---

### Navigation

#### Top Navigation Bar
- **Dimensions**: Height 64px
- **Styles**:
  ```css
  background: #FFFFFF;
  border-bottom: 1px solid #E3E8EE;
  position: sticky;
  top: 0;
  z-index: 100;
  ```

#### Nav Link
- **Styles**:
  ```css
  font-size: 14px;
  font-weight: 500;
  color: #3C4257;
  padding: 8px 12px;
  ```
- **Hover**: `color: #1A1F36`
- **Active**: `color: #635BFF`

#### Sidebar Navigation
- **Width**: 240px (expanded), 64px (collapsed)
- **Background**: #FFFFFF or #F6F9FC
- **Section header**:
  ```css
  font-size: 11px;
  font-weight: 600;
  color: #8898AA;
  text-transform: uppercase;
  padding: 16px 16px 8px;
  ```

#### Sidebar Item
- **Styles**:
  ```css
  padding: 8px 16px;
  font-size: 14px;
  color: #3C4257;
  border-radius: 6px;
  margin: 2px 8px;
  ```
- **Hover**: `background: #F6F9FC`
- **Active**:
  ```css
  background: #F6F5FF;
  color: #635BFF;
  border-left: 3px solid #635BFF;
  ```

#### Tabs (Underline)
- **Styles**:
  ```css
  font-size: 14px;
  font-weight: 500;
  color: #697386;
  padding: 12px 0;
  border-bottom: 2px solid transparent;
  ```
- **Active**: `color: #635BFF; border-color: #635BFF`
- **Hover**: `color: #3C4257`
- **Gap between tabs**: 24px

#### Tabs (Pill)
- **Styles**:
  ```css
  font-size: 14px;
  font-weight: 500;
  color: #697386;
  padding: 6px 12px;
  border-radius: 6px;
  background: transparent;
  ```
- **Active**: `background: #F6F5FF; color: #635BFF`

#### Breadcrumbs
- **Styles**:
  ```css
  font-size: 14px;
  color: #697386;
  ```
- **Separator**: Chevron-right icon, 12px, color #C1C9D2
- **Current page**: `color: #3C4257`
- **Links**: `color: #635BFF` on hover

---

### Tables

#### Table Container
- **Styles**:
  ```css
  background: #FFFFFF;
  border: 1px solid #E3E8EE;
  border-radius: 8px;
  overflow: hidden;
  ```

#### Table Header
- **Styles**:
  ```css
  background: #F6F9FC;
  border-bottom: 1px solid #E3E8EE;
  ```

#### Table Header Cell
- **Styles**:
  ```css
  padding: 12px 16px;
  font-size: 12px;
  font-weight: 600;
  color: #697386;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  text-align: left;
  ```
- **Sortable**: Cursor pointer, sort icon on right
- **Sorted**: `color: #3C4257`

#### Table Row
- **Styles**:
  ```css
  border-bottom: 1px solid #E3E8EE;
  ```
- **Hover**: `background: #F6F9FC`
- **Selected**: `background: #F6F5FF`

#### Table Cell
- **Styles**:
  ```css
  padding: 12px 16px;
  font-size: 14px;
  color: #3C4257;
  vertical-align: middle;
  ```

#### Table Actions Cell
- **Alignment**: Right
- **Actions**: Icon buttons, 32px

#### Expandable Table Row
- **Trigger**: Chevron icon or row click
- **Expanded content**: Nested below row, indented
- **Styles**:
  ```css
  background: #F6F9FC;
  padding: 16px 16px 16px 48px;
  border-bottom: 1px solid #E3E8EE;
  ```
- **Animation**: Height transition, 200ms
- **Nested content**: Key-value pairs, additional details

#### Table with Inline Filters
- **Filter chips**: Above table, removable
- **Filter dropdown**: Multi-select with checkboxes
- **Clear all**: Text button to remove all filters

---

### Lists

#### List Item
- **Styles**:
  ```css
  padding: 12px 16px;
  border-bottom: 1px solid #E3E8EE;
  ```
- **Hover**: `background: #F6F9FC`

#### Description List
- **Term**: font-weight 500, color #697386, font-size 13px
- **Description**: color #3C4257, font-size 14px

---

### Badges/Tags/Chips

#### Badge (Status)
- **Dimensions**: Height 20px, padding 2px 8px
- **Styles**:
  ```css
  border-radius: 10px;
  font-size: 12px;
  font-weight: 500;
  ```
- **Variants**:
  - Default: `background: #F1F5F9; color: #697386`
  - Success/Paid/Active: `background: #ECFDF5; color: #166534`
  - Warning/Pending: `background: #FFFBEB; color: #B45309`
  - Error/Failed: `background: #FEF2F2; color: #991B1B`
  - Info/Open: `background: #EFF6FF; color: #1E40AF`
  - Purple/Primary: `background: #F6F5FF; color: #635BFF`
  - In Progress: `background: #FEF3C7; color: #D97706`
  - Incomplete: `background: #F1F5F9; color: #697386` with info icon
  - Test Mode: `background: #FFF3CD; color: #B45309`
  - Default (payment): `background: #ECFDF5; color: #166534`

#### Category Badge
- **Purpose**: Categorize items (Team, API, Checkout)
- **Styles**:
  ```css
  background: #F1F5F9;
  color: #697386;
  padding: 2px 8px;
  border-radius: 4px;
  font-size: 11px;
  font-weight: 500;
  ```

#### Tag
- **Dimensions**: Height 24px, padding 4px 8px
- **Styles**:
  ```css
  background: #F6F9FC;
  border: 1px solid #E3E8EE;
  border-radius: 4px;
  font-size: 12px;
  color: #3C4257;
  ```
- **With remove**: X icon, 12px, right side

#### Filter Chip
- **Dimensions**: Height 32px, padding 6px 12px
- **Styles**:
  ```css
  background: #FFFFFF;
  border: 1px solid #E3E8EE;
  border-radius: 16px;
  font-size: 13px;
  ```
- **Selected**: `background: #F6F5FF; border-color: #635BFF; color: #635BFF`

---

### Avatars

#### Avatar Sizes
```css
--avatar-xs: 24px;
--avatar-sm: 32px;
--avatar-md: 40px;
--avatar-lg: 48px;
--avatar-xl: 64px;
--avatar-2xl: 96px;
```

#### Avatar Styles
- **Image**:
  ```css
  border-radius: 50%;
  object-fit: cover;
  ```
- **Initials fallback**:
  ```css
  background: #635BFF;
  color: #FFFFFF;
  font-weight: 600;
  display: flex;
  align-items: center;
  justify-content: center;
  ```
- **With status dot**: 8px circle, positioned bottom-right
  - Online: #30B130
  - Away: #F5A623
  - Busy: #DF1B41
  - Offline: #C1C9D2

#### Avatar Group
- **Overlap**: -8px margin
- **Border**: 2px solid white
- **"+N" indicator**: Gray background, font-size 12px

---

### Tooltips

#### Tooltip
- **Styles**:
  ```css
  background: #1A1F36;
  color: #FFFFFF;
  padding: 6px 10px;
  border-radius: 4px;
  font-size: 12px;
  max-width: 200px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  ```
- **Arrow**: 6px, same background color

---

### Alerts/Banners

#### Alert
- **Styles**:
  ```css
  padding: 12px 16px;
  border-radius: 6px;
  font-size: 14px;
  display: flex;
  gap: 12px;
  ```
- **Variants**:
  - Info: `background: #EFF6FF; border-left: 4px solid #0074D4; color: #1E40AF`
  - Success: `background: #ECFDF5; border-left: 4px solid #30B130; color: #166534`
  - Warning: `background: #FFFBEB; border-left: 4px solid #F5A623; color: #B45309`
  - Error: `background: #FEF2F2; border-left: 4px solid #DF1B41; color: #991B1B`

#### Banner (Full-width)
- **Styles**:
  ```css
  padding: 12px 24px;
  font-size: 14px;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  ```
- **Test mode banner**: `background: #FFF3CD; color: #B45309`
- **With close button**: Right-aligned X icon

---

### Progress Indicators

#### Progress Bar
- **Dimensions**: Height 4px (default), 8px (thick)
- **Styles**:
  ```css
  background: #E3E8EE;
  border-radius: 2px;
  ```
- **Fill**: `background: #635BFF; border-radius: 2px`

#### Spinner
- **Sizes**: 16px (sm), 20px (md), 24px (lg), 32px (xl)
- **Styles**:
  ```css
  border: 2px solid #E3E8EE;
  border-top-color: #635BFF;
  border-radius: 50%;
  animation: spin 600ms linear infinite;
  ```

#### Skeleton
- **Styles**:
  ```css
  background: linear-gradient(90deg, #F1F5F9 25%, #E3E8EE 50%, #F1F5F9 75%);
  background-size: 200% 100%;
  animation: shimmer 1.5s ease infinite;
  border-radius: 4px;
  ```

#### Step Indicator
- **Circle dimensions**: 24px (default), 32px (large)
- **Styles**:
  - Pending: `border: 2px solid #D8DEE4; background: #FFFFFF; color: #697386`
  - Active: `border: 2px solid #635BFF; background: #635BFF; color: #FFFFFF`
  - Completed: `background: #635BFF; color: #FFFFFF` with checkmark
- **Connector line**: `height: 2px; background: #E3E8EE` (completed: #635BFF)

---

### Pagination

#### Pagination
- **Button dimensions**: 32px height, min-width 32px
- **Styles**:
  ```css
  border: 1px solid #E3E8EE;
  border-radius: 6px;
  background: #FFFFFF;
  font-size: 14px;
  color: #3C4257;
  ```
- **Active**: `background: #635BFF; color: #FFFFFF; border-color: #635BFF`
- **Disabled**: `opacity: 0.5; cursor: not-allowed`

---

### Accordions

#### Accordion
- **Header**:
  ```css
  padding: 16px;
  font-size: 14px;
  font-weight: 500;
  color: #3C4257;
  cursor: pointer;
  border-bottom: 1px solid #E3E8EE;
  ```
- **Chevron**: Rotates 180deg when expanded
- **Content**:
  ```css
  padding: 16px;
  font-size: 14px;
  color: #697386;
  ```

---

### Code Block

#### Code Block
- **Styles**:
  ```css
  background: #1A1F36;
  border-radius: 8px;
  padding: 16px;
  font-family: var(--font-mono);
  font-size: 13px;
  color: #E3E8EE;
  overflow-x: auto;
  ```
- **Syntax highlighting**:
  - Keywords: #C792EA
  - Strings: #C3E88D
  - Numbers: #F78C6C
  - Comments: #697386
  - Functions: #82AAFF

#### Inline Code
- **Styles**:
  ```css
  background: #F6F9FC;
  padding: 2px 6px;
  border-radius: 4px;
  font-family: var(--font-mono);
  font-size: 13px;
  color: #DF1B41;
  ```

---

### Form Elements

#### Form Group
- **Spacing**: 16px between groups

#### Label
- **Styles**:
  ```css
  font-size: 14px;
  font-weight: 500;
  color: #3C4257;
  margin-bottom: 6px;
  display: block;
  ```

#### Required Indicator
- **Styles**: `color: #DF1B41` asterisk after label

#### Helper Text
- **Styles**:
  ```css
  font-size: 13px;
  color: #697386;
  margin-top: 4px;
  ```

#### Error Message
- **Styles**:
  ```css
  font-size: 13px;
  color: #DF1B41;
  margin-top: 4px;
  ```
- **With icon**: 14px warning icon

---

### Empty States

#### Empty State
- **Structure**: Icon (48-64px), title, description, action button
- **Container**:
  ```css
  text-align: center;
  padding: 48px 24px;
  ```
- **Icon**: Muted color (#C1C9D2)
- **Title**: font-size 16px, font-weight 600
- **Description**: font-size 14px, color #697386, max-width 300px

---

### Toast/Notifications

#### Toast
- **Dimensions**: Min-width 300px, max-width 420px
- **Styles**:
  ```css
  background: #FFFFFF;
  border-radius: 8px;
  box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
  padding: 16px;
  display: flex;
  gap: 12px;
  ```
- **Icon**: 20px, colored by type
- **Close button**: Top-right, 16px

---

### Data Display

#### Stat Card
- **Structure**: Label, value, trend
- **Label**: font-size 13px, color #697386
- **Value**: font-size 32px, font-weight 600, color #1A1F36
- **Trend**: font-size 13px, with arrow icon
  - Up: color #30B130
  - Down: color #DF1B41

#### Key-Value Pair
- **Styles**:
  ```css
  display: flex;
  justify-content: space-between;
  padding: 8px 0;
  border-bottom: 1px solid #E3E8EE;
  ```
- **Key**: color #697386
- **Value**: color #3C4257, font-weight 500

---

### Charts

#### Chart Colors
```css
--chart-primary: #635BFF;
--chart-secondary: #0FBEF0;
--chart-tertiary: #30B130;
--chart-quaternary: #F5A623;
--chart-quinary: #F74E8C;
--chart-gray: #8898AA;
```

#### Axis Styles
- **Labels**: font-size 11px, color #8898AA
- **Lines**: stroke #E3E8EE, stroke-width 1px
- **Grid**: stroke #F1F5F9, stroke-dasharray 4

#### Bar Chart
- **Bar radius**: 4px (top corners)
- **Gap**: 8px between bars

#### Line Chart
- **Line width**: 2px
- **Data point**: 6px circle
- **Area fill**: 10% opacity of line color

#### Donut/Pie Chart
- **Purpose**: Show proportional data (ownership splits, distribution)
- **Dimensions**: 120-200px diameter
- **Styles**:
  ```css
  stroke-width: 24px;
  fill: transparent;
  ```
- **Center label**: Total or key metric
- **Legend**: Right side, colored dots + labels
- **Colors**: Use chart color palette

#### Area Chart
- **Fill opacity**: 0.1
- **Line**: 2px stroke on top
- **Gradient**: Top to bottom fade

---

### Specialized Components

#### QR Code Display
- **Purpose**: Share links, payment codes
- **Container**:
  ```css
  background: #FFFFFF;
  padding: 24px;
  border-radius: 12px;
  text-align: center;
  ```
- **QR size**: 160-200px
- **Actions below**: Copy link, Download image buttons

#### Risk/Threshold Slider
- **Purpose**: Adjust sensitivity (fraud protection, etc.)
- **Structure**: Slider with labeled endpoints
- **Labels**: "Block more fraud" ↔ "Allow more payments"
- **Track**: Gradient from red to green
- **Indicator**: Current position marker

#### Pricing Tier Slider
- **Purpose**: Select plan tiers
- **Structure**: Horizontal steps with labels
- **Step markers**: Circles on track
- **Active step**: Elevated card showing details
- **Labels below**: Tier names and user counts

#### Map Embed
- **Purpose**: Show location data (audit logs, user activity)
- **Provider**: Mapbox style
- **Styles**:
  ```css
  border-radius: 8px;
  overflow: hidden;
  ```
- **Markers**: Custom pins for locations
- **Attribution**: Bottom corner

#### Payment Method Display
- **Structure**: Icon + name + details + badge
- **Icons**: Card brands (Visa, Mastercard, Amex), bank icon
- **Badge**: "Default" for primary method
- **Expandable**: Chevron to show more details

#### API ID Display
- **Purpose**: Show copyable API identifiers
- **Styles**:
  ```css
  font-family: var(--font-mono);
  font-size: 13px;
  background: #F6F9FC;
  padding: 4px 8px;
  border-radius: 4px;
  color: #697386;
  ```
- **Copy button**: Icon button on right
- **Truncation**: Ellipsis for long IDs

---

## 4. Layout System

### Grid System
- **Columns**: 12-column grid
- **Gutter**: 24px
- **Margin**: 24px (mobile), 32px (tablet), 64px (desktop)

### Container Max-widths
```css
--container-sm: 640px;
--container-md: 768px;
--container-lg: 1024px;
--container-xl: 1280px;
--container-2xl: 1440px;
--container-full: 100%;
```

### Breakpoints
```css
--breakpoint-sm: 640px;
--breakpoint-md: 768px;
--breakpoint-lg: 1024px;
--breakpoint-xl: 1280px;
--breakpoint-2xl: 1536px;
```

### Responsive Behavior
- **Mobile (< 640px)**: Single column, stacked navigation
- **Tablet (640-1024px)**: 2-column where appropriate, hamburger menu
- **Desktop (> 1024px)**: Full multi-column layouts, expanded navigation

### Page Structure Templates

#### Marketing Page
```
+----------------------------------+
|           Top Nav (64px)         |
+----------------------------------+
|                                  |
|         Hero Section             |
|          (80-120px py)           |
|                                  |
+----------------------------------+
|                                  |
|      Feature Sections            |
|          (64px py each)          |
|                                  |
+----------------------------------+
|         Footer (py 64px)         |
+----------------------------------+
```

#### Dashboard Page
```
+----------------------------------+
|           Top Nav (64px)         |
+--------+-------------------------+
|        |                         |
|Sidebar |     Content Area        |
|(240px) |      (px: 32px)         |
|        |                         |
|        |                         |
+--------+-------------------------+
```

#### Form Page
```
+----------------------------------+
|    Header with close (64px)      |
+----------------------------------+
| Step    |                        |
| Sidebar |    Form Content        |
| (200px) |    (max-width 600px)   |
|         |                        |
+---------+------------------------+
```

### Content Width Constraints
- **Form content**: max-width 600px
- **Article content**: max-width 720px
- **Table content**: max-width 1200px (with horizontal scroll beyond)

### Vertical Rhythm
- **Section spacing**: 64px
- **Component spacing**: 24px
- **Element spacing**: 16px
- **Tight spacing**: 8px

---

## 5. Patterns

### Navigation Patterns

#### Header Behavior
- **Position**: Sticky, top: 0
- **Shadow on scroll**: Applied when scrolled past threshold
- **Mobile**: Hamburger menu trigger on right

#### Mobile Navigation
- **Trigger**: Hamburger icon (24px)
- **Menu**: Full-screen overlay or slide-in drawer
- **Animation**: 300ms slide from right

#### Sidebar Patterns
- **Collapsible sections**: Chevron rotates on expand
- **Active indicator**: Purple left border
- **Nested items**: Indented 16px with dot indicator

#### Tab Navigation
- **Underline style**: 2px bottom border on active
- **Pill style**: Background change on active
- **Scroll behavior**: Horizontal scroll with fade indicators

#### Link Styles
- **Default**: color #635BFF
- **Hover**: color #5851EB, text-decoration underline
- **Visited**: Same as default (no change)

### Form Patterns

#### Form Layout
- **Label position**: Above input
- **Label alignment**: Left
- **Field grouping**: Cards or bordered sections

#### Validation Display
- **Inline errors**: Below input, red text with icon
- **Error summary**: Top of form, alert style
- **Real-time validation**: On blur

#### Required Field Indication
- Asterisk (*) after label in red

#### Helper Text
- Below input, muted color
- Appears before error message

#### Input Groups
- **With prefix**: Currency symbol, country code
- **With suffix**: Dropdown, icon button
- **Combined inputs**: Border between, shared container

### Content Patterns

#### Card Layouts
- **Grid**: 3-4 columns on desktop, responsive
- **Masonry**: Variable height cards
- **List**: Full-width, stacked

#### List Layouts
- **Simple list**: Icon + content
- **Complex list**: Multi-line with metadata
- **Action list**: With buttons on right

#### Empty States
- **Centered**: Icon, title, description, CTA
- **Full-width**: Background pattern optional

#### Loading States
- **Skeleton**: Matches content structure
- **Spinner**: Centered in container
- **Progressive**: Partial content with loading areas

#### Error States
- **Inline**: Below field
- **Page-level**: Error page with illustration
- **Toast**: Temporary notification

### Feedback Patterns

#### Toast Positioning
- **Position**: Top-right
- **Offset**: 24px from edges
- **Stack**: New toasts push old ones down

#### Modal Overlay
- **Background**: rgba(0, 0, 0, 0.4)
- **Blur**: 4px backdrop-filter
- **Animation**: Fade in 200ms

#### Confirmation Dialogs
- **Structure**: Icon, title, description, actions
- **Destructive**: Red primary button

#### Inline Feedback
- **Success**: Green checkmark + message
- **Error**: Red X + message
- **Loading**: Spinner + "Processing..."

---

## 6. Page Templates

### Marketing Homepage
- **Hero**: Full-width, gradient background, centered content
- **Features**: 3-column grid, icon cards
- **Testimonials**: Quote cards, company logos
- **CTA Section**: Centered, prominent button
- **Footer**: 4-column links, bottom bar

### Product Page
- **Subnav**: Product-specific tabs
- **Hero**: Split layout (text left, visual right)
- **Feature sections**: Alternating layout
- **Pricing preview**: Card highlights

### Dashboard Home
- **Header**: Page title, primary action button
- **Metrics row**: 3-4 stat cards
- **Main content**: Tables, charts, activity

### Settings Page
- **Sidebar**: Settings categories
- **Content**: Form sections, save at bottom
- **Width**: Constrained (max-width 720px)

### Documentation Page
- **Sidebar**: Collapsible navigation tree
- **Content**: Article format, code blocks
- **TOC**: Right sidebar on desktop

### Authentication Pages
- **Layout**: Centered card, decorative background
- **Card**: max-width 400px, shadow
- **Form**: Email, password, remember me, forgot link
- **Decorative shapes**: Diagonal stripes in brand colors (purple, cyan)

### Multi-Step Wizard Page
- **Layout**: Full-screen with header, sidebar, content, help panel
- **Header**: Title + progress badge ("In progress"), close button
- **Sidebar** (200px):
  - Numbered steps with sub-items
  - Active step: Purple number, bold text
  - Completed step: Checkmark icon
  - Sub-items: Indented with dot indicators
- **Content area**: Centered form, max-width 600px
- **Help panel** (right, 280px):
  - Context-sensitive guidance
  - Light background (#F6F9FC)
  - Helpful links
- **Footer**: Back button (secondary), Continue button (primary)

### Customer Detail Page
- **Layout**: Header with actions, collapsible sections
- **Sections**: Insights, Details, Metadata (collapsible)
- **Actions dropdown**: Grouped by category
- **Related data**: Tabs for Overview, Events and logs
- **Tables**: Payments, Invoices with status badges

### Audit Log Page
- **Layout**: Table with expandable rows
- **Columns**: Action, Category, Device ID, IP Address, Time
- **Expandable details**: User, Device, IP, Browser, OS, etc.
- **Embedded map**: Shows location of activity
- **Filters**: By category, date range, user

### Invoice Editor Page
- **Layout**: Split view (form left, preview right)
- **Form sections**: Customer, items, payment methods
- **Preview tabs**: Email, Invoice PDF, Payment page
- **Payment method cards**: Selectable with icons
- **Collapsible**: Advanced options accordion

---

## 7. Imagery & Media

### Image Aspect Ratios
- **Hero images**: 16:9 or 2:1
- **Card thumbnails**: 16:9 or 4:3
- **Avatar**: 1:1 (square/circle)
- **Icons**: 1:1

### Image Border Treatments
- **Card images**: border-radius matching card (8px)
- **Standalone**: border-radius 8px
- **Screenshots**: Border + shadow, 8px radius

### Placeholder/Fallback
- **Loading**: Skeleton with shimmer
- **Error**: Gray background with icon
- **Avatar fallback**: Initials on colored background

### Video Player
- **Container**: 16:9 aspect ratio
- **Controls**: Bottom, translucent background
- **Play button overlay**: Centered, 64px circle

### Avatar Fallbacks
- **With image**: Display image
- **Without image**: Show initials on gradient
- **Gradient colors**: Based on name hash

---

## 8. Accessibility

### Color Contrast Ratios
- **Normal text**: Minimum 4.5:1
- **Large text (18px+)**: Minimum 3:1
- **Interactive elements**: Minimum 3:1
- **Decorative elements**: No requirement

### Focus Indicator Styles
- **Default**: 3px purple outline with offset
- **High contrast**: Solid 2px outline
- **Skip to main**: Visible on focus only

### Touch Target Sizes
- **Minimum**: 44px x 44px
- **Recommended**: 48px x 48px
- **Spacing between targets**: Minimum 8px

### Screen Reader Considerations
- **Skip links**: "Skip to main content"
- **Landmarks**: header, nav, main, footer
- **ARIA labels**: On icon-only buttons
- **Live regions**: For dynamic content updates
- **Focus management**: On modal open/close

---

## Appendix: CSS Custom Properties Summary

```css
:root {
  /* Colors */
  --color-primary: #635BFF;
  --color-primary-dark: #5851EB;
  --color-success: #30B130;
  --color-warning: #F5A623;
  --color-error: #DF1B41;
  --color-info: #0074D4;

  /* Neutrals */
  --color-gray-50: #F7FAFC;
  --color-gray-100: #F6F9FC;
  --color-gray-200: #E3E8EE;
  --color-gray-500: #8898AA;
  --color-gray-600: #697386;
  --color-gray-900: #1A1F36;

  /* Typography */
  --font-primary: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
  --font-mono: 'SFMono-Regular', Consolas, monospace;

  /* Spacing */
  --space-1: 4px;
  --space-2: 8px;
  --space-3: 12px;
  --space-4: 16px;
  --space-6: 24px;
  --space-8: 32px;

  /* Borders */
  --radius-sm: 4px;
  --radius-md: 6px;
  --radius-lg: 8px;
  --radius-xl: 12px;
  --radius-full: 9999px;

  /* Shadows */
  --shadow-sm: 0 1px 3px rgba(0, 0, 0, 0.08);
  --shadow-md: 0 4px 6px rgba(0, 0, 0, 0.08);
  --shadow-lg: 0 10px 15px rgba(0, 0, 0, 0.1);
  --shadow-focus: 0 0 0 3px rgba(99, 91, 255, 0.4);

  /* Transitions */
  --transition-fast: 150ms ease;
  --transition-normal: 200ms ease;
  --transition-slow: 300ms ease;
}
```
