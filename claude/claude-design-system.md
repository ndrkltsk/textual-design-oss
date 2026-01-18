# Design System Documentation

## 1. Design & Brand Identity

### Design Philosophy and Guiding Principles
- **Warmth and Approachability**: The design creates a welcoming, human-centered experience through warm color palettes and organic visual elements
- **Clarity and Focus**: Clean layouts with ample whitespace direct attention to content and conversation
- **Trustworthiness**: Professional yet friendly aesthetic builds confidence without feeling corporate or cold
- **Adaptability**: Full support for light and dark themes while maintaining brand consistency
- **Simplicity**: Minimalist approach that removes friction from the user experience

### Visual Style Direction
- **Warm Minimalism**: Clean, uncluttered interfaces with warm, earthy tones
- **Organic Elements**: Soft rounded corners, subtle shadows, and natural color transitions
- **Content-First**: Typography and content take center stage with supporting UI elements receding into the background

### Overall Mood and Tone
- Calm and focused
- Intelligent yet accessible
- Professional but personable
- Modern with timeless qualities

### Brand Personality Expressed Through UI
- Friendly greetings ("Good morning/afternoon/evening, [Name]")
- Conversational interface design
- Warm accent colors (terracotta/coral)
- Soft, inviting backgrounds
- Human-centered iconography

### Visual Language Consistency
- Consistent use of rounded corners throughout
- Unified color temperature across all surfaces
- Harmonious spacing rhythm
- Cohesive icon style

---

## 2. Design Tokens

### Colors

#### Light Theme

##### Primary Palette
| Token | Hex | Usage |
|-------|-----|-------|
| `--color-primary` | `#CC785C` | Primary buttons, key actions, links |
| `--color-primary-hover` | `#B86A50` | Primary button hover state |
| `--color-primary-disabled` | `#D9A694` | Disabled primary buttons |

##### Secondary/Accent Colors
| Token | Hex | Usage |
|-------|-----|-------|
| `--color-accent-purple` | `#6B5B95` | Subscribe/upgrade CTAs |
| `--color-accent-purple-hover` | `#5D4F84` | Purple button hover |
| `--color-accent-teal` | `#4A9B8C` | Success indicators, checkmarks |
| `--color-accent-blue` | `#4A90A4` | Links, interactive elements |

##### Background Colors
| Token | Hex | Usage |
|-------|-----|-------|
| `--color-bg-primary` | `#F5F5F0` | Main page background |
| `--color-bg-secondary` | `#EDEEE8` | Sidebar background |
| `--color-bg-tertiary` | `#E8E8E2` | Cards, elevated surfaces |
| `--color-bg-input` | `#FFFFFF` | Input field backgrounds |
| `--color-bg-input-alt` | `#F0F0EA` | Alternative input backgrounds |
| `--color-bg-card` | `#FFFFFF` | Card backgrounds |
| `--color-bg-card-hover` | `#F8F8F4` | Card hover state |
| `--color-bg-overlay` | `rgba(0, 0, 0, 0.5)` | Modal overlays |
| `--color-bg-toast` | `#2D2A26` | Toast notification background |
| `--color-bg-banner` | `#F5F0E8` | Promotional banners |

##### Text Colors
| Token | Hex | Usage |
|-------|-----|-------|
| `--color-text-primary` | `#1A1A1A` | Primary text, headings |
| `--color-text-secondary` | `#4A4A4A` | Secondary text, descriptions |
| `--color-text-tertiary` | `#6B6B6B` | Helper text, timestamps |
| `--color-text-muted` | `#8B8B8B` | Placeholder text, disabled |
| `--color-text-inverse` | `#FFFFFF` | Text on dark backgrounds |
| `--color-text-link` | `#CC785C` | Link text |
| `--color-text-link-hover` | `#B86A50` | Link hover state |

##### Semantic Colors
| Token | Hex | Usage |
|-------|-----|-------|
| `--color-success` | `#4A9B8C` | Success states, confirmations |
| `--color-success-bg` | `#E8F5F2` | Success background |
| `--color-warning` | `#D4A84B` | Warning states |
| `--color-warning-bg` | `#FFF8E6` | Warning background |
| `--color-error` | `#C75050` | Error states, destructive actions |
| `--color-error-bg` | `#FDF2F2` | Error background |
| `--color-error-text` | `#B84242` | Error message text |
| `--color-info` | `#4A90A4` | Information states |
| `--color-info-bg` | `#E8F4F8` | Info background |

##### Border Colors
| Token | Hex | Usage |
|-------|-----|-------|
| `--color-border-primary` | `#D4D4CE` | Primary borders |
| `--color-border-secondary` | `#E0E0DA` | Subtle borders |
| `--color-border-focus` | `#CC785C` | Focus ring color |
| `--color-border-input` | `#C8C8C2` | Input field borders |
| `--color-border-error` | `#C75050` | Error state borders |

#### Dark Theme

##### Background Colors
| Token | Hex | Usage |
|-------|-----|-------|
| `--color-bg-primary-dark` | `#2D2A26` | Main page background |
| `--color-bg-secondary-dark` | `#252320` | Sidebar background |
| `--color-bg-tertiary-dark` | `#363330` | Cards, elevated surfaces |
| `--color-bg-input-dark` | `#3A3835` | Input field backgrounds |
| `--color-bg-card-dark` | `#353230` | Card backgrounds |
| `--color-bg-overlay-dark` | `rgba(0, 0, 0, 0.7)` | Modal overlays |

##### Text Colors (Dark Theme)
| Token | Hex | Usage |
|-------|-----|-------|
| `--color-text-primary-dark` | `#F5F5F0` | Primary text |
| `--color-text-secondary-dark` | `#C8C8C2` | Secondary text |
| `--color-text-tertiary-dark` | `#9A9A94` | Helper text |
| `--color-text-muted-dark` | `#6B6B65` | Placeholder, disabled |

##### Border Colors (Dark Theme)
| Token | Hex | Usage |
|-------|-----|-------|
| `--color-border-primary-dark` | `#4A4845` | Primary borders |
| `--color-border-secondary-dark` | `#3A3835` | Subtle borders |

#### Gradients
```css
/* Sunset gradient (decorative icon) */
--gradient-sunset: radial-gradient(circle, #CC785C 0%, #D4A84B 50%, #CC785C 100%);

/* Subtle card hover gradient */
--gradient-card-hover: linear-gradient(180deg, rgba(255,255,255,0.02) 0%, rgba(255,255,255,0) 100%);
```

---

### Typography

#### Font Families
```css
--font-family-display: 'Tiempos Headline', 'Georgia', serif;
--font-family-body: 'Söhne', 'Helvetica Neue', 'Arial', sans-serif;
--font-family-mono: 'Söhne Mono', 'SF Mono', 'Monaco', 'Consolas', monospace;
```

#### Font Weights
| Token | Value | Usage |
|-------|-------|-------|
| `--font-weight-regular` | 400 | Body text, descriptions |
| `--font-weight-medium` | 500 | Buttons, labels, emphasis |
| `--font-weight-semibold` | 600 | Subheadings, important text |
| `--font-weight-bold` | 700 | Headings (display font) |

#### Type Scale
| Token | Size (px) | Size (rem) | Usage |
|-------|-----------|------------|-------|
| `--font-size-xs` | 11px | 0.6875rem | Micro labels, badges |
| `--font-size-sm` | 13px | 0.8125rem | Helper text, timestamps |
| `--font-size-base` | 15px | 0.9375rem | Body text |
| `--font-size-md` | 16px | 1rem | Large body, input text |
| `--font-size-lg` | 18px | 1.125rem | Subheadings |
| `--font-size-xl` | 20px | 1.25rem | Section titles |
| `--font-size-2xl` | 24px | 1.5rem | Card titles |
| `--font-size-3xl` | 32px | 2rem | Page headings |
| `--font-size-4xl` | 40px | 2.5rem | Hero text |
| `--font-size-5xl` | 48px | 3rem | Large hero/greeting |

#### Line Heights
| Token | Value | Usage |
|-------|-------|-------|
| `--line-height-tight` | 1.2 | Headings, display text |
| `--line-height-snug` | 1.35 | Subheadings |
| `--line-height-normal` | 1.5 | Body text |
| `--line-height-relaxed` | 1.65 | Long-form reading |
| `--line-height-loose` | 1.8 | Spacious paragraphs |

#### Letter Spacing
| Token | Value | Usage |
|-------|-------|-------|
| `--letter-spacing-tight` | -0.02em | Large headings |
| `--letter-spacing-normal` | 0 | Body text |
| `--letter-spacing-wide` | 0.02em | Labels, buttons |
| `--letter-spacing-wider` | 0.05em | Uppercase labels |

#### Text Styles Catalog

##### Headings (Display Font - Serif)
```css
/* Hero Greeting */
.text-hero {
  font-family: var(--font-family-display);
  font-size: 48px;
  font-weight: 400;
  line-height: 1.2;
  letter-spacing: -0.02em;
  color: var(--color-text-primary);
}

/* Page Title */
.text-h1 {
  font-family: var(--font-family-display);
  font-size: 32px;
  font-weight: 400;
  line-height: 1.25;
  letter-spacing: -0.01em;
}

/* Section Title */
.text-h2 {
  font-family: var(--font-family-display);
  font-size: 24px;
  font-weight: 400;
  line-height: 1.3;
}

/* Subsection Title */
.text-h3 {
  font-family: var(--font-family-body);
  font-size: 18px;
  font-weight: 600;
  line-height: 1.4;
}
```

##### Body Text (Sans-serif)
```css
/* Body Large */
.text-body-lg {
  font-family: var(--font-family-body);
  font-size: 16px;
  font-weight: 400;
  line-height: 1.6;
}

/* Body Default */
.text-body {
  font-family: var(--font-family-body);
  font-size: 15px;
  font-weight: 400;
  line-height: 1.5;
}

/* Body Small */
.text-body-sm {
  font-family: var(--font-family-body);
  font-size: 13px;
  font-weight: 400;
  line-height: 1.45;
}

/* Caption */
.text-caption {
  font-family: var(--font-family-body);
  font-size: 12px;
  font-weight: 400;
  line-height: 1.4;
  color: var(--color-text-tertiary);
}

/* Label */
.text-label {
  font-family: var(--font-family-body);
  font-size: 14px;
  font-weight: 500;
  line-height: 1.4;
}

/* Button Text */
.text-button {
  font-family: var(--font-family-body);
  font-size: 14px;
  font-weight: 500;
  line-height: 1;
  letter-spacing: 0.01em;
}
```

##### Code (Monospace)
```css
/* Code Block */
.text-code {
  font-family: var(--font-family-mono);
  font-size: 14px;
  font-weight: 400;
  line-height: 1.6;
}

/* Inline Code */
.text-code-inline {
  font-family: var(--font-family-mono);
  font-size: 13px;
  font-weight: 400;
}
```

---

### Spacing

#### Base Unit
```css
--spacing-unit: 4px;
```

#### Spacing Scale
| Token | Value | Usage |
|-------|-------|-------|
| `--spacing-0` | 0px | No spacing |
| `--spacing-1` | 4px | Tight spacing, icon gaps |
| `--spacing-2` | 8px | Small gaps, compact padding |
| `--spacing-3` | 12px | Medium-tight spacing |
| `--spacing-4` | 16px | Standard padding, gaps |
| `--spacing-5` | 20px | Medium spacing |
| `--spacing-6` | 24px | Section gaps |
| `--spacing-8` | 32px | Large gaps |
| `--spacing-10` | 40px | Extra large spacing |
| `--spacing-12` | 48px | Section margins |
| `--spacing-16` | 64px | Major section breaks |
| `--spacing-20` | 80px | Page-level spacing |
| `--spacing-24` | 96px | Large page margins |

#### Component Internal Padding
| Component | Padding |
|-----------|---------|
| Button (default) | 12px 20px |
| Button (small) | 8px 16px |
| Button (large) | 16px 24px |
| Input field | 12px 16px |
| Card | 20px 24px |
| Modal | 24px 32px |
| Sidebar item | 8px 12px |
| Dropdown item | 10px 16px |

#### Layout Margins and Gaps
| Context | Value |
|---------|-------|
| Page horizontal margin | 24px (mobile) / 48px (desktop) |
| Sidebar width | 280px |
| Chat content max-width | 768px |
| Card gap in grid | 16px |
| Section vertical gap | 32px |
| Form field gap | 16px |

---

### Effects

#### Shadow Definitions
```css
/* Elevation Level 1 - Subtle */
--shadow-sm: 0 1px 2px rgba(0, 0, 0, 0.04), 0 1px 3px rgba(0, 0, 0, 0.06);

/* Elevation Level 2 - Cards */
--shadow-md: 0 2px 4px rgba(0, 0, 0, 0.04), 0 4px 8px rgba(0, 0, 0, 0.06);

/* Elevation Level 3 - Dropdowns, Popovers */
--shadow-lg: 0 4px 8px rgba(0, 0, 0, 0.06), 0 8px 16px rgba(0, 0, 0, 0.08);

/* Elevation Level 4 - Modals */
--shadow-xl: 0 8px 16px rgba(0, 0, 0, 0.08), 0 16px 32px rgba(0, 0, 0, 0.12);

/* Focus Ring Shadow */
--shadow-focus: 0 0 0 3px rgba(204, 120, 92, 0.3);

/* Inner Shadow (for inputs) */
--shadow-inner: inset 0 1px 2px rgba(0, 0, 0, 0.06);
```

#### Blur Effects
```css
--blur-sm: blur(4px);
--blur-md: blur(8px);
--blur-lg: blur(16px);
--blur-overlay: blur(4px); /* Modal backdrop */
```

#### Opacity Values
| Token | Value | Usage |
|-------|-------|-------|
| `--opacity-disabled` | 0.5 | Disabled elements |
| `--opacity-muted` | 0.6 | Muted content |
| `--opacity-hover` | 0.8 | Hover overlays |
| `--opacity-overlay` | 0.5 | Modal backdrops |
| `--opacity-overlay-dark` | 0.7 | Dark theme overlays |

---

### Borders

#### Border Widths
| Token | Value | Usage |
|-------|-------|-------|
| `--border-width-none` | 0 | No border |
| `--border-width-thin` | 1px | Default borders |
| `--border-width-medium` | 2px | Focus states, emphasis |
| `--border-width-thick` | 3px | Active states |

#### Border Radius Scale
| Token | Value | Usage |
|-------|-------|-------|
| `--radius-none` | 0 | Sharp corners |
| `--radius-sm` | 4px | Small elements, badges |
| `--radius-md` | 8px | Buttons, inputs |
| `--radius-lg` | 12px | Cards, modals |
| `--radius-xl` | 16px | Large cards |
| `--radius-2xl` | 24px | Chat bubbles, large modals |
| `--radius-pill` | 9999px | Pills, toggle switches |
| `--radius-circle` | 50% | Avatars, circular buttons |

#### Border Styles
```css
--border-solid: solid;
--border-dashed: dashed;
```

---

### Iconography

#### Icon Style
- **Style**: Outlined (line icons)
- **Stroke Weight**: 1.5px - 2px
- **Corner Style**: Rounded
- **Library**: Custom icon set (similar to Lucide/Feather style)

#### Icon Sizes
| Token | Size | Usage |
|-------|------|-------|
| `--icon-xs` | 12px | Inline with small text |
| `--icon-sm` | 16px | Buttons, inline elements |
| `--icon-md` | 20px | Default icon size |
| `--icon-lg` | 24px | Navigation, prominent icons |
| `--icon-xl` | 32px | Feature icons |
| `--icon-2xl` | 48px | Illustration icons |

#### Common Icons Used
- Chat bubble (conversations)
- Star (favorites/starred)
- Settings gear
- Plus/Add
- Close/X
- Arrow (back, forward, expand)
- Paperclip (attachments)
- Copy
- Retry/Refresh
- Thumbs up/down
- Send arrow
- Document/File
- Globe (published)
- Lock (private)
- User avatar circle
- Checkbox (checked/unchecked)
- Chevron (dropdown indicators)

---

### Motion & Animation

#### Easing Curves
```css
--ease-default: cubic-bezier(0.4, 0, 0.2, 1);
--ease-in: cubic-bezier(0.4, 0, 1, 1);
--ease-out: cubic-bezier(0, 0, 0.2, 1);
--ease-in-out: cubic-bezier(0.4, 0, 0.2, 1);
--ease-bounce: cubic-bezier(0.68, -0.55, 0.265, 1.55);
```

#### Duration Scale
| Token | Value | Usage |
|-------|-------|-------|
| `--duration-instant` | 0ms | Immediate feedback |
| `--duration-fast` | 100ms | Micro-interactions |
| `--duration-normal` | 200ms | Standard transitions |
| `--duration-slow` | 300ms | Larger transitions |
| `--duration-slower` | 400ms | Modal animations |
| `--duration-slowest` | 500ms | Page transitions |

#### Common Animation Patterns
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

/* Pulse (loading indicator) */
@keyframes pulse {
  0%, 100% { opacity: 1; }
  50% { opacity: 0.5; }
}

/* Spin (loading spinner) */
@keyframes spin {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}
```

#### Transition Properties
```css
/* Standard transition */
.transition-default {
  transition-property: background-color, border-color, color, opacity;
  transition-duration: var(--duration-normal);
  transition-timing-function: var(--ease-default);
}

/* Transform transition */
.transition-transform {
  transition-property: transform;
  transition-duration: var(--duration-normal);
  transition-timing-function: var(--ease-default);
}

/* All properties */
.transition-all {
  transition: all var(--duration-normal) var(--ease-default);
}
```

---

## 3. Components

### Buttons

#### Primary Button
**Purpose**: Main call-to-action, primary user actions

**Dimensions**:
- Height: 44px (default), 36px (small), 52px (large)
- Min-width: 80px
- Padding: 12px 20px (default), 8px 16px (small), 16px 24px (large)
- Border-radius: 8px

**Visual Variants**:

| State | Background | Text | Border |
|-------|------------|------|--------|
| Default | `#CC785C` | `#FFFFFF` | none |
| Hover | `#B86A50` | `#FFFFFF` | none |
| Active | `#A55E45` | `#FFFFFF` | none |
| Focus | `#CC785C` | `#FFFFFF` | 3px focus ring `rgba(204,120,92,0.3)` |
| Disabled | `#D9A694` | `#FFFFFF` | none, opacity: 0.6 |
| Loading | `#CC785C` | Spinner | none |

**Typography**:
- Font: Sans-serif
- Size: 14px
- Weight: 500
- Letter-spacing: 0.01em

**Anatomy**:
- Optional leading icon (16px, 8px gap)
- Label text
- Optional trailing icon (16px, 8px gap)

---

#### Secondary Button
**Purpose**: Secondary actions, less prominent CTAs

**Dimensions**: Same as Primary

**Visual Variants**:

| State | Background | Text | Border |
|-------|------------|------|--------|
| Default | `#F0F0EA` | `#1A1A1A` | none |
| Hover | `#E8E8E2` | `#1A1A1A` | none |
| Active | `#E0E0DA` | `#1A1A1A` | none |
| Focus | `#F0F0EA` | `#1A1A1A` | 3px focus ring |
| Disabled | `#F5F5F0` | `#8B8B8B` | none |

---

#### Ghost Button
**Purpose**: Tertiary actions, navigation elements

**Dimensions**: Same padding, height adapts to content

**Visual Variants**:

| State | Background | Text | Border |
|-------|------------|------|--------|
| Default | transparent | `#4A4A4A` | none |
| Hover | `rgba(0,0,0,0.05)` | `#1A1A1A` | none |
| Active | `rgba(0,0,0,0.08)` | `#1A1A1A` | none |
| Focus | transparent | `#1A1A1A` | 3px focus ring |
| Disabled | transparent | `#8B8B8B` | none |

---

#### Purple/Accent Button (Subscribe CTA)
**Purpose**: Premium upgrade actions, special CTAs

**Dimensions**: Same as Primary

**Visual Variants**:

| State | Background | Text | Border |
|-------|------------|------|--------|
| Default | `#6B5B95` | `#FFFFFF` | none |
| Hover | `#5D4F84` | `#FFFFFF` | none |
| Active | `#504573` | `#FFFFFF` | none |

---

#### Destructive/Danger Button
**Purpose**: Delete actions, destructive operations

**Dimensions**: Same as Primary

**Visual Variants**:

| State | Background | Text | Border |
|-------|------------|------|--------|
| Default | `#C75050` | `#FFFFFF` | none |
| Hover | `#B84545` | `#FFFFFF` | none |
| Active | `#A53D3D` | `#FFFFFF` | none |
| Focus | `#C75050` | `#FFFFFF` | 3px focus ring `rgba(199,80,80,0.3)` |

**Usage Notes**:
- Used for "Delete", "Delete Account", "I Understand" confirmation buttons
- Always paired with a "Cancel" secondary button
- Typically appears in confirmation modals

---

#### Icon Button
**Purpose**: Actions represented by icons only

**Dimensions**:
- Size: 32px x 32px (small), 40px x 40px (default), 48px x 48px (large)
- Border-radius: 8px or 50% (circular variant)

**Visual Variants**: Same states as Ghost button

---

### Inputs

#### Text Input
**Purpose**: Single-line text entry

**Dimensions**:
- Height: 44px (default), 36px (small), 52px (large)
- Padding: 12px 16px
- Border-radius: 8px

**Visual States**:

| State | Background | Border | Text |
|-------|------------|--------|------|
| Default | `#FFFFFF` | 1px `#C8C8C2` | `#1A1A1A` |
| Hover | `#FFFFFF` | 1px `#A0A09A` | `#1A1A1A` |
| Focus | `#FFFFFF` | 2px `#CC785C` | `#1A1A1A` |
| Filled | `#FFFFFF` | 1px `#C8C8C2` | `#1A1A1A` |
| Disabled | `#F5F5F0` | 1px `#E0E0DA` | `#8B8B8B` |
| Error | `#FFFFFF` | 2px `#C75050` | `#1A1A1A` |

**Placeholder**: Color `#8B8B8B`

**Typography**:
- Font: Sans-serif
- Size: 15px
- Weight: 400

**Anatomy**:
- Optional label (above, 4px gap)
- Input container
- Optional helper text (below, 4px gap)
- Optional leading/trailing icons

---

#### Textarea
**Purpose**: Multi-line text entry

**Dimensions**:
- Min-height: 100px
- Padding: 12px 16px
- Border-radius: 12px (chat input), 8px (forms)
- Resize: vertical

**Chat Input Variant**:
- Background: `#FFFFFF` (light) / `#3A3835` (dark)
- Border-radius: 24px
- Padding: 16px 20px
- Placeholder: "How can Claude help you today?" / "Reply to Claude..."

---

#### Select/Dropdown
**Purpose**: Single selection from a list

**Dimensions**: Same as Text Input

**Trigger Visual**:
- Trailing chevron icon (16px)
- Same states as Text Input

**Dropdown Panel**:
- Background: `#FFFFFF`
- Border-radius: 12px
- Shadow: `--shadow-lg`
- Max-height: 320px (scrollable)
- Padding: 8px

**Dropdown Item**:
- Padding: 10px 16px
- Border-radius: 6px
- Hover: Background `#F5F5F0`
- Selected: Background `#F0F0EA`, checkmark icon

---

#### Checkbox
**Purpose**: Multiple selection, agreement toggles

**Dimensions**:
- Box size: 18px x 18px
- Border-radius: 4px
- Border: 2px

**Visual States**:

| State | Background | Border | Checkmark |
|-------|------------|--------|-----------|
| Unchecked | transparent | `#C8C8C2` | none |
| Unchecked Hover | transparent | `#A0A09A` | none |
| Checked | `#4A9B8C` | `#4A9B8C` | white |
| Checked Hover | `#3D8A7A` | `#3D8A7A` | white |
| Disabled | `#E0E0DA` | `#E0E0DA` | `#8B8B8B` if checked |

**Anatomy**:
- Checkbox box
- Label (8px gap from box)
- Optional description below label

---

#### Radio Button
**Purpose**: Single selection from multiple options

**Dimensions**:
- Circle size: 18px x 18px
- Inner dot: 8px

**Visual States**: Similar to Checkbox but circular

---

#### Toggle Switch
**Purpose**: Binary on/off settings

**Dimensions**:
- Track: 44px x 24px
- Thumb: 20px x 20px
- Border-radius: pill (9999px)

**Visual States**:

| State | Track Background | Thumb Position |
|-------|------------------|----------------|
| Off | `#D4D4CE` | Left (2px from edge) |
| Off Hover | `#C8C8C2` | Left |
| On | `#CC785C` (primary terracotta) | Right (2px from edge) |
| On Hover | `#B86A50` | Right |
| Disabled Off | `#E8E8E2` | Left, opacity 0.5 |
| Disabled On | `#D9A694` | Right, opacity 0.5 |

**Animation**: Thumb slides with 200ms ease transition

**Note**: Toggle "On" state uses primary terracotta color for consistency with brand

---

#### Phone Input with Country Selector
**Purpose**: International phone number entry

**Dimensions**:
- Height: 44px
- Combined width: flexible

**Anatomy**:
- Country selector (left): 72px width, flag icon + chevron
- Phone input (right): flexible width, joined border

**Country Selector**:
- Background: `#F5F5F0`
- Border: 1px `#C8C8C2`
- Border-radius: 8px 0 0 8px (left rounded only)
- Flag icon: 20px width
- Dropdown: Full country list with flags

**Phone Input**:
- Background: `#FFFFFF`
- Border: 1px `#C8C8C2`
- Border-radius: 0 8px 8px 0 (right rounded only)
- Border-left: none (joined with selector)
- Placeholder: "(555) 000-0000"

---

#### Verification Code Input
**Purpose**: SMS/Email verification code entry

**Dimensions**:
- Height: 52px
- Width: 100% (single input field)
- Padding: 16px 20px
- Border-radius: 8px

**Visual**:
- Background: `#FFFFFF` (light) / `#3A3835` (dark)
- Border: 1px `#C8C8C2`
- Text: Centered, 18px, medium weight
- Placeholder: "Enter verification code"

**Associated Elements**:
- "Not seeing the code? Try again" link below
- Phone number display above

---

### Cards

#### Chat History Card
**Purpose**: Display recent conversation preview

**Dimensions**:
- Padding: 16px 20px
- Border-radius: 12px
- Min-height: [estimated] 100px

**Visual**:
- Background: `#FFFFFF` (light) / `#353230` (dark)
- Border: none
- Shadow: none (flat design)
- Hover: Background `#F8F8F4` / `#3A3835`

**Anatomy**:
- Chat icon (20px, top-left)
- Title (font-weight: 600, truncate at 2 lines)
- Timestamp (font-size: 13px, color: tertiary)

---

#### Prompt Suggestion Card
**Purpose**: Quick-start prompt templates

**Dimensions**:
- Padding: 16px
- Border-radius: 8px
- Width: flexible within grid

**Visual**:
- Background: `#F5F5F0`
- Border: none
- Hover: Background `#EDEEE8`, slight lift

**Anatomy**:
- Prompt text (2 lines max, 14px)
- Decorative corner icon

**Hover Tooltip**: "Try this prompt" (dark background pill)

---

#### File Attachment Card
**Purpose**: Display attached files

**Dimensions**:
- Padding: 12px 16px
- Border-radius: 8px
- Max-width: 300px

**Visual**:
- Background: `#F0F0EA`
- Border: 1px `#E0E0DA`

**Anatomy**:
- File type icon (24px)
- Filename (truncated, 14px, medium weight)
- File size / type label (12px, tertiary color)
- Remove button (X icon, top-right)

---

#### Pricing Card
**Purpose**: Plan comparison display

**Dimensions**:
- Padding: 32px
- Border-radius: 16px
- Width: ~400px

**Visual**:
- Background: `#FFFFFF` / `#F5F5F0`
- Border: 1px `#E0E0DA` or none

**Anatomy**:
- Plan illustration icon (48px)
- Plan name (serif, 24px)
- Price (large, 32px + "/ month" smaller)
- Feature list with checkmark icons
- CTA button at bottom

---

### Modals/Dialogs

#### Standard Modal
**Purpose**: Focused interactions requiring user attention

**Dimensions**:
- Width: 480px (small), 560px (default), 720px (large)
- Max-height: 90vh
- Padding: 24px 32px
- Border-radius: 16px

**Visual**:
- Background: `#FFFFFF` (light) / `#2D2A26` (dark)
- Shadow: `--shadow-xl`
- Overlay: `rgba(0,0,0,0.5)` with blur

**Anatomy**:
- Header: Title (serif, 24px) + Close button (X, top-right)
- Body: Content area (flexible)
- Footer: Action buttons (right-aligned, 12px gap)

**Animation**:
- Enter: Fade in + scale from 95% (300ms)
- Exit: Fade out + scale to 95% (200ms)

---

#### Rename Modal
**Purpose**: Rename conversations

**Specific Elements**:
- Single text input
- Cancel + Save buttons
- Width: 400px

---

#### Feedback Modal
**Purpose**: Collect user feedback

**Specific Elements**:
- Title: "Give feedback"
- Textarea for feedback
- Character limit indicator (optional)
- Cancel + Send buttons

---

#### Publish Modal
**Purpose**: Publish artifacts publicly

**Specific Elements**:
- Privacy selection (radio buttons)
- Generated URL with copy button
- Warning text about unpublishing
- Unpublish / Done buttons

---

#### Feature Preview Modal
**Purpose**: Introduce new features

**Specific Elements**:
- Feature illustration
- Title + description
- Toggle to enable feature
- Close button

---

#### Delete Confirmation Modal
**Purpose**: Confirm destructive actions (delete chat, delete account)

**Dimensions**:
- Width: 400px
- Padding: 24px

**Specific Elements**:
- Warning icon (optional)
- Title: "Delete this chat?" / "Delete your account?"
- Description text explaining consequences
- Two buttons: "Cancel" (secondary) + "Delete" / "I Understand" (destructive red)

**Visual**:
- Background: `#FFFFFF` (light) / `#2D2A26` (dark)
- Destructive button: `#C75050`
- Cancel button: Secondary style

---

#### Account Export Modal
**Purpose**: Export user data

**Specific Elements**:
- Title: "Export data"
- Description of what data is included
- "Export data" primary button

---

### Dropdowns/Menus

#### Context Menu
**Purpose**: Right-click or overflow actions

**Dimensions**:
- Min-width: 160px
- Max-width: 280px
- Padding: 4px
- Border-radius: 12px

**Visual**:
- Background: `#FFFFFF`
- Shadow: `--shadow-lg`
- Border: 1px `#E0E0DA`

**Menu Item**:
- Padding: 10px 12px
- Border-radius: 6px
- Hover: Background `#F5F5F0`
- Icon: 16px, 12px gap from label
- Destructive items: Text color `#C75050`

**Separator**:
- Height: 1px
- Background: `#E0E0DA`
- Margin: 4px 8px

---

#### Appearance Submenu
**Purpose**: Theme selection

**Items**:
- System (with device icon)
- Light (with sun icon)
- Dark (with moon icon)
- Checkmark on selected item

---

### Navigation

#### Header/Top Bar
**Dimensions**:
- Height: 56px
- Padding: 0 24px
- Background: transparent or `#F5F5F0`

**Anatomy**:
- Left: Product wordmark "Claude" (serif, 20px)
- Center: Conversation title with dropdown + icon
- Right: Star (favorite) + Settings + Avatar with notification badge

---

#### Sidebar
**Dimensions**:
- Width: 280px (expanded), 64px (collapsed)
- Background: `#EDEEE8` (light) / `#252320` (dark)

**Sections**:
1. Logo/Brand (top)
2. "Start new chat" button
3. Starred chats section
4. Recent chats section
5. User account section (bottom)

**Sidebar Item**:
- Padding: 8px 12px
- Border-radius: 8px
- Hover: Background `#E0E0DA`
- Active: Background `#D8D8D2`
- Icon: 16px + 12px gap + Label

**Collapsible**: Chevron button to collapse/expand

---

#### Tabs
**Purpose**: Content section navigation

**Tab Item**:
- Padding: 12px 16px
- Border-bottom: 2px (active indicator)
- Active: `#CC785C` bottom border, `#1A1A1A` text
- Inactive: No border, `#6B6B6B` text
- Hover: `#4A4A4A` text

---

### Tables

**Not prominently featured in the interface**, but when present:

- Header: Bold text, background `#F5F5F0`
- Row: Padding 12px 16px
- Border: 1px bottom `#E0E0DA`
- Hover: Background `#F8F8F4`

---

### Lists

#### Chat Message List
**Purpose**: Conversation history display

**Message Bubble - User**:
- Background: `#F0F0EA`
- Border-radius: 20px
- Padding: 16px 20px
- Max-width: 85%
- Alignment: Right

**Message Bubble - AI Response**:
- Background: transparent
- Padding: 16px 0
- Full width
- Avatar icon (left-aligned, inline with first line)

**Message Actions**:
- Copy, Retry, Thumbs up/down
- Icon buttons, 32px
- Appear on hover

---

### Badges/Tags/Chips

#### NEW Badge
**Purpose**: Highlight new features

**Dimensions**:
- Padding: 4px 8px
- Border-radius: 4px

**Visual**:
- Background: `#4A9B8C`
- Text: `#FFFFFF`, 11px, uppercase, font-weight 600

---

#### Plan Badge
**Purpose**: Show user's subscription tier

**Visual**:
- "Free plan" - subtle text
- "Pro" - with icon

---

#### File Type Badge
**Purpose**: Indicate file types on attachments

**Visual**:
- Background: color-coded by type
- Text: uppercase, small

---

### Avatars

#### User Avatar
**Dimensions**:
- Size: 32px (default), 24px (small), 48px (large)
- Border-radius: 50%

**Visual**:
- Background: `#4A4A4A` (fallback)
- Initials: White, centered (if no image)
- Image: Cover, rounded

**With Notification Badge**:
- Badge: 8px circle
- Position: Top-right, overlapping
- Color: `#CC785C` or `#C75050`

---

### Tooltips

**Purpose**: Additional context on hover

**Dimensions**:
- Padding: 8px 12px
- Border-radius: 6px
- Max-width: 280px

**Visual**:
- Background: `#1A1A1A`
- Text: `#FFFFFF`, 13px
- Shadow: `--shadow-md`

**Arrow**: 6px triangle pointing to trigger

**Animation**: Fade in after 200ms delay

---

### Alerts/Banners

#### Inline Banner
**Purpose**: System messages, upgrade prompts

**Dimensions**:
- Padding: 12px 16px
- Border-radius: 8px
- Full width (within container)

**Visual**:
- Background: `#FFF8E6` (warning), `#FDF2F2` (error)
- Border-left: 4px solid semantic color (optional)
- Icon: 20px, left-aligned

**Upgrade Banner**:
- Background: `#F5F0E8`
- "Subscribe to Pro for 5x more usage with Claude 3.5 Sonnet"
- CTA link on right

---

#### Rate Limit Warning Banner
**Purpose**: Notify user of usage limits

**Dimensions**:
- Padding: 16px 24px
- Border-radius: 12px
- Max-width: matches content area

**Visual**:
- Background: `#F5F0E8` / `#FFF8E6`
- Warning icon: Triangle with exclamation, `#D4A84B` (amber)
- Text: "You are out of free messages until [time]"
- CTA: "Subscribe to Pro" button (purple accent)

**Anatomy**:
- Warning icon (24px, left)
- Message text with linked "messages" text
- Time indicator
- Subscribe button (right-aligned)

---

#### Toast Notification
**Purpose**: Transient feedback messages

**Dimensions**:
- Padding: 12px 16px
- Border-radius: 8px
- Min-width: 280px
- Max-width: 400px

**Visual**:
- Background: `#2D2A26` (dark theme default for toasts)
- Text: `#F5F5F0`
- Shadow: `--shadow-lg`

**Position**:
- Default: Bottom-center
- Alternative: Top-right (for non-blocking notifications)
- Settings confirmations: Top-right with checkmark

**Types**:
- Success: Green checkmark icon, teal accent
- Error: Red X icon, red accent
- Warning: Amber triangle icon
- Info: Blue info icon

**Toast Variants**:

| Type | Background | Icon Color | Position |
|------|------------|------------|----------|
| Success | `#2D2A26` | `#4A9B8C` | Top-right |
| Error | `#2D2A26` | `#C75050` | Bottom-center |
| Warning | `#2D2A26` | `#D4A84B` | Top-right |
| Info | `#2D2A26` | `#4A90A4` | Bottom-center |

**Animation**: Slide up + fade in, auto-dismiss after 4s (8s for errors)

---

### Progress Indicators

#### Loading Spinner
**Dimensions**: 20px (default), 16px (small), 32px (large)

**Visual**:
- Color: `#CC785C` or current text color
- Animation: Spin, 1s linear infinite

**AI Thinking Indicator**:
- Animated logo/icon
- Pulsing opacity
- "Claude is thinking..." text (optional)

---

#### Skeleton Loading
**Visual**:
- Background: `#E8E8E2`
- Animated shimmer gradient
- Rounded corners matching actual content

---

### Accordions

#### FAQ Accordion
**Purpose**: Expandable content sections

**Dimensions**:
- Padding: 16px 20px
- Border-radius: 8px (if card style)

**Header**:
- Question text: 16px, medium weight
- Chevron icon: right-aligned, rotates on expand

**Content**:
- Padding-top: 12px
- Text: 15px, regular weight
- Line-height: 1.6

**Animation**: Height transition, 200ms ease

---

### Collapsible Sections

#### Section Header (Collapsible)
**Purpose**: Expandable content sections with header toggle

**Dimensions**:
- Padding: 8px 0
- Gap between icon and title: 8px

**Anatomy**:
- Leading icon (optional, 20px)
- Section title (font-weight: 600, 16px)
- Chevron icon (16px, right side)
- Optional trailing action link ("View all →")

**Visual States**:
- Expanded: Chevron points up
- Collapsed: Chevron points down
- Hover: Subtle background on clickable area

**Animation**:
- Chevron: Rotate 180deg, 200ms ease
- Content: Height transition, 200ms ease

---

### Search

#### Chat History Search
**Purpose**: Search through past conversations

**Dimensions**:
- Page layout: Full page with sidebar
- Search input: Full width of content area
- Height: 48px
- Padding: 12px 16px
- Border-radius: 8px

**Search Input**:
- Background: `#FFFFFF`
- Border: 1px `#C8C8C2`
- Leading icon: Search magnifying glass, 20px
- Placeholder: Search query text displayed

**Results List**:
- Chat item cards
- Title + timestamp
- Chat icon on left
- Hover state: Background `#F5F5F0`

**Empty State**: No results display (clean empty area)

---

### Drawers/Panels

#### File Content Drawer
**Purpose**: Display extracted content from uploaded files

**Dimensions**:
- Width: 480px (same as artifact panel)
- Position: Right side panel
- Header: 56px

**Header**:
- Back arrow button (left)
- Title: "File content"
- Close button (X, right)

**Content Area**:
- Info notice: "Formatting may be inconsistent from source" with info icon
- File metadata: Filename, size, extracted lines count
- Document content: Monospace or serif font
- Scrollable content area

**Info Notice**:
- Background: Subtle warning/info
- Icon: Info circle, 16px
- Text: 13px, tertiary color

---

#### Artifact Side Panel
**Purpose**: Display generated artifacts (code, documents, etc.)

**Dimensions**:
- Width: 480px
- Position: Right side, full height
- Header: 56px

**Header Anatomy**:
- Back arrow (left)
- Artifact title (center)
- Star/favorite button
- Action menu (more options)
- Close button (right)

**Tab Bar** (when applicable):
- Preview / Code toggle
- Segmented control style
- Active tab: Background `#F0F0EA`, text `#1A1A1A`
- Inactive tab: Background transparent, text `#6B6B6B`

**Footer Actions**:
- Publish button
- Copy button
- Download button

---

### Code Block

#### Artifact Code Panel
**Purpose**: Display generated code

**Dimensions**:
- Full height panel (right side)
- Header: 48px
- Padding: 16px

**Visual**:
- Background: `#1E1E1E` (VS Code dark theme style)
- Border-radius: 12px (if floating)
- Monospace font

**Header**:
- Back arrow
- File/artifact title
- Action buttons (copy, download, publish)

**Syntax Highlighting**:
- Keywords: `#569CD6` (blue)
- Strings: `#CE9178` (orange)
- Comments: `#6A9955` (green)
- Functions: `#DCDCAA` (yellow)
- Numbers: `#B5CEA8` (light green)
- Variables: `#9CDCFE` (cyan)

---

## 4. Layout System

### Grid System
- **Type**: Flexible, content-centered
- **Max content width**: 768px (chat), 1200px (full pages)
- **Columns**: Not strictly columnar; component-based layout

### Container Max-widths
| Container | Max-width |
|-----------|-----------|
| Chat content | 768px |
| Settings content | 720px |
| Modal content | 560px |
| Pricing cards | 1000px (2-up grid) |
| Full page | 1400px |

### Breakpoints
| Name | Value | Usage |
|------|-------|-------|
| `xs` | 0 | Mobile base |
| `sm` | 480px | Large mobile |
| `md` | 768px | Tablet |
| `lg` | 1024px | Desktop |
| `xl` | 1280px | Large desktop |
| `2xl` | 1536px | Extra large screens |

### Responsive Behavior Rules
- **Sidebar**: Collapsible on mobile, overlay drawer
- **Chat panel**: Full width on mobile
- **Artifact panel**: Full screen modal on mobile, side panel on desktop
- **Grid cards**: 1 column mobile, 2 columns tablet, 3 columns desktop

### Page Structure Templates

#### Chat Interface Layout
```
┌─────────────────────────────────────────────────┐
│ Header (56px)                                   │
├─────────────┬───────────────────────────────────┤
│             │                                   │
│  Sidebar    │       Chat Content                │
│  (280px)    │       (flexible)                  │
│             │                                   │
│             ├───────────────────────────────────┤
│             │       Input Area                  │
└─────────────┴───────────────────────────────────┘
```

#### Chat with Artifact Layout
```
┌─────────────────────────────────────────────────┐
│ Header (56px)                                   │
├─────────────┬─────────────────┬─────────────────┤
│             │                 │                 │
│  Sidebar    │  Chat Content   │  Artifact Panel │
│  (280px)    │  (flexible)     │  (480px)        │
│             │                 │                 │
│             ├─────────────────┤                 │
│             │  Input Area     │                 │
└─────────────┴─────────────────┴─────────────────┘
```

#### Settings Page Layout
```
┌─────────────────────────────────────────────────┐
│ Header (56px)                                   │
├─────────────┬───────────────────────────────────┤
│             │                                   │
│  Sidebar    │       Settings Content            │
│  (280px)    │       (max 720px, centered)       │
│             │                                   │
│             │                                   │
└─────────────┴───────────────────────────────────┘
```

### Content Width Constraints
| Context | Max-width |
|---------|-----------|
| Prose content | 65ch (optimal reading) |
| Form fields | 400px |
| Chat messages | 85% of container |
| Modal body | 100% of modal |

### Vertical Rhythm
- **Base unit**: 8px
- **Section gaps**: 32px - 48px
- **Component gaps**: 16px - 24px
- **Related element gaps**: 8px - 12px

---

## 5. Patterns

### Navigation Patterns

#### Header Behavior
- **Position**: Sticky top
- **Scroll effect**: None (stays consistent)
- **Mobile**: Logo + hamburger menu

#### Sidebar Patterns
- **Expand/Collapse**: Toggle button (chevron icon)
- **Scroll**: Independent scroll within sidebar
- **Active state**: Background highlight
- **Hover**: Subtle background change

#### Tab Navigation
- **Style**: Underline indicator
- **Animation**: Indicator slides between tabs
- **Mobile**: Horizontal scroll if needed

#### Link Styles
- **Default**: `#CC785C`, no underline
- **Hover**: `#B86A50`, underline
- **Visited**: Same as default
- **Active**: `#A55E45`

---

### Form Patterns

#### Form Layout
- **Label position**: Above input (4px gap)
- **Field grouping**: 16px gap between fields
- **Related fields**: 12px gap
- **Section breaks**: 24px gap

#### Validation Display
- **Inline errors**: Below input, red text, error icon
- **Error border**: 2px red on input
- **Success state**: Green checkmark (optional)

#### Required Field Indication
- No asterisk by default
- "(optional)" suffix for optional fields
- Or "(required)" for critical required fields

#### Helper Text
- **Position**: Below input
- **Style**: 13px, tertiary color
- **With error**: Replaced by error message

#### Input Group Patterns
- Multiple inputs in a row (e.g., address)
- Unified border treatment
- Consistent height

---

### Content Patterns

#### Card Layouts
- **Grid**: 3 columns desktop, 2 tablet, 1 mobile
- **Gap**: 16px
- **Alignment**: Stretch to equal height

#### Empty States
- **Illustration**: Simple, on-brand graphic
- **Heading**: Friendly message
- **Description**: Helpful next step
- **CTA**: Primary action button

#### Loading States
- **Skeleton screens**: For initial load
- **Spinners**: For actions in progress
- **Progress text**: "Claude is thinking..."

#### Error States
- **404 Page**: Friendly message, navigation options
- **Error toast**: Transient, dismissible
- **Inline error**: For form fields

---

### Feedback Patterns

#### Toast Positioning
- **Default**: Bottom-center
- **Mobile**: Full width at bottom
- **Stacking**: New toasts push old ones up

#### Toast Animation
- **Enter**: Slide up + fade in (300ms)
- **Exit**: Fade out + slide down (200ms)
- **Auto-dismiss**: 4 seconds (standard), 8 seconds (errors)

#### Modal Overlay
- **Background**: Black at 50% opacity
- **Blur**: 4px backdrop blur
- **Click outside**: Dismisses modal
- **Escape key**: Dismisses modal

#### Confirmation Dialogs
- **Destructive actions**: Require explicit confirmation
- **Primary action**: On the right
- **Destructive button**: Red styling

#### Inline Feedback
- **Success messages**: Green text/icon
- **Error messages**: Red text/icon below input
- **Character counts**: Below textarea, right-aligned

---

## 6. Page Templates

### Home/New Chat Page
**Structure**:
- Greeting banner (time-based: "Good morning/afternoon/evening, [Name]")
- Plan status indicator (if free plan): "Using limited free plan" + "Upgrade" link
- Rate limit warning (when applicable): Banner with warning icon
- Chat input (large, centered)
- Prompt suggestions (optional, 3 cards if enabled)
- "Your recent chats" collapsible section
- Recent chats grid (3 columns, 2 rows = 6 cards)
- "View all" link

**Collapsible "Your recent chats" Section**:
- Section header with chat icon
- Title: "Your recent chats"
- Chevron icon (rotates on collapse/expand)
- "View all →" link (right-aligned)

**Recent Chat Cards**:
- 3-column grid layout
- Card padding: 16px
- Chat bubble icon (top)
- Chat title (truncated, 2 lines max)
- Timestamp: "X minutes ago"
- Hover: Slight background change

**Spacing**:
- Greeting: 48px from header
- Rate limit banner: 24px below greeting
- Input: 32px below banner/greeting
- Recent chats section: 32px below input
- Card grid gap: 16px

---

### Chat Conversation Page
**Structure**:
- Header with conversation title
- Message list (alternating user/AI)
- Chat input (bottom, sticky)

**Message Spacing**:
- Between different authors: 24px
- Consecutive same author: 8px

---

### Settings Page
**Structure**:
- Header with "Settings" title and gear icon
- Settings navigation (vertical tabs on left)
- Content area with form sections
- Form cards with rounded corners

**Navigation Tabs**:
- Profile (default active)
- Billing
- Account
- Active tab: Background `#F5F5F0`, left border accent

**Profile Section**:
- Card 1: Name settings
  - Full name (text input)
  - "What should we call you?" (text input)
  - "Update Name" button
- Card 2: Work settings
  - "What best describes your work?" (dropdown)
  - "Show prompt suggestions?" (toggle switch)

**Billing Section**:
- Current plan display
- "Subscribe Now" / "Manage subscription" button (purple accent)
- Payment method (if subscribed)

**Account Section**:
- "Export data" button (secondary)
- "Delete Account" button (destructive red)
- Warning text about deletion consequences

---

### Pricing/Subscription Page
**Structure**:
- Header
- Page title (centered)
- Plan cards (side by side)
- Feature comparison (optional)

---

### Login/Auth Pages
**Structure**:
- Centered card layout
- Logo at top
- Form fields
- Social login options
- Links to alternate actions

---

### Onboarding Flow Pages

#### Step 1: Name Entry
**Structure**:
- Centered layout
- "Hello, I'm Claude" greeting (serif, large)
- "What should I call you?" prompt
- Single text input for name/nickname
- Continue button

**Visual**:
- Background: `#2D2A26` (dark theme)
- Text: `#F5F5F0`
- Input: Dark background input

---

#### Step 2: Usage Policy
**Structure**:
- Title: "A few things to know before we begin"
- Info cards with blue icons
- Each card: Icon + title + description
- "Acknowledge & Continue" primary button

**Info Cards**:
- Icon: Circle with info icon, blue `#4A90A4`
- Title: Bold, 16px
- Description: Regular, 14px, secondary color
- Spacing: 16px between cards

**Topics Covered**:
- Usage guidelines
- Data handling
- AI limitations

---

#### Step 3: Getting Started
**Structure**:
- Title: "Wonderful, [Name]. Here are a few more things to know."
- Info cards with blue icons (similar to Step 2)
- "Sounds Good, Let's Begin" button with arrow icon

---

#### Phone Verification Page
**Structure**:
- Logo at top center
- Title: "First, let's create your account"
- Subtitle: "Verify mobile phone number & age"
- Country selector + Phone input
- Age confirmation checkbox
- "Send Verification Code" primary button
- Helper text about phone requirements
- Footer: Email verified status + change email link

**Visual** (Dark Theme):
- Background: `#2D2A26`
- Input backgrounds: `#3A3835`
- Checkbox: Teal when checked

**Error State**:
- Red error text: "Error sending code. Double check your phone number."
- Centered below checkbox, above button

---

#### Code Verification Page
**Structure**:
- Logo at top center
- Title: "First, let's create your account"
- Instruction: "Please enter the code sent via text to: [phone]"
- Verification code input
- "Verify & Create Account" primary button
- "Not seeing the code? Try again" link
- Footer: Email verified status

---

### Chat History Page
**Structure**:
- Header with "Your chat history" title
- "Start New Chat" button (top-right)
- Search input (full width)
- Results list (chat items)

**Anatomy**:
- Sidebar (left)
- Main content area with search
- Chat history list below

---

### Subscription Form Page
**Structure**:
- Back arrow (top-left)
- Logo (top-center)
- Title: "Subscribe to Pro plan"
- Plan summary box (lavender background)
- Billing form fields

**Plan Summary Box**:
- Background: `#E8E4F0` (light lavender/purple)
- Price: "£18/month (includes VAT)"
- Feature list with checkmark icons
- Features in `#6B5B95` purple accent for price highlight

**Form Fields**:
- Full name (read-only from profile)
- Country or region (dropdown)
- Address line 1
- Address line 2 (optional)
- Town or city
- Postal code
- Payment method section

---

## 7. Imagery & Media

### Image Aspect Ratios
| Usage | Ratio |
|-------|-------|
| User uploaded images | Preserve original |
| Thumbnails | 1:1 (square) |
| Preview images | 16:9 |
| Avatars | 1:1 (circular crop) |

### Image Border Treatments
- **Border-radius**: 8px (standard), 12px (larger images)
- **Border**: None by default, 1px `#E0E0DA` on some contexts
- **Shadow**: `--shadow-sm` on hover (optional)

### Placeholder/Fallback Styles
- **Avatar fallback**: Initials on colored background
- **Image loading**: Skeleton placeholder
- **Failed load**: Generic file icon

### Avatar Sizes and Fallbacks
| Size | Dimensions | Font size (initials) |
|------|------------|---------------------|
| xs | 24px | 10px |
| sm | 32px | 12px |
| md | 40px | 14px |
| lg | 48px | 16px |
| xl | 64px | 20px |

---

## 8. Accessibility

### Color Contrast Ratios
- **Normal text**: Minimum 4.5:1
- **Large text**: Minimum 3:1
- **UI components**: Minimum 3:1
- **Primary colors tested**: `#CC785C` on white = ~4.5:1

### Focus Indicator Styles
- **Style**: 3px solid outline
- **Color**: `rgba(204, 120, 92, 0.5)` (primary with transparency)
- **Offset**: 2px from element
- **Visible on**: All interactive elements when focused via keyboard

### Touch Target Sizes
- **Minimum size**: 44px x 44px
- **Recommended**: 48px x 48px
- **Spacing between targets**: Minimum 8px

### Screen Reader Considerations
- **Alt text**: Required for all meaningful images
- **ARIA labels**: On icon-only buttons
- **Live regions**: For toast notifications
- **Skip links**: To main content
- **Heading hierarchy**: Proper h1-h6 structure
- **Form labels**: Associated with inputs

### Keyboard Navigation
- **Tab order**: Logical, follows visual order
- **Focus trap**: In modals
- **Escape**: Closes modals, dropdowns
- **Enter/Space**: Activates buttons
- **Arrow keys**: Navigate within components (dropdowns, tabs)

---

## Appendix: CSS Custom Properties Summary

```css
:root {
  /* Colors - Light Theme */
  --color-primary: #CC785C;
  --color-primary-hover: #B86A50;
  --color-accent-purple: #6B5B95;
  --color-accent-teal: #4A9B8C;

  --color-bg-primary: #F5F5F0;
  --color-bg-secondary: #EDEEE8;
  --color-bg-tertiary: #E8E8E2;

  --color-text-primary: #1A1A1A;
  --color-text-secondary: #4A4A4A;
  --color-text-tertiary: #6B6B6B;

  --color-border-primary: #D4D4CE;
  --color-border-input: #C8C8C2;

  --color-success: #4A9B8C;
  --color-warning: #D4A84B;
  --color-error: #C75050;

  /* Typography */
  --font-family-display: 'Tiempos Headline', Georgia, serif;
  --font-family-body: 'Söhne', Helvetica Neue, Arial, sans-serif;
  --font-family-mono: 'Söhne Mono', SF Mono, Monaco, monospace;

  /* Spacing */
  --spacing-unit: 4px;
  --spacing-1: 4px;
  --spacing-2: 8px;
  --spacing-3: 12px;
  --spacing-4: 16px;
  --spacing-6: 24px;
  --spacing-8: 32px;

  /* Borders */
  --radius-sm: 4px;
  --radius-md: 8px;
  --radius-lg: 12px;
  --radius-xl: 16px;
  --radius-pill: 9999px;

  /* Shadows */
  --shadow-sm: 0 1px 2px rgba(0,0,0,0.04), 0 1px 3px rgba(0,0,0,0.06);
  --shadow-md: 0 2px 4px rgba(0,0,0,0.04), 0 4px 8px rgba(0,0,0,0.06);
  --shadow-lg: 0 4px 8px rgba(0,0,0,0.06), 0 8px 16px rgba(0,0,0,0.08);
  --shadow-xl: 0 8px 16px rgba(0,0,0,0.08), 0 16px 32px rgba(0,0,0,0.12);

  /* Motion */
  --duration-fast: 100ms;
  --duration-normal: 200ms;
  --duration-slow: 300ms;
  --ease-default: cubic-bezier(0.4, 0, 0.2, 1);
}

/* Dark Theme Override */
[data-theme="dark"] {
  --color-bg-primary: #2D2A26;
  --color-bg-secondary: #252320;
  --color-bg-tertiary: #363330;

  --color-text-primary: #F5F5F0;
  --color-text-secondary: #C8C8C2;
  --color-text-tertiary: #9A9A94;

  --color-border-primary: #4A4845;
}
```