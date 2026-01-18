# Design System Documentation

## 1. Design & Brand Identity

### Design Philosophy and Guiding Principles
- **Approachable yet professional**: The design balances friendly, whimsical elements with clean, business-oriented interfaces
- **Empowerment-focused**: Visual language emphasizes enabling small businesses to achieve professional results
- **Clarity over complexity**: Clean layouts with generous whitespace prioritize ease of use
- **Consistent personality**: The playful brand character appears throughout without compromising usability

### Visual Style Direction
- **Marketing site**: Bold, expressive, colorful with strong serif typography and hand-drawn illustrations
- **Application**: Clean, functional, minimal with focus on content and task completion
- **Dual personality**: Warm, creative marketing presence paired with professional, efficient application interface

### Overall Mood and Tone
- Friendly and encouraging
- Confident but not intimidating
- Playful with purpose
- Professional yet accessible
- Human and warm

### Brand Personality Expressed Through UI
- Hand-drawn illustrations add warmth and approachability
- Bold color choices (yellow, pink, teal) convey energy and creativity
- Serif typography on marketing adds sophistication and personality
- Clean application UI shows professionalism and reliability
- Mascot (Freddie the chimp) provides consistent brand recognition

### Visual Language Consistency
- Yellow consistently signals primary actions and promotions
- Teal consistently represents interactive/clickable elements in the app
- Illustrations maintain consistent line-weight and artistic style
- Typography pairs are used consistently across contexts

---

## 2. Design Tokens

### Colors

#### Primary Palette
| Name | Hex | Usage |
|------|-----|-------|
| Cavendish (Yellow) | `#FFE01B` | Primary CTA buttons, progress bars, highlights, promotional banners |
| Peppercorn (Dark) | `#241C15` | Primary text, dark headers, footer backgrounds |
| Kale (Teal) | `#007C89` | App primary buttons, links, interactive elements |

#### Secondary/Accent Colors
| Name | Hex | Usage |
|------|-----|-------|
| Lavender Pink | `#F2D2E1` | Marketing section backgrounds |
| Jasper Blue | `#D1E3E8` | Hero backgrounds, selected card states |
| Sage Green | `#D4E9D6` | Success backgrounds, confirmation states |
| Coconut (Cream) | `#FFFDF5` | Page backgrounds, light surfaces |

#### Neutral/Grayscale Scale
| Name | Hex | Usage |
|------|-----|-------|
| White | `#FFFFFF` | Cards, content areas, inputs |
| Gray 50 | `#FAFAFA` | Subtle backgrounds |
| Gray 100 | `#F5F5F5` | Table headers, dividers |
| Gray 200 | `#EEEEEE` | Borders, disabled backgrounds |
| Gray 300 | `#E0E0E0` | Input borders |
| Gray 400 | `#BDBDBD` | Placeholder text, disabled text |
| Gray 500 | `#9E9E9E` | Secondary icons |
| Gray 600 | `#757575` | Secondary text, captions |
| Gray 700 | `#616161` | Body text (muted) |
| Gray 800 | `#424242` | Body text |
| Gray 900 | `#212121` | Headings, primary text |

#### Semantic Colors
| State | Hex | Usage |
|-------|-----|-------|
| Success | `#008040` | Success messages, checkmarks, positive indicators |
| Success Light | `#D4E9D6` | Success alert backgrounds |
| Warning | `#F5A623` | Warning states, caution indicators |
| Warning Light | `#FFF3CD` | Warning alert backgrounds |
| Error | `#D32F2F` | Error states, validation errors |
| Error Light | `#FADCC8` | Error alert backgrounds (peach) |
| Info | `#007C89` | Informational messages, links |

#### Background Colors
| Name | Hex | Usage |
|------|-----|-------|
| Page Background | `#FFFDF5` | Main page background (cream) |
| Card Background | `#FFFFFF` | Card surfaces |
| Modal Overlay | `rgba(0, 0, 0, 0.5)` | Modal backdrop |
| Sidebar Background | `#FFFFFF` | Sidebar panel |
| Header Background | `#FFFDF5` | App header bar |
| Dark Section | `#241C15` | Dark marketing sections, footer |
| Hero Blue | `#C5DDE6` | Light blue hero sections |
| Hero Pink | `#F2D2E1` | Pink marketing sections |
| Hero Yellow | `#FFE01B` | Yellow accent sections |

#### Text Colors
| Name | Hex | Usage |
|------|-----|-------|
| Primary | `#241C15` | Headings, body text |
| Secondary | `#616161` | Secondary text, descriptions |
| Muted | `#9E9E9E` | Placeholder text, hints |
| Disabled | `#BDBDBD` | Disabled states |
| Inverse | `#FFFFFF` | Text on dark backgrounds |
| Link | `#007C89` | Hyperlinks, interactive text |
| Link Hover | `#005F6B` | Hovered links |

#### Border Colors
| Name | Hex | Usage |
|------|-----|-------|
| Default | `#E0E0E0` | Card borders, dividers |
| Input | `#BDBDBD` | Form input borders |
| Focus | `#007C89` | Focused input borders |
| Selected | `#007C89` | Selected card borders |

#### Gradient Definitions
```css
/* Yellow gradient for progress bars */
background: linear-gradient(90deg, #FFE01B 0%, #FFE01B 100%);

/* Dark gradient overlay */
background: linear-gradient(180deg, rgba(36, 28, 21, 0) 0%, rgba(36, 28, 21, 0.8) 100%);
```

---

### Typography

#### Font Families
| Type | Font Family | Fallback Stack |
|------|-------------|----------------|
| Headings (Marketing) | Means Web | Georgia, "Times New Roman", serif |
| Body | Graphik Web | -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif |
| Monospace | "Roboto Mono" | "SF Mono", Monaco, Consolas, monospace |

#### Font Weights
| Weight | Value | Usage |
|--------|-------|-------|
| Regular | 400 | Body text, descriptions |
| Medium | 500 | Button labels, emphasis |
| Semibold | 600 | Subheadings, labels |
| Bold | 700 | Headings, strong emphasis |

#### Type Scale
| Name | Size | Line Height | Weight | Usage |
|------|------|-------------|--------|-------|
| Display XL | 72px / 4.5rem | 1.1 | 700 | Hero headlines (marketing) |
| Display L | 56px / 3.5rem | 1.15 | 700 | Large section headings |
| Display M | 48px / 3rem | 1.2 | 700 | Page titles |
| H1 | 40px / 2.5rem | 1.2 | 700 | Primary headings |
| H2 | 32px / 2rem | 1.25 | 700 | Section headings |
| H3 | 24px / 1.5rem | 1.3 | 600 | Subsection headings |
| H4 | 20px / 1.25rem | 1.4 | 600 | Card titles |
| H5 | 18px / 1.125rem | 1.4 | 600 | Small headings |
| H6 | 16px / 1rem | 1.5 | 600 | Micro headings |
| Body Large | 18px / 1.125rem | 1.6 | 400 | Lead paragraphs |
| Body | 16px / 1rem | 1.5 | 400 | Default body text |
| Body Small | 14px / 0.875rem | 1.5 | 400 | Secondary text |
| Caption | 12px / 0.75rem | 1.4 | 400 | Captions, labels |
| Overline | 11px / 0.6875rem | 1.5 | 600 | Category labels, all-caps |

#### Letter Spacing
| Type | Value |
|------|-------|
| Headings | -0.02em |
| Body | 0 |
| Buttons | 0.02em |
| Overline/Caps | 0.1em |

#### Paragraph Spacing
| Context | Value |
|---------|-------|
| Default paragraph margin | 16px (1rem) |
| Tight spacing | 8px (0.5rem) |
| Loose spacing | 24px (1.5rem) |

#### Text Styles Catalog
```css
/* Marketing Headline */
.headline-marketing {
  font-family: "Means Web", Georgia, serif;
  font-size: 56px;
  font-weight: 700;
  line-height: 1.15;
  letter-spacing: -0.02em;
  color: #241C15;
}

/* App Page Title */
.page-title {
  font-family: "Means Web", Georgia, serif;
  font-size: 40px;
  font-weight: 400;
  line-height: 1.2;
  color: #241C15;
}

/* Section Heading */
.section-heading {
  font-family: "Graphik Web", sans-serif;
  font-size: 24px;
  font-weight: 600;
  line-height: 1.3;
  color: #241C15;
}

/* Body Text */
.body-text {
  font-family: "Graphik Web", sans-serif;
  font-size: 16px;
  font-weight: 400;
  line-height: 1.5;
  color: #241C15;
}

/* Caption */
.caption {
  font-family: "Graphik Web", sans-serif;
  font-size: 12px;
  font-weight: 400;
  line-height: 1.4;
  color: #757575;
}

/* Button Label */
.button-label {
  font-family: "Graphik Web", sans-serif;
  font-size: 16px;
  font-weight: 500;
  line-height: 1;
  letter-spacing: 0.02em;
}
```

---

### Spacing

#### Base Unit
`4px` (0.25rem)

#### Spacing Scale
| Token | Value | Usage |
|-------|-------|-------|
| space-0 | 0px | Reset |
| space-1 | 4px | Tight inline spacing |
| space-2 | 8px | Icon-text gaps, tight padding |
| space-3 | 12px | Small component padding |
| space-4 | 16px | Default padding, paragraph spacing |
| space-5 | 20px | Medium padding |
| space-6 | 24px | Section padding (small) |
| space-8 | 32px | Section padding (medium) |
| space-10 | 40px | Large padding |
| space-12 | 48px | Section margins |
| space-16 | 64px | Large section margins |
| space-20 | 80px | Hero section padding |
| space-24 | 96px | Page section spacing |
| space-32 | 128px | Major section breaks |

#### Component Internal Padding
| Component | Padding |
|-----------|---------|
| Button (small) | 8px 16px |
| Button (medium) | 12px 24px |
| Button (large) | 16px 32px |
| Card | 24px |
| Modal | 32px |
| Input | 12px 16px |
| Badge | 4px 8px |
| Tab | 12px 16px |

#### Layout Margins and Gaps
| Context | Value |
|---------|-------|
| Card grid gap | 24px |
| Form field gap | 24px |
| Sidebar item gap | 4px |
| Header horizontal padding | 24px |
| Page horizontal margin | 24px (mobile), 48px (desktop) |

---

### Effects

#### Shadow Definitions
| Level | Value | Usage |
|-------|-------|-------|
| Elevation 0 | none | Flat elements |
| Elevation 1 | `0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.08)` | Cards, dropdowns |
| Elevation 2 | `0 4px 6px rgba(0,0,0,0.1), 0 2px 4px rgba(0,0,0,0.06)` | Raised cards, popovers |
| Elevation 3 | `0 10px 20px rgba(0,0,0,0.15), 0 3px 6px rgba(0,0,0,0.1)` | Modals, dialogs |
| Elevation 4 | `0 15px 25px rgba(0,0,0,0.15), 0 5px 10px rgba(0,0,0,0.05)` | Floating elements |

#### Blur Effects
| Name | Value | Usage |
|------|-------|-------|
| Modal backdrop | `blur(4px)` | Behind modals |
| Frosted glass | `blur(10px)` | Overlay effects |

#### Opacity Values
| Name | Value | Usage |
|------|-------|-------|
| Disabled | 0.5 | Disabled elements |
| Overlay | 0.5 | Modal overlays |
| Hover | 0.08 | Hover state overlays |
| Muted | 0.6 | Muted text/icons |

---

### Borders

#### Border Widths
| Token | Value | Usage |
|-------|-------|-------|
| border-0 | 0px | No border |
| border-1 | 1px | Default borders |
| border-2 | 2px | Focus rings, emphasis |
| border-3 | 3px | Heavy emphasis |
| border-4 | 4px | Progress bars |

#### Border Radius Scale
| Token | Value | Usage |
|-------|-------|-------|
| radius-none | 0px | Sharp corners |
| radius-sm | 4px | Small inputs, tags |
| radius-md | 8px | Buttons, cards |
| radius-lg | 12px | Large cards, modals |
| radius-xl | 16px | Hero cards |
| radius-2xl | 24px | Large containers |
| radius-pill | 9999px | Pills, rounded buttons |
| radius-circle | 50% | Avatars, circular elements |

#### Border Styles
| Name | Usage |
|------|-------|
| Solid | Default borders |
| Dashed | Empty states, drop zones |
| None | Borderless elements |

---

### Iconography

#### Icon Style
- **Style**: Outlined (linear)
- **Stroke weight**: 1.5px - 2px
- **Line cap**: Round
- **Line join**: Round
- **Visual style**: Clean, geometric, friendly

#### Icon Sizes
| Size | Dimension | Usage |
|------|-----------|-------|
| XS | 12px | Inline indicators |
| SM | 16px | Small buttons, labels |
| MD | 20px | Default icons |
| LG | 24px | Navigation, actions |
| XL | 32px | Feature icons |
| 2XL | 48px | Empty states |

#### Icon Stroke Weights
| Size | Stroke |
|------|--------|
| XS-SM | 1.5px |
| MD-LG | 2px |
| XL+ | 2px |

#### Icon Library
The product uses a custom icon set similar to Heroicons or Phosphor Icons (outlined variant).

---

### Motion & Animation

#### Easing Curves
| Name | Value | Usage |
|------|-------|-------|
| ease-default | `cubic-bezier(0.4, 0, 0.2, 1)` | General transitions |
| ease-in | `cubic-bezier(0.4, 0, 1, 1)` | Exit animations |
| ease-out | `cubic-bezier(0, 0, 0.2, 1)` | Enter animations |
| ease-in-out | `cubic-bezier(0.4, 0, 0.2, 1)` | Symmetric animations |
| ease-spring | `cubic-bezier(0.175, 0.885, 0.32, 1.275)` | Bouncy interactions |

#### Duration Scale
| Token | Value | Usage |
|-------|-------|-------|
| duration-instant | 0ms | Immediate feedback |
| duration-fast | 100ms | Micro-interactions |
| duration-normal | 200ms | Default transitions |
| duration-slow | 300ms | Complex animations |
| duration-slower | 400ms | Page transitions |
| duration-slowest | 500ms | Modal animations |

#### Transition Properties
| Element | Properties | Duration | Easing |
|---------|-----------|----------|--------|
| Button hover | background-color, transform | 150ms | ease-out |
| Link hover | color | 150ms | ease-out |
| Modal enter | opacity, transform | 300ms | ease-out |
| Modal exit | opacity, transform | 200ms | ease-in |
| Dropdown | opacity, transform | 200ms | ease-out |
| Sidebar | width | 200ms | ease-in-out |
| Card hover | box-shadow, transform | 200ms | ease-out |

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
    transform: translateY(10px);
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

/* Spin (for loaders) */
@keyframes spin {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}
```

---

## 3. Components

### Buttons

#### Primary Button (Teal - App)
**Purpose**: Main call-to-action in application interfaces

| Property | Value |
|----------|-------|
| Height | 48px |
| Min-width | 120px |
| Padding | 12px 24px |
| Border radius | 9999px (pill) |
| Background | `#007C89` |
| Text color | `#FFFFFF` |
| Font size | 16px |
| Font weight | 500 |
| Letter spacing | 0.02em |

**States**:
- **Default**: Background `#007C89`
- **Hover**: Background `#006670`, cursor pointer
- **Active/Pressed**: Background `#005560`
- **Focus**: 2px outline offset 2px, outline color `#007C89`
- **Disabled**: Background `#007C89` at 50% opacity, cursor not-allowed
- **Loading**: Text replaced with spinner, background unchanged

#### Primary Button (Yellow - Marketing)
**Purpose**: Main call-to-action on marketing pages

| Property | Value |
|----------|-------|
| Height | 56px |
| Padding | 16px 32px |
| Border radius | 9999px (pill) |
| Background | `#FFE01B` |
| Text color | `#241C15` |
| Font size | 16px |
| Font weight | 500 |

**States**:
- **Default**: Background `#FFE01B`
- **Hover**: Background `#E6C900`, slight scale `transform: scale(1.02)`
- **Active**: Background `#CCB300`

#### Secondary Button (Outline)
**Purpose**: Secondary actions

| Property | Value |
|----------|-------|
| Height | 48px |
| Padding | 12px 24px |
| Border radius | 9999px (pill) |
| Background | transparent |
| Border | 1px solid `#007C89` |
| Text color | `#007C89` |

**States**:
- **Hover**: Background `rgba(0, 124, 137, 0.08)`
- **Active**: Background `rgba(0, 124, 137, 0.12)`
- **Disabled**: Border and text at 50% opacity

#### Tertiary Button (Text/Ghost)
**Purpose**: Low-emphasis actions, Cancel buttons

| Property | Value |
|----------|-------|
| Height | 48px |
| Padding | 12px 24px |
| Background | transparent |
| Text color | `#007C89` |

**States**:
- **Hover**: Text underline, background `rgba(0, 124, 137, 0.04)`
- **Active**: Background `rgba(0, 124, 137, 0.08)`

#### Icon Button
**Purpose**: Actions with icons only

| Property | Value |
|----------|-------|
| Size | 40px x 40px |
| Border radius | 50% |
| Background | transparent |
| Icon size | 20px |
| Icon color | `#616161` |

**States**:
- **Hover**: Background `rgba(0, 0, 0, 0.04)`
- **Active**: Background `rgba(0, 0, 0, 0.08)`

#### Split Button
**Purpose**: Primary action with additional options

| Property | Value |
|----------|-------|
| Height | 48px |
| Border radius | 8px |
| Main button | Teal background |
| Dropdown trigger | Teal background with divider |

---

### Form Inputs

#### Text Input
**Purpose**: Single-line text entry

| Property | Value |
|----------|-------|
| Height | 48px |
| Padding | 12px 16px |
| Border | 1px solid `#BDBDBD` |
| Border radius | 8px |
| Background | `#FFFFFF` |
| Font size | 16px |
| Placeholder color | `#9E9E9E` |

**States**:
- **Default**: Border `#BDBDBD`
- **Hover**: Border `#757575`
- **Focus**: Border `#007C89`, 2px border width
- **Error**: Border `#D32F2F`
- **Disabled**: Background `#F5F5F5`, text at 50% opacity
- **Success**: Green checkmark icon on right

**Anatomy**:
- Label (above): 14px, font-weight 500, margin-bottom 8px
- Helper text (below): 12px, color `#757575`, margin-top 4px
- Required indicator: Asterisk or "Required" text

#### Textarea
**Purpose**: Multi-line text entry

| Property | Value |
|----------|-------|
| Min-height | 120px |
| Padding | 12px 16px |
| Border | 1px solid `#BDBDBD` |
| Border radius | 8px |
| Resize | vertical |
| Line numbers | Optional, left-aligned |

#### Select/Dropdown
**Purpose**: Single selection from options

| Property | Value |
|----------|-------|
| Height | 48px |
| Padding | 12px 16px |
| Border | 1px solid `#BDBDBD` |
| Border radius | 8px |
| Background | `#FFFFFF` |
| Icon | Chevron down, 16px, right-aligned |

**Dropdown Menu**:
- Background: `#FFFFFF`
- Border radius: 8px
- Shadow: Elevation 2
- Item padding: 12px 16px
- Item hover: Background `#F5F5F5`
- Selected: Background `rgba(0, 124, 137, 0.08)`, checkmark icon

#### Checkbox
**Purpose**: Multi-selection or boolean choice

| Property | Value |
|----------|-------|
| Size | 20px x 20px |
| Border | 2px solid `#BDBDBD` |
| Border radius | 4px |
| Background (unchecked) | `#FFFFFF` |
| Background (checked) | `#007C89` |
| Checkmark | White, 2px stroke |

**States**:
- **Unchecked**: White background, gray border
- **Checked**: Teal background, white checkmark
- **Hover**: Border `#757575`
- **Disabled**: 50% opacity

#### Radio Button
**Purpose**: Single selection from group

| Property | Value |
|----------|-------|
| Size | 20px x 20px |
| Border | 2px solid `#BDBDBD` |
| Border radius | 50% |
| Inner dot (selected) | 10px, `#007C89` |

#### Toggle Switch
**Purpose**: On/off binary choice

| Property | Value |
|----------|-------|
| Track width | 44px |
| Track height | 24px |
| Track radius | 12px |
| Thumb size | 20px |
| Track (off) | `#BDBDBD` |
| Track (on) | `#007C89` |
| Thumb | `#FFFFFF` |

---

### Cards

#### Standard Card
**Purpose**: Container for grouped content

| Property | Value |
|----------|-------|
| Padding | 24px |
| Border | 1px solid `#E0E0E0` |
| Border radius | 8px |
| Background | `#FFFFFF` |
| Shadow | None or Elevation 1 |

#### Selection Card (Radio)
**Purpose**: Single-select option cards

| Property | Value |
|----------|-------|
| Padding | 20px |
| Border | 1px solid `#E0E0E0` |
| Border radius | 8px |
| Background | `#FFFFFF` |

**States**:
- **Default**: White background, gray border
- **Hover**: Border `#BDBDBD`
- **Selected**: Background `rgba(0, 124, 137, 0.06)`, border `#007C89`, radio filled

#### Checkbox Card
**Purpose**: Multi-select option cards

Same as Selection Card but with checkbox in corner instead of radio.

#### Feature Card (Marketing)
**Purpose**: Highlight features on marketing pages

| Property | Value |
|----------|-------|
| Padding | 32px |
| Border radius | 16px |
| Background | Various colors (yellow, pink, blue) |
| Image | 1:1 or 4:3 aspect ratio |

---

### Modals/Dialogs

#### Standard Modal
**Purpose**: Focused tasks, confirmations

| Property | Value |
|----------|-------|
| Max-width | 560px |
| Padding | 32px |
| Border radius | 16px |
| Background | `#FFFFFF` |
| Shadow | Elevation 3 |
| Overlay | `rgba(0, 0, 0, 0.5)` |

**Anatomy**:
- Close button: Top-right, 24px X icon
- Title: H3, 24px, margin-bottom 16px
- Content: Body text, margin-bottom 24px
- Actions: Right-aligned, 16px gap between buttons

#### Confirmation Dialog
**Purpose**: Confirm destructive or important actions

| Property | Value |
|----------|-------|
| Max-width | 400px |
| Padding | 24px |
| Button layout | Stacked or side-by-side |

#### Wizard Modal
**Purpose**: Multi-step processes

| Property | Value |
|----------|-------|
| Max-width | 800px |
| Progress bar | Yellow, 4px height, top of modal |
| Step indicator | "STEP X OUT OF Y" text |

---

### Navigation

#### Marketing Header
| Property | Value |
|----------|-------|
| Height | 72px |
| Background | `#FFFFFF` |
| Padding | 0 24px |
| Position | Fixed, top |
| Shadow | Elevation 1 (on scroll) |

**Elements**:
- Logo: Left-aligned
- Nav items: Center, 16px font, 500 weight, 32px gap
- Dropdown trigger: Chevron icon
- Actions: Right-aligned (Search, Language, Phone, Log In, Sign Up)

#### Mega Menu Dropdown
| Property | Value |
|----------|-------|
| Background | `#FFFFFF` |
| Shadow | Elevation 2 |
| Padding | 32px |
| Columns | 2-3 column layout |
| Item icon | 20px, left of text |

#### App Header Bar
| Property | Value |
|----------|-------|
| Height | 64px |
| Background | `#FFFDF5` (cream) |
| Border bottom | 1px solid `#E0E0E0` |
| Logo | Freddie icon, left |
| Actions | Search icon, avatar, right |

#### App Sidebar
| Property | Value |
|----------|-------|
| Width | 256px (expanded), 64px (collapsed) |
| Background | `#FFFFFF` |
| Border right | 1px solid `#E0E0E0` |

**Nav Item**:
- Height: 44px
- Padding: 12px 16px
- Icon: 20px, left
- Text: 14px, 400 weight
- Gap: 12px (icon to text)
- Active: Background `rgba(0, 124, 137, 0.08)`, teal text and icon
- Hover: Background `#F5F5F5`

**Submenu Item**:
- Padding-left: 48px
- Font-size: 14px
- Active indicator: 3px teal left border

#### Tabs
**Purpose**: Content section navigation

| Property | Value |
|----------|-------|
| Height | 48px |
| Tab padding | 12px 16px |
| Font size | 14px |
| Font weight | 500 |
| Active indicator | 2px bottom border, teal |

**States**:
- **Default**: Text `#616161`
- **Hover**: Text `#241C15`
- **Active**: Text `#007C89`, 2px bottom border

#### Breadcrumbs
| Property | Value |
|----------|-------|
| Font size | 14px |
| Separator | ">" or chevron icon |
| Gap | 8px |
| Current page | Font-weight 600 |
| Link color | `#007C89` |

---

### Tables

#### Data Table
| Property | Value |
|----------|-------|
| Border | 1px solid `#E0E0E0` |
| Border radius | 8px |
| Header background | `#F5F5F5` |
| Row height | 52px |
| Cell padding | 12px 16px |

**Header**:
- Font size: 12px
- Font weight: 600
- Text transform: uppercase
- Letter spacing: 0.05em
- Color: `#616161`

**Cell**:
- Font size: 14px
- Color: `#241C15`

**Row Hover**: Background `#FAFAFA`

**Checkbox Column**: 48px width, centered

---

### Badges/Tags

#### Badge
**Purpose**: Status indicators, counts

| Property | Value |
|----------|-------|
| Height | 24px |
| Padding | 4px 8px |
| Border radius | 4px |
| Font size | 12px |
| Font weight | 500 |

**Variants**:
- **Default**: Background `#F5F5F5`, text `#616161`
- **Primary**: Background `#007C89`, text `#FFFFFF`
- **Success**: Background `#D4E9D6`, text `#008040`
- **Warning**: Background `#FFF3CD`, text `#856404`
- **Error**: Background `#FADCC8`, text `#D32F2F`
- **Featured**: Background `#007C89`, text `#FFFFFF`

#### Tag
**Purpose**: Categorization, labels

| Property | Value |
|----------|-------|
| Height | 28px |
| Padding | 4px 12px |
| Border radius | 4px |
| Font size | 13px |
| Border | 1px solid current color |

---

### Alerts/Banners

#### Alert (Inline)
**Purpose**: Contextual feedback messages

| Property | Value |
|----------|-------|
| Padding | 16px |
| Border radius | 8px |
| Border-left | 4px solid (varies by type) |
| Icon | 20px, left-aligned |

**Variants**:
- **Error**: Background `#FADCC8`, border `#D32F2F`
- **Success**: Background `#D4E9D6`, border `#008040`
- **Warning**: Background `#FFF3CD`, border `#F5A623`
- **Info**: Background `#D1E3E8`, border `#007C89`

#### Announcement Banner
**Purpose**: Site-wide announcements

| Property | Value |
|----------|-------|
| Height | 44px |
| Background | `#241C15` |
| Text color | `#FFFFFF` |
| Text size | 14px |
| Link color | `#FFE01B` |
| Position | Fixed, top (above header) |

---

### Progress Indicators

#### Progress Bar
| Property | Value |
|----------|-------|
| Height | 4px (thin), 8px (default) |
| Background | `#E0E0E0` |
| Fill | `#FFE01B` (marketing), `#007C89` (app) |
| Border radius | 4px |

#### Loading Spinner
| Property | Value |
|----------|-------|
| Size | 20px (button), 32px (page) |
| Color | Current color or `#007C89` |
| Animation | Spin, 1s, linear, infinite |

#### Skeleton
| Property | Value |
|----------|-------|
| Background | `#E0E0E0` |
| Animation | Shimmer effect, 1.5s |
| Border radius | Match target element |

---

### Tooltips
| Property | Value |
|----------|-------|
| Max-width | 240px |
| Padding | 8px 12px |
| Background | `#241C15` |
| Text color | `#FFFFFF` |
| Font size | 13px |
| Border radius | 4px |
| Arrow | 6px triangle |

---

### Avatar
| Property | Value |
|----------|-------|
| Sizes | 24px, 32px, 40px, 48px, 64px |
| Border radius | 50% |
| Border | 2px solid `#FFFFFF` |
| Fallback | Initials on colored background |
| Background colors | Rotation of brand colors |

---

### Chat Widget

#### Trigger Button
| Property | Value |
|----------|-------|
| Size | 56px x 56px |
| Border radius | 28px |
| Background | `#241C15` |
| Icon | Chat bubble, white |
| Shadow | Elevation 3 |
| Position | Fixed, bottom-right |

#### Chat Panel
| Property | Value |
|----------|-------|
| Width | 375px |
| Max-height | 600px |
| Border radius | 16px |
| Background | `#FFFFFF` |
| Header | `#241C15`, 56px height |

**Message Bubbles**:
- Bot: Background `#F5F5F5`, left-aligned
- User: Background `#241C15`, text white, right-aligned
- Border radius: 16px
- Padding: 12px 16px
- Max-width: 80%

**Quick Reply Buttons**:
- Border: 1px solid `#241C15`
- Border radius: 16px
- Padding: 8px 16px
- Hover: Background `#F5F5F5`

---

### Feedback Tab
| Property | Value |
|----------|-------|
| Position | Fixed, right edge, vertically centered |
| Width | 32px |
| Height | 100px |
| Background | `#757575` |
| Text | "Feedback", rotated 90deg |
| Border radius | 4px 0 0 4px |

---

### Help FAB
| Property | Value |
|----------|-------|
| Size | 48px x 48px |
| Border radius | 50% |
| Background | `#241C15` |
| Icon | Question mark, white |
| Shadow | Elevation 2 |
| Position | Fixed, bottom-right |

---

## 4. Layout System

### Grid System
| Property | Value |
|----------|-------|
| Type | 12-column grid |
| Gutter | 24px |
| Margin | 24px (mobile), 48px (tablet), 64px (desktop) |

### Container Max-widths
| Breakpoint | Max-width |
|------------|-----------|
| Small | 100% |
| Medium | 768px |
| Large | 1024px |
| XL | 1200px |
| 2XL | 1440px |

### Breakpoints
| Name | Value | Usage |
|------|-------|-------|
| Mobile | 0-639px | Single column |
| Tablet | 640-1023px | 2 columns |
| Desktop | 1024-1279px | Sidebar + content |
| Large | 1280-1535px | Full layout |
| XL | 1536px+ | Max-width constrained |

### Responsive Behavior Rules
- Sidebar collapses to hamburger menu below 1024px
- Card grids: 1 column (mobile), 2 columns (tablet), 3-4 columns (desktop)
- Navigation becomes hamburger menu below 768px
- Typography scales down by ~10-15% on mobile

### Page Structure Templates

#### Marketing Page
```
[Announcement Banner - fixed]
[Header - fixed]
[Hero Section - full-width, colored background]
[Content Sections - max-width container]
[CTA Section - full-width, colored background]
[Footer - full-width, dark background]
```

#### App Page (Dashboard)
```
[App Header - fixed, 64px]
[Sidebar - fixed left, 256px]
[Main Content - fluid, left margin 256px]
  [Page Title]
  [Content Area]
```

#### App Page (Full-width - Campaign Editor)
```
[Editor Header - fixed, includes back, title, actions]
[Main Content - full width]
  [Left Panel - form/settings]
  [Right Panel - preview]
```

### Vertical Rhythm
- Base line-height: 24px (1.5 x 16px)
- Section spacing: 48px, 64px, 96px
- Component spacing: 16px, 24px, 32px

---

## 5. Patterns

### Navigation Patterns

#### Header Behavior
- **Sticky on scroll**: Header becomes fixed after scrolling past hero
- **Shadow on scroll**: Adds Elevation 1 shadow when scrolled
- **Mobile**: Hamburger menu slides in from left

#### Mobile Navigation
- **Trigger**: Hamburger icon (3 horizontal lines)
- **Panel**: Full-height drawer from left
- **Close**: X icon or tap outside
- **Animation**: Slide in, 300ms

#### Tab Navigation Styles
- Underline active indicator
- No background change
- Smooth transition on tab change
- Scroll horizontal on mobile if needed

#### Link Styles
- Default: `#007C89`, no underline
- Hover: Underline
- Visited: Same as default
- Active: Darker shade

### Form Patterns

#### Form Layout
- Labels above inputs
- Single column on mobile
- 2-column on desktop for short fields (first/last name)
- Full-width for email, password
- 24px vertical gap between fields

#### Validation Display
- Inline errors below field
- Error border on input
- Error icon (optional) in input
- Real-time validation on blur
- Success checkmark for valid fields

#### Required Field Indication
- "Required" text after label, or
- Asterisk (*) after label

#### Helper Text
- Position: Below input
- Color: `#757575`
- Size: 12px
- Use for format hints, character counts

### Content Patterns

#### Card Layouts
- Equal height cards in grid
- 24px gap between cards
- Responsive: 1-4 columns based on viewport

#### Empty States
- Centered illustration
- Heading (serif, 24-32px)
- Description text
- Primary action button
- Secondary link (optional)

#### Loading States
- Skeleton screens for content
- Spinner for actions
- Progress bar for multi-step processes

### Feedback Patterns

#### Toast Notifications
- Position: Top-center
- Auto-dismiss: 5 seconds
- Manual dismiss: X icon
- Max 3 stacked
- Animation: Slide down, fade

#### Modal Overlays
- Semi-transparent black (`rgba(0,0,0,0.5)`)
- Click outside to close (optional)
- Escape key to close
- Focus trap inside modal

#### Confirmation Dialogs
- Clear question/statement
- Destructive action in red
- Cancel as secondary button
- Can't be dismissed by clicking outside

---

## 6. Page Templates

### Marketing Homepage
- Announcement banner (optional)
- Navigation header
- Hero section with headline, subhead, CTA, image
- Feature sections (alternating layout)
- Social proof / testimonials
- Pricing preview
- CTA section
- Footer

### App Dashboard
- App header with logo, search, avatar
- Sidebar navigation
- Welcome/onboarding card (for new users)
- Task list / checklist
- Performance metrics cards
- Quick actions

### Settings Page
- Page title
- Tab navigation (Account, Billing, etc.)
- Form sections with headings
- Save/Cancel actions

### Wizard/Onboarding Flow
- Progress bar at top
- Step indicator
- Large heading question
- Selection options (cards or inputs)
- Navigation (Back, Next, Skip)
- Help/support link

---

## 7. Imagery & Media

### Image Aspect Ratios
| Usage | Ratio |
|-------|-------|
| Hero images | 16:9 or custom |
| Feature images | 4:3 or 1:1 |
| Card thumbnails | 16:9 |
| Avatar | 1:1 |
| Integration logos | 1:1, square |

### Image Border Treatments
- Border radius: Matches container (8px, 16px)
- Shadow: Optional Elevation 1
- Border: None typically

### Placeholder/Fallback Styles
- Background: `#F5F5F5`
- Icon: Image placeholder icon, centered
- Text: "No image" (optional)

### Illustration Style
- Hand-drawn, sketchy line work
- Black and white with occasional color accents
- Whimsical, friendly characters
- Consistent line weight: 2-3px

### Avatar Sizes and Fallbacks
| Size | Dimension | Fallback |
|------|-----------|----------|
| XS | 24px | Single initial |
| SM | 32px | Initials |
| MD | 40px | Initials |
| LG | 48px | Initials |
| XL | 64px | Initials |

**Fallback Colors**: Rotate through brand palette for consistency per user.

---

## 8. Accessibility

### Color Contrast Ratios
| Element | Ratio | Status |
|---------|-------|--------|
| Body text on white | 12.6:1 | AAA |
| Link text on white | 4.7:1 | AA |
| White on teal button | 4.6:1 | AA |
| Dark on yellow button | 15:1 | AAA |
| Placeholder text | 3.1:1 | AA (large text only) |

### Focus Indicator Styles
- **Buttons**: 2px outline, offset 2px, color matches button
- **Inputs**: 2px border color change to teal
- **Links**: Dotted underline + slight background
- **Cards**: 2px teal outline

### Touch Target Sizes
| Element | Minimum Size |
|---------|--------------|
| Buttons | 44px x 44px |
| Links (mobile) | 44px tap area |
| Checkboxes/Radio | 44px tap area |
| Icon buttons | 44px x 44px |

### Screen Reader Considerations
- Semantic HTML structure (h1-h6 hierarchy)
- ARIA labels for icon-only buttons
- Form labels properly associated
- Error messages announced
- Modal focus management
- Skip navigation link
- Alt text for images
- Live regions for dynamic content

---

## Appendix: CSS Custom Properties

```css
:root {
  /* Colors */
  --color-primary-yellow: #FFE01B;
  --color-primary-dark: #241C15;
  --color-primary-teal: #007C89;

  --color-bg-cream: #FFFDF5;
  --color-bg-white: #FFFFFF;
  --color-bg-light: #F5F5F5;

  --color-text-primary: #241C15;
  --color-text-secondary: #616161;
  --color-text-muted: #9E9E9E;
  --color-text-inverse: #FFFFFF;

  --color-border: #E0E0E0;
  --color-border-input: #BDBDBD;

  --color-success: #008040;
  --color-error: #D32F2F;
  --color-warning: #F5A623;

  /* Typography */
  --font-serif: "Means Web", Georgia, serif;
  --font-sans: "Graphik Web", -apple-system, sans-serif;

  --text-xs: 0.75rem;
  --text-sm: 0.875rem;
  --text-base: 1rem;
  --text-lg: 1.125rem;
  --text-xl: 1.25rem;
  --text-2xl: 1.5rem;
  --text-3xl: 2rem;
  --text-4xl: 2.5rem;
  --text-5xl: 3rem;

  /* Spacing */
  --space-1: 0.25rem;
  --space-2: 0.5rem;
  --space-3: 0.75rem;
  --space-4: 1rem;
  --space-5: 1.25rem;
  --space-6: 1.5rem;
  --space-8: 2rem;
  --space-10: 2.5rem;
  --space-12: 3rem;
  --space-16: 4rem;

  /* Border Radius */
  --radius-sm: 4px;
  --radius-md: 8px;
  --radius-lg: 12px;
  --radius-xl: 16px;
  --radius-pill: 9999px;
  --radius-circle: 50%;

  /* Shadows */
  --shadow-sm: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.08);
  --shadow-md: 0 4px 6px rgba(0,0,0,0.1), 0 2px 4px rgba(0,0,0,0.06);
  --shadow-lg: 0 10px 20px rgba(0,0,0,0.15), 0 3px 6px rgba(0,0,0,0.1);

  /* Transitions */
  --transition-fast: 150ms ease-out;
  --transition-normal: 200ms ease-out;
  --transition-slow: 300ms ease-out;
}
```