# Design System Documentation

## 1. Design & Brand Identity

### Design Philosophy
- **Minimalist and Clean**: The interface prioritizes content and conversation, with minimal visual clutter
- **Conversational First**: All UI elements support the primary chat interaction paradigm
- **Accessibility**: High contrast ratios, clear typography, and consistent interactive patterns
- **Dual Theme Support**: Full light and dark mode implementations with careful attention to both

### Visual Style Direction
- Modern, professional, and approachable
- Flat design with subtle depth through shadows and layering
- Generous whitespace to improve readability
- Rounded corners throughout for a friendly, accessible feel

### Overall Mood and Tone
- Intelligent but not intimidating
- Professional yet conversational
- Trustworthy and reliable
- Calm and focused

### Brand Personality Expressed Through UI
- Intelligence conveyed through clean typography and organized layouts
- Approachability through rounded corners and generous spacing
- Reliability through consistent patterns and predictable interactions
- Innovation through unique features like voice visualization and canvas editing

### Visual Language Consistency
- Consistent icon style (outlined, 1.5px stroke)
- Unified border radius scale across all components
- Cohesive color palette applied systematically
- Typography hierarchy maintained throughout

---

## 2. Design Tokens

### Colors

#### Primary Palette
| Token | Hex | Usage |
|-------|-----|-------|
| `--primary-black` | `#000000` | Primary buttons, text (light mode) |
| `--primary-white` | `#ffffff` | Primary buttons (dark mode), backgrounds |
| `--accent-purple` | `#5865F2` | Upgrade buttons, premium features |
| `--accent-green` | `#10A37F` | Success states, brand accent |

#### Background Colors
| Token | Light Mode | Dark Mode | Usage |
|-------|------------|-----------|-------|
| `--bg-primary` | `#ffffff` | `#212121` | Main background |
| `--bg-secondary` | `#f4f4f4` | `#2f2f2f` | Sidebar, secondary surfaces |
| `--bg-tertiary` | `#ececec` | `#424242` | Hover states, input backgrounds |
| `--bg-elevated` | `#ffffff` | `#2f2f2f` | Cards, modals, dropdowns |
| `--bg-chat-user` | `#f4f4f4` | `#303030` | User message bubbles |
| `--bg-input` | `#f4f4f4` | `#303030` | Input field background |
| `--bg-overlay` | `rgba(0,0,0,0.5)` | `rgba(0,0,0,0.7)` | Modal overlays |

#### Text Colors
| Token | Light Mode | Dark Mode | Usage |
|-------|------------|-----------|-------|
| `--text-primary` | `#0d0d0d` | `#ececec` | Primary text, headings |
| `--text-secondary` | `#666666` | `#b4b4b4` | Secondary text, descriptions |
| `--text-tertiary` | `#999999` | `#8e8e8e` | Placeholder, muted text |
| `--text-disabled` | `#c5c5c5` | `#6e6e6e` | Disabled states |
| `--text-inverse` | `#ffffff` | `#000000` | Text on primary buttons |
| `--text-link` | `#0066cc` | `#6eb5ff` | Hyperlinks |

#### Border Colors
| Token | Light Mode | Dark Mode | Usage |
|-------|------------|-----------|-------|
| `--border-default` | `#e5e5e5` | `#424242` | Default borders |
| `--border-subtle` | `#f0f0f0` | `#333333` | Subtle dividers |
| `--border-strong` | `#d1d1d1` | `#555555` | Emphasized borders |
| `--border-focus` | `#000000` | `#ffffff` | Focus rings |

#### Semantic Colors
| Token | Hex | Usage |
|-------|-----|-------|
| `--success` | `#10A37F` | Success messages, confirmations |
| `--success-bg` | `#10A37F` | Success toast background |
| `--error` | `#EF4444` | Error states, destructive actions |
| `--error-bg` | `rgba(239,68,68,0.1)` | Error backgrounds |
| `--warning` | `#F59E0B` | Warning states |
| `--info` | `#3B82F6` | Information states |

#### Interactive Colors
| Token | Light Mode | Dark Mode | Usage |
|-------|------------|-----------|-------|
| `--toggle-active` | `#10A37F` | `#10A37F` | Active toggle switches |
| `--toggle-inactive` | `#e5e5e5` | `#424242` | Inactive toggle switches |
| `--button-primary` | `#000000` | `#ffffff` | Primary button background |
| `--button-primary-hover` | `#333333` | `#e5e5e5` | Primary button hover |
| `--button-secondary` | `transparent` | `transparent` | Secondary button |
| `--button-destructive` | `#EF4444` | `#EF4444` | Delete/destructive buttons |

#### Highlight Colors
| Token | Hex | Usage |
|-------|-----|-------|
| `--highlight-yellow` | `#FEF3C7` | Text selection in canvas |
| `--highlight-selection` | `#B4D5FE` | Text selection |

#### Gradient Definitions
```css
/* Voice orb gradient */
--gradient-voice-orb: radial-gradient(circle, #87CEEB 0%, #4A90D9 50%, #2E5A8B 100%);

/* Upgrade button gradient */
--gradient-upgrade: linear-gradient(135deg, #5865F2 0%, #7C3AED 100%);

/* Premium promo card */
--gradient-promo: linear-gradient(135deg, #87CEEB 0%, #4A90D9 100%);
```

### Typography

#### Font Families
```css
--font-primary: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, sans-serif;
--font-mono: 'Söhne Mono', Monaco, 'Andale Mono', 'Ubuntu Mono', monospace;
```

#### Font Weights
| Token | Weight | Usage |
|-------|--------|-------|
| `--font-regular` | 400 | Body text, descriptions |
| `--font-medium` | 500 | UI labels, buttons |
| `--font-semibold` | 600 | Subheadings, emphasis |
| `--font-bold` | 700 | Headings, titles |

#### Type Scale
| Token | Size | Line Height | Usage |
|-------|------|-------------|-------|
| `--text-xs` | 12px | 16px | Captions, timestamps |
| `--text-sm` | 14px | 20px | Secondary text, labels |
| `--text-base` | 16px | 24px | Body text, chat messages |
| `--text-lg` | 18px | 28px | Section headings |
| `--text-xl` | 20px | 28px | Modal titles |
| `--text-2xl` | 24px | 32px | Page headings |
| `--text-3xl` | 30px | 36px | Hero text |
| `--text-4xl` | 36px | 40px | Large display text |

#### Letter Spacing
| Token | Value | Usage |
|-------|-------|-------|
| `--tracking-tight` | -0.02em | Large headings |
| `--tracking-normal` | 0 | Body text |
| `--tracking-wide` | 0.02em | Uppercase labels, buttons |

#### Text Styles Catalog
```css
/* Heading 1 - Page titles */
.h1 {
  font-size: 30px;
  font-weight: 700;
  line-height: 36px;
  letter-spacing: -0.02em;
}

/* Heading 2 - Section headings */
.h2 {
  font-size: 24px;
  font-weight: 600;
  line-height: 32px;
}

/* Heading 3 - Subsections */
.h3 {
  font-size: 20px;
  font-weight: 600;
  line-height: 28px;
}

/* Heading 4 - Card titles */
.h4 {
  font-size: 18px;
  font-weight: 600;
  line-height: 24px;
}

/* Body - Default text */
.body {
  font-size: 16px;
  font-weight: 400;
  line-height: 24px;
}

/* Body Small */
.body-sm {
  font-size: 14px;
  font-weight: 400;
  line-height: 20px;
}

/* Caption */
.caption {
  font-size: 12px;
  font-weight: 400;
  line-height: 16px;
  color: var(--text-secondary);
}

/* Label */
.label {
  font-size: 14px;
  font-weight: 500;
  line-height: 20px;
}

/* Code */
.code {
  font-family: var(--font-mono);
  font-size: 14px;
  line-height: 20px;
}
```

### Spacing

#### Base Unit
`4px` - All spacing values are multiples of 4px

#### Spacing Scale
| Token | Value | Usage |
|-------|-------|-------|
| `--space-0` | 0px | No spacing |
| `--space-1` | 4px | Tight spacing, icon gaps |
| `--space-2` | 8px | Small gaps, button padding |
| `--space-3` | 12px | Medium gaps |
| `--space-4` | 16px | Default padding, gaps |
| `--space-5` | 20px | Component spacing |
| `--space-6` | 24px | Section spacing |
| `--space-8` | 32px | Large section spacing |
| `--space-10` | 40px | Major section breaks |
| `--space-12` | 48px | Page sections |
| `--space-16` | 64px | Major layout spacing |

#### Component Padding Patterns
```css
/* Button padding */
--button-padding-sm: 6px 12px;
--button-padding-md: 8px 16px;
--button-padding-lg: 12px 24px;

/* Input padding */
--input-padding: 12px 16px;

/* Card padding */
--card-padding: 16px;
--card-padding-lg: 24px;

/* Modal padding */
--modal-padding: 24px;

/* Sidebar item padding */
--sidebar-item-padding: 8px 12px;
```

### Effects

#### Shadow Definitions
| Token | Value | Usage |
|-------|-------|-------|
| `--shadow-sm` | `0 1px 2px rgba(0,0,0,0.05)` | Subtle elevation |
| `--shadow-md` | `0 4px 6px rgba(0,0,0,0.07), 0 2px 4px rgba(0,0,0,0.05)` | Cards, dropdowns |
| `--shadow-lg` | `0 10px 15px rgba(0,0,0,0.1), 0 4px 6px rgba(0,0,0,0.05)` | Modals, popovers |
| `--shadow-xl` | `0 20px 25px rgba(0,0,0,0.1), 0 10px 10px rgba(0,0,0,0.04)` | Large modals |

#### Blur Effects
| Token | Value | Usage |
|-------|-------|-------|
| `--blur-sm` | `4px` | Subtle blur |
| `--blur-md` | `8px` | Modal backdrops |
| `--blur-lg` | `16px` | Heavy blur overlays |

#### Opacity Values
| Token | Value | Usage |
|-------|-------|-------|
| `--opacity-disabled` | 0.5 | Disabled elements |
| `--opacity-hover` | 0.8 | Hover states |
| `--opacity-overlay` | 0.5 | Dark overlay |
| `--opacity-muted` | 0.6 | Muted text/elements |

### Borders

#### Border Widths
| Token | Value | Usage |
|-------|-------|-------|
| `--border-width-thin` | 1px | Default borders |
| `--border-width-medium` | 2px | Focus rings, emphasis |
| `--border-width-thick` | 3px | Strong emphasis |

#### Border Radius Scale
| Token | Value | Usage |
|-------|-------|-------|
| `--radius-none` | 0px | Sharp corners |
| `--radius-sm` | 4px | Small elements, badges |
| `--radius-md` | 8px | Buttons, inputs |
| `--radius-lg` | 12px | Cards, containers |
| `--radius-xl` | 16px | Large cards, modals |
| `--radius-2xl` | 24px | Chat input, large elements |
| `--radius-full` | 9999px | Pills, avatars, circles |

### Iconography

#### Icon Style
- **Style**: Outlined (stroke-based)
- **Stroke Weight**: 1.5px - 2px
- **Corner Style**: Rounded
- **Library**: Custom icons, similar to Heroicons/Phosphor style

#### Icon Sizes
| Token | Size | Usage |
|-------|------|-------|
| `--icon-xs` | 12px | Inline indicators |
| `--icon-sm` | 16px | Button icons, small UI |
| `--icon-md` | 20px | Default icons |
| `--icon-lg` | 24px | Navigation, prominent icons |
| `--icon-xl` | 32px | Feature icons |
| `--icon-2xl` | 48px | Hero/empty state icons |

### Motion & Animation

#### Duration Scale
| Token | Value | Usage |
|-------|-------|-------|
| `--duration-instant` | 50ms | Micro-interactions |
| `--duration-fast` | 100ms | Hover states, toggles |
| `--duration-normal` | 200ms | Default transitions |
| `--duration-slow` | 300ms | Modal open/close |
| `--duration-slower` | 500ms | Page transitions |

#### Easing Curves
```css
--ease-default: cubic-bezier(0.4, 0, 0.2, 1);
--ease-in: cubic-bezier(0.4, 0, 1, 1);
--ease-out: cubic-bezier(0, 0, 0.2, 1);
--ease-in-out: cubic-bezier(0.4, 0, 0.2, 1);
--ease-bounce: cubic-bezier(0.68, -0.55, 0.265, 1.55);
```

#### Animation Patterns
```css
/* Fade in */
@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

/* Slide up */
@keyframes slideUp {
  from { transform: translateY(10px); opacity: 0; }
  to { transform: translateY(0); opacity: 1; }
}

/* Scale in (for modals) */
@keyframes scaleIn {
  from { transform: scale(0.95); opacity: 0; }
  to { transform: scale(1); opacity: 1; }
}

/* Pulse (for loading states) */
@keyframes pulse {
  0%, 100% { opacity: 1; }
  50% { opacity: 0.5; }
}

/* Spin (for spinners) */
@keyframes spin {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}

/* Voice orb animation */
@keyframes voiceOrb {
  0%, 100% { transform: scale(1); }
  50% { transform: scale(1.05); }
}
```

---

## 3. Components

### Buttons

#### Primary Button
**Purpose**: Main call-to-action buttons

**Dimensions & Styles**:
```css
/* Default (Medium) */
height: 40px;
padding: 8px 16px;
border-radius: 9999px; /* pill shape */
font-size: 14px;
font-weight: 500;

/* Small */
height: 32px;
padding: 6px 12px;
font-size: 13px;

/* Large */
height: 48px;
padding: 12px 24px;
font-size: 16px;
```

**States**:
| State | Light Mode | Dark Mode |
|-------|------------|-----------|
| Default | bg: `#000000`, text: `#ffffff` | bg: `#ffffff`, text: `#000000` |
| Hover | bg: `#333333` | bg: `#e5e5e5` |
| Active | bg: `#1a1a1a` | bg: `#d5d5d5` |
| Disabled | bg: `#e5e5e5`, text: `#999999` | bg: `#424242`, text: `#6e6e6e` |
| Loading | Shows spinner, text hidden |

#### Secondary Button (Outline)
**Purpose**: Secondary actions

```css
height: 40px;
padding: 8px 16px;
border-radius: 9999px;
border: 1px solid var(--border-default);
background: transparent;
```

**States**:
| State | Light Mode | Dark Mode |
|-------|------------|-----------|
| Default | border: `#e5e5e5`, text: `#0d0d0d` | border: `#424242`, text: `#ececec` |
| Hover | bg: `#f4f4f4` | bg: `#333333` |
| Active | bg: `#e5e5e5` | bg: `#424242` |

#### Destructive Button
**Purpose**: Delete, remove, dangerous actions

```css
/* Outline variant */
border: 1px solid #EF4444;
color: #EF4444;
background: transparent;

/* Filled variant */
background: #EF4444;
color: #ffffff;
```

#### Ghost Button
**Purpose**: Tertiary actions, icon buttons

```css
padding: 8px;
border-radius: 8px;
background: transparent;
```

**States**:
| State | Background |
|-------|------------|
| Default | transparent |
| Hover | `var(--bg-tertiary)` |
| Active | `var(--bg-secondary)` |

#### Icon Button
**Purpose**: Actions with icons only

```css
width: 36px;
height: 36px;
padding: 8px;
border-radius: 8px;
display: flex;
align-items: center;
justify-content: center;
```

#### Upgrade Button
**Purpose**: Premium feature upgrade

```css
background: #5865F2;
color: #ffffff;
border-radius: 9999px;
padding: 8px 16px;

/* With sparkle icon on left */
display: flex;
align-items: center;
gap: 6px;
```

### Inputs

#### Text Input
**Purpose**: Single-line text entry

```css
height: 44px;
padding: 12px 16px;
border-radius: 12px;
border: 1px solid var(--border-default);
background: var(--bg-input);
font-size: 16px;
```

**States**:
| State | Border | Background |
|-------|--------|------------|
| Default | `var(--border-default)` | `var(--bg-input)` |
| Focus | `var(--border-focus)` | `var(--bg-primary)` |
| Error | `#EF4444` | - |
| Disabled | - | opacity: 0.5 |

#### Chat Input (Composer)
**Purpose**: Main message input area

```css
min-height: 52px;
max-height: 200px;
padding: 14px 16px;
border-radius: 24px;
background: var(--bg-input);
border: 1px solid var(--border-default);

/* With toolbar */
padding-bottom: 48px; /* space for toolbar */
```

**Anatomy**:
- Textarea (auto-expanding)
- Toolbar row: [+Attach] [Tools] ... [Mic] [Voice] [Send]
- Placeholder: "Ask anything"
- File attachment previews (when attached)

#### Textarea
**Purpose**: Multi-line text entry

```css
min-height: 100px;
padding: 12px 16px;
border-radius: 12px;
border: 1px solid var(--border-default);
resize: vertical;
```

#### Search Input
**Purpose**: Search functionality

```css
height: 44px;
padding: 12px 16px;
padding-left: 44px; /* space for search icon */
border-radius: 12px;
background: var(--bg-input);
```

**Anatomy**:
- Search icon (left)
- Text input
- Clear button (right, when has value)

#### Toggle Switch
**Purpose**: Binary on/off settings

```css
width: 44px;
height: 24px;
border-radius: 12px;
padding: 2px;
transition: background 200ms;
```

**States**:
| State | Background | Knob Position |
|-------|------------|---------------|
| Off | `#e5e5e5` (light) / `#424242` (dark) | Left |
| On | `#10A37F` | Right |
| Disabled | opacity: 0.5 | - |

**Knob**:
```css
width: 20px;
height: 20px;
border-radius: 10px;
background: #ffffff;
box-shadow: 0 1px 2px rgba(0,0,0,0.1);
```

#### Checkbox
**Purpose**: Multiple selection

```css
width: 18px;
height: 18px;
border-radius: 4px;
border: 2px solid var(--border-default);
```

**States**:
| State | Style |
|-------|-------|
| Unchecked | Empty, border only |
| Checked | bg: `#10A37F`, white checkmark |
| Indeterminate | bg: `#10A37F`, white dash |

#### Radio Button
**Purpose**: Single selection from group

```css
width: 18px;
height: 18px;
border-radius: 9px;
border: 2px solid var(--border-default);
```

**States**:
| State | Style |
|-------|-------|
| Unselected | Empty, border only |
| Selected | Border: `#10A37F`, inner dot |

#### Select/Dropdown
**Purpose**: Choose from predefined options

```css
height: 44px;
padding: 12px 16px;
padding-right: 40px; /* space for chevron */
border-radius: 12px;
border: 1px solid var(--border-default);
```

**Anatomy**:
- Selected value text
- Chevron down icon (right)
- Dropdown menu (on click)

### Cards

#### GPT Card
**Purpose**: Display GPT/bot information

```css
padding: 16px;
border-radius: 12px;
background: var(--bg-elevated);
border: 1px solid var(--border-default);
```

**Anatomy**:
- Avatar (48px, rounded)
- Title (font-weight: 600)
- Description (2 lines, truncated)
- Author/creator info
- Usage count badge

#### Article Card (Citation)
**Purpose**: Display referenced articles/sources

```css
width: 280px;
border-radius: 12px;
overflow: hidden;
background: var(--bg-elevated);
border: 1px solid var(--border-default);
```

**Anatomy**:
- Thumbnail image (aspect-ratio: 16/9)
- Source icon + name
- Title (2 lines)
- Date

#### Pricing Card
**Purpose**: Subscription plan display

```css
padding: 24px;
border-radius: 16px;
background: var(--bg-elevated);
border: 1px solid var(--border-default);
```

**Anatomy**:
- Plan name badge
- Price (large)
- Period ("/month")
- Description
- Feature list with checkmarks
- CTA button

### Modals/Dialogs

#### Standard Modal
**Purpose**: Focused task completion

```css
/* Container */
max-width: 480px;
width: 90vw;
max-height: 90vh;
border-radius: 16px;
background: var(--bg-elevated);
box-shadow: var(--shadow-xl);

/* Padding */
padding: 24px;
```

**Anatomy**:
- Close button (top-right, X icon)
- Title (h2)
- Content area
- Action buttons (bottom-right)

#### Settings Modal
**Purpose**: Application settings

```css
max-width: 720px;
height: 600px;
display: flex;
```

**Anatomy**:
- Left sidebar (200px) with navigation tabs
- Right content area with selected settings
- Close button

#### Confirmation Dialog
**Purpose**: Confirm destructive actions

```css
max-width: 400px;
padding: 24px;
border-radius: 16px;
```

**Anatomy**:
- Title (question format)
- Description text
- Warning/info bullets (optional)
- Cancel + Confirm buttons

#### Share Modal
**Purpose**: Share content to social platforms

```css
max-width: 480px;
padding: 24px;
```

**Anatomy**:
- Title
- Content preview card
- Share buttons row (Link, X, LinkedIn, Reddit)
- "Link copied!" feedback

### Dropdowns/Menus

#### Standard Dropdown Menu
```css
min-width: 200px;
padding: 8px;
border-radius: 12px;
background: var(--bg-elevated);
border: 1px solid var(--border-default);
box-shadow: var(--shadow-lg);
```

**Menu Item**:
```css
padding: 10px 12px;
border-radius: 8px;
display: flex;
align-items: center;
gap: 12px;

/* Hover */
background: var(--bg-tertiary);
```

**Anatomy**:
- Icon (left, 20px)
- Label text
- Keyboard shortcut (right, muted)
- Chevron (for submenus)

#### Model Selector Dropdown
```css
/* Trigger */
display: flex;
align-items: center;
gap: 8px;
padding: 8px 12px;
border-radius: 8px;

/* Menu */
min-width: 280px;
```

**Item Anatomy**:
- Model icon
- Model name
- Description (small, muted)
- Checkmark (if selected)
- "Upgrade" badge (if premium)

### Navigation

#### Sidebar
```css
width: 260px;
height: 100vh;
background: var(--bg-secondary);
padding: 8px;
display: flex;
flex-direction: column;
```

**Sections**:
1. Logo/Brand area
2. New chat button
3. Navigation items (Search, Library, Sora, GPTs)
4. Chat history (scrollable)
5. User profile (bottom)

#### Sidebar Navigation Item
```css
padding: 10px 12px;
border-radius: 8px;
display: flex;
align-items: center;
gap: 12px;
font-size: 14px;
```

**States**:
| State | Style |
|-------|-------|
| Default | transparent |
| Hover | bg: `var(--bg-tertiary)` |
| Active/Selected | bg: `var(--bg-tertiary)`, font-weight: 500 |

#### Chat History Item
```css
padding: 10px 12px;
border-radius: 8px;
font-size: 14px;
overflow: hidden;
text-overflow: ellipsis;
white-space: nowrap;
```

**Context Menu**:
- Rename
- Archive
- Delete

#### Header Bar
```css
height: 56px;
padding: 0 16px;
display: flex;
align-items: center;
justify-content: space-between;
border-bottom: 1px solid var(--border-subtle);
```

**Anatomy**:
- Left: Toggle sidebar, New chat, Model selector
- Center: Title (in canvas view)
- Right: Share, More options

#### Tabs
```css
/* Tab container */
display: flex;
gap: 0;
border-bottom: 1px solid var(--border-default);

/* Tab item */
padding: 12px 16px;
font-size: 14px;
font-weight: 500;
border-bottom: 2px solid transparent;
```

**States**:
| State | Style |
|-------|-------|
| Default | text: `var(--text-secondary)` |
| Hover | text: `var(--text-primary)` |
| Active | text: `var(--text-primary)`, border-bottom: `#000` (light) / `#fff` (dark) |

### Tables

#### Data Table
```css
width: 100%;
border-collapse: collapse;
```

**Header Row**:
```css
th {
  padding: 12px 16px;
  text-align: left;
  font-weight: 600;
  font-size: 14px;
  border-bottom: 1px solid var(--border-default);
  color: var(--text-secondary);
}
```

**Body Row**:
```css
td {
  padding: 12px 16px;
  font-size: 14px;
  border-bottom: 1px solid var(--border-subtle);
}

tr:hover td {
  background: var(--bg-tertiary);
}
```

### Badges/Tags/Chips

#### Badge
**Purpose**: Status indicators, counts

```css
display: inline-flex;
padding: 2px 8px;
border-radius: 9999px;
font-size: 12px;
font-weight: 500;
```

**Variants**:
| Variant | Light Mode | Dark Mode |
|---------|------------|-----------|
| Default | bg: `#f4f4f4`, text: `#666` | bg: `#333`, text: `#b4b4b4` |
| Success | bg: `#d1fae5`, text: `#065f46` | bg: `#064e3b`, text: `#6ee7b7` |
| Error | bg: `#fee2e2`, text: `#991b1b` | bg: `#7f1d1d`, text: `#fca5a5` |
| Pro | bg: `#5865F2`, text: `#fff` | same |

#### Action Chip
**Purpose**: Quick actions, filters

```css
display: inline-flex;
align-items: center;
gap: 8px;
padding: 10px 16px;
border-radius: 9999px;
border: 1px solid var(--border-default);
background: var(--bg-elevated);
font-size: 14px;
```

**States**:
| State | Style |
|-------|-------|
| Default | border, transparent bg |
| Hover | bg: `var(--bg-tertiary)` |
| Selected | bg: `var(--bg-secondary)`, border: darker |

#### Capability Chip
**Purpose**: Feature toggles (Web Search, Code, Canvas, etc.)

```css
display: inline-flex;
align-items: center;
gap: 6px;
padding: 8px 12px;
border-radius: 8px;
border: 1px solid var(--border-default);
```

**Anatomy**:
- Icon (left)
- Label
- Checkbox (right)

### Avatars

#### User Avatar
```css
/* Sizes */
--avatar-xs: 24px;
--avatar-sm: 32px;
--avatar-md: 40px;
--avatar-lg: 48px;
--avatar-xl: 64px;

/* Style */
border-radius: 9999px;
background: linear-gradient(135deg, #ec4899, #8b5cf6, #3b82f6);
display: flex;
align-items: center;
justify-content: center;
color: #ffffff;
font-weight: 600;
```

#### GPT Avatar
```css
width: 40px;
height: 40px;
border-radius: 8px;
overflow: hidden;
```

#### Voice Avatar
```css
/* Large circle with gradient background */
width: 200px;
height: 200px;
border-radius: 100px;
background: var(--gradient-voice-orb);

/* Animated glow effect during voice mode */
animation: voiceOrb 2s ease-in-out infinite;
```

### Tooltips

```css
padding: 8px 12px;
border-radius: 8px;
background: var(--bg-elevated);
color: var(--text-primary);
font-size: 13px;
box-shadow: var(--shadow-md);
max-width: 250px;
```

**Position**: Typically appears above or below trigger element with small arrow.

### Alerts/Banners

#### Inline Alert
```css
padding: 12px 16px;
border-radius: 12px;
display: flex;
align-items: flex-start;
gap: 12px;
```

**Variants**:
| Variant | Background | Border | Icon Color |
|---------|------------|--------|------------|
| Info | `#eff6ff` | `#bfdbfe` | `#3b82f6` |
| Success | `#ecfdf5` | `#a7f3d0` | `#10a37f` |
| Warning | `#fffbeb` | `#fde68a` | `#f59e0b` |
| Error | `#fef2f2` | `#fecaca` | `#ef4444` |

#### Toast Notification
```css
min-width: 300px;
padding: 12px 16px;
border-radius: 12px;
display: flex;
align-items: center;
gap: 12px;
box-shadow: var(--shadow-lg);
```

**Position**: Top-center of viewport

**Success Toast**:
```css
background: #10A37F;
color: #ffffff;
```

**Anatomy**:
- Icon (checkmark for success)
- Message text
- Dismiss button (optional)

### Progress Indicators

#### Linear Progress Bar
```css
/* Track */
height: 4px;
border-radius: 2px;
background: var(--bg-tertiary);
overflow: hidden;

/* Fill */
height: 100%;
background: var(--accent-green);
border-radius: 2px;
transition: width 300ms ease;
```

#### Spinner
```css
width: 20px;
height: 20px;
border: 2px solid var(--border-default);
border-top-color: var(--text-primary);
border-radius: 50%;
animation: spin 1s linear infinite;
```

#### Skeleton Loading
```css
background: linear-gradient(
  90deg,
  var(--bg-tertiary) 0%,
  var(--bg-secondary) 50%,
  var(--bg-tertiary) 100%
);
background-size: 200% 100%;
animation: skeleton 1.5s ease-in-out infinite;
border-radius: 8px;
```

#### Research Progress Card
```css
padding: 16px;
border-radius: 12px;
background: var(--bg-elevated);
border: 1px solid var(--border-default);
```

**Anatomy**:
- Status text ("Starting research")
- Progress bar
- Stop button (square icon)

### Pagination

#### Page Indicator
```css
display: flex;
align-items: center;
gap: 4px;
font-size: 14px;
color: var(--text-secondary);
```

**Format**: `2/2` or dots for simple cases

#### Arrow Navigation
```css
/* Arrow button */
width: 32px;
height: 32px;
border-radius: 8px;
display: flex;
align-items: center;
justify-content: center;
```

### Chat Message Components

#### User Message
```css
max-width: 70%;
margin-left: auto;
padding: 12px 16px;
border-radius: 20px;
background: var(--bg-chat-user);
```

#### Assistant Message
```css
max-width: 100%;
padding: 0;
/* No bubble background, flows with page */
```

#### Voice Message Transcript
```css
padding: 12px 16px;
border-radius: 16px;
background: var(--bg-secondary);
font-style: italic;
```

**Anatomy**:
- Microphone icon
- Transcript text
- Duration (e.g., "00:04")

#### Message Actions Bar
```css
display: flex;
gap: 4px;
margin-top: 8px;
opacity: 0;
transition: opacity 200ms;

/* Visible on message hover */
.message:hover & {
  opacity: 1;
}
```

**Actions**: Copy, Like, Dislike, Read Aloud, Regenerate, Share

#### Citation Badge
```css
display: inline-flex;
align-items: center;
padding: 2px 6px;
border-radius: 4px;
background: var(--bg-secondary);
font-size: 12px;
cursor: pointer;
```

---

## 4. Layout System

### Grid System

#### Container Widths
```css
--container-sm: 640px;
--container-md: 768px;
--container-lg: 1024px;
--container-xl: 1280px;
--container-2xl: 1536px;
```

#### Chat Content Width
```css
max-width: 768px;
margin: 0 auto;
padding: 0 16px;
```

### Breakpoints
| Name | Min Width | Usage |
|------|-----------|-------|
| `sm` | 640px | Small tablets |
| `md` | 768px | Tablets |
| `lg` | 1024px | Small desktops |
| `xl` | 1280px | Standard desktops |
| `2xl` | 1536px | Large screens |

### Page Structure Templates

#### Main Chat Layout
```
┌─────────────────────────────────────────┐
│ Header (56px)                           │
├──────────┬──────────────────────────────┤
│          │                              │
│ Sidebar  │     Chat Content Area        │
│ (260px)  │     (max-width: 768px)       │
│          │                              │
│          ├──────────────────────────────┤
│          │     Input Composer           │
└──────────┴──────────────────────────────┘
```

#### Canvas/Split View Layout
```
┌─────────────────────────────────────────┐
│ Header (56px)                           │
├──────────┬─────────────┬────────────────┤
│          │             │                │
│ Sidebar  │   Chat      │    Canvas      │
│ (260px)  │   (40%)     │    (60%)       │
│          │             │                │
│          ├─────────────┤                │
│          │   Input     │                │
└──────────┴─────────────┴────────────────┘
```

#### Research Mode Layout
```
┌─────────────────────────────────────────┐
│ Header (56px)                           │
├──────────┬─────────────┬────────────────┤
│          │             │  Activity/     │
│ Sidebar  │   Chat      │  Sources       │
│ (260px)  │   (60%)     │  Panel (40%)   │
│          │             │                │
└──────────┴─────────────┴────────────────┘
```

### Vertical Rhythm

#### Section Spacing
```css
/* Between major sections */
margin-bottom: 32px;

/* Between related items */
margin-bottom: 16px;

/* Between tightly coupled items */
margin-bottom: 8px;
```

---

## 5. Patterns

### Navigation Patterns

#### Header Behavior
- Fixed position, always visible
- Contains primary navigation controls
- Model selector accessible from header
- Share/options on right side

#### Sidebar Behavior
- Collapsible (hamburger menu on mobile)
- Hover to expand in collapsed mode
- Scrollable chat history section
- Sticky user profile at bottom

#### Mobile Navigation
- Sidebar becomes overlay/drawer
- Hamburger menu trigger
- Slide-in from left animation

### Form Patterns

#### Label Position
- Labels above inputs
- Helper text below inputs
- Required indicator: none (all fields assumed required unless stated)

#### Validation Display
- Inline errors below field
- Red border on error state
- Error message with icon

#### Input Groups
```css
display: flex;
flex-direction: column;
gap: 16px;
```

### Content Patterns

#### Empty States
```css
/* Center content */
display: flex;
flex-direction: column;
align-items: center;
justify-content: center;
text-align: center;
padding: 48px;

/* Icon */
width: 48px;
height: 48px;
margin-bottom: 16px;
color: var(--text-tertiary);

/* Message */
font-size: 16px;
color: var(--text-secondary);
```

**Example**: "No hidden images" in Library view

#### Loading States
- Skeleton screens for content areas
- Progress bar for research/generation
- Spinner for quick operations
- "Starting research" card with progress

#### Error States
- Inline error messages
- Toast notifications for async errors
- Error pages for fatal errors

### Feedback Patterns

#### Toast Positioning
- Top-center of viewport
- Stacked if multiple
- Auto-dismiss after 3-5 seconds

#### Modal Overlay
```css
position: fixed;
inset: 0;
background: rgba(0, 0, 0, 0.5);
display: flex;
align-items: center;
justify-content: center;
```

#### Confirmation Pattern
1. User triggers action
2. Confirmation modal appears
3. Cancel or Confirm options
4. Success feedback (toast or inline)

---

## 6. Page Templates

### New Chat Page
- Centered greeting: "What's on your mind today?"
- Input composer
- Quick action chips (Summarize, Get advice, Analyze data, etc.)
- Promotional card (optional, for team features)

### Active Chat Page
- Message thread
- Auto-scroll to newest
- Input composer fixed at bottom
- Message actions on hover

### Settings Page
- Modal overlay
- Left sidebar with sections:
  - General
  - Notifications
  - Personalization
  - Connected apps
  - Data controls
  - Security
  - Account
- Content area with relevant controls

### GPT Store Page
- Search bar at top
- Category tabs (All, Personal account workspace)
- GPT list with cards
- "Create" button in header

### Library Page
- Tabs: All, Images, Hidden
- Grid of generated images
- Lightbox for image preview

---

## 7. Imagery & Media

### Image Aspect Ratios
| Usage | Ratio |
|-------|-------|
| Article thumbnails | 16:9 |
| GPT avatars | 1:1 (square) |
| User avatars | 1:1 (circle) |
| Generated images | Various, preserves original |
| Voice avatars | 1:1 (large circle) |

### Image Border Treatments
```css
/* Generated images */
border-radius: 12px;
overflow: hidden;

/* Thumbnails */
border-radius: 8px;

/* Avatars */
border-radius: 50%; /* circular */
/* or */
border-radius: 8px; /* rounded square for GPTs */
```

### Image Placeholder/Fallback
- Gradient background for user avatars
- Default icon for missing GPT images
- Skeleton loading for images loading

### Avatar Sizes
| Context | Size |
|---------|------|
| Chat message | 32px |
| Sidebar user | 32px |
| GPT card | 48px |
| Profile | 64px |
| Voice mode | 200px |

---

## 8. Accessibility

### Color Contrast Ratios
- All text meets WCAG AA standards (4.5:1 for normal text, 3:1 for large text)
- Interactive elements have sufficient contrast
- Both light and dark modes tested for accessibility

### Focus Indicators
```css
/* Default focus ring */
outline: 2px solid var(--border-focus);
outline-offset: 2px;
border-radius: inherit;

/* For buttons */
box-shadow: 0 0 0 2px var(--bg-primary), 0 0 0 4px var(--border-focus);
```

### Touch Targets
- Minimum 44x44px for all interactive elements
- Adequate spacing between touch targets
- Larger targets for primary actions

### Screen Reader Considerations
- Semantic HTML structure
- ARIA labels for icon-only buttons
- Live regions for dynamic content
- Skip links for main content

---

## 9. Code Editor/Canvas

### Syntax Highlighting Theme (Dark Mode)
```css
--code-bg: #1e1e1e;
--code-text: #d4d4d4;
--code-keyword: #569cd6;      /* blue - import, def, class */
--code-string: #ce9178;       /* orange - strings */
--code-number: #b5cea8;       /* light green - numbers */
--code-comment: #6a9955;      /* green - comments */
--code-function: #dcdcaa;     /* yellow - function names */
--code-variable: #9cdcfe;     /* light blue - variables */
--code-operator: #d4d4d4;     /* white - operators */
--code-punctuation: #d4d4d4;  /* white - brackets, etc. */
```

### Line Numbers
```css
padding-right: 16px;
text-align: right;
color: #858585;
user-select: none;
min-width: 40px;
```

### Code Canvas Panel
```css
/* Panel header */
height: 48px;
padding: 0 16px;
display: flex;
align-items: center;
justify-content: space-between;
border-bottom: 1px solid var(--border-default);

/* Title dropdown in header */
/* Action buttons: History, Undo, Redo, Copy, Download, Share, Run */

/* Code area */
padding: 16px;
font-family: var(--font-mono);
font-size: 14px;
line-height: 20px;
overflow: auto;

/* Console panel */
height: 100px;
border-top: 1px solid var(--border-default);
background: var(--bg-secondary);
```

### Document Canvas Panel
```css
/* For text documents */
padding: 48px;
max-width: 720px;
margin: 0 auto;
font-size: 16px;
line-height: 1.6;
```

### Canvas Text Selection
```css
/* Yellow highlight for selected text */
background: #FEF3C7;
/* Shows inline formatting toolbar: B, I, Aa */
```

---

## 10. Voice Mode

### Voice Orb
```css
width: 200px;
height: 200px;
border-radius: 100px;
background: radial-gradient(
  circle at 30% 30%,
  #87CEEB 0%,
  #4A90D9 40%,
  #2E5A8B 100%
);
animation: voiceOrb 2s ease-in-out infinite;
```

### Voice Mode Controls
```css
/* Container */
position: fixed;
bottom: 48px;
left: 50%;
transform: translateX(-50%);
display: flex;
gap: 16px;

/* Control buttons */
width: 56px;
height: 56px;
border-radius: 28px;
background: var(--bg-elevated);
box-shadow: var(--shadow-lg);
```

**Buttons**: Microphone, End/Close

### Voice Selection Carousel
```css
/* Voice option */
display: flex;
flex-direction: column;
align-items: center;
gap: 8px;

/* Avatar */
width: 120px;
height: 120px;
border-radius: 60px;

/* Name */
font-size: 16px;
font-weight: 500;

/* Description */
font-size: 14px;
color: var(--text-secondary);
```

**Navigation**: Left/right arrows for carousel

---

## 11. Special Components

### Image Generation Style Picker
```css
/* Grid */
display: grid;
grid-template-columns: repeat(3, 1fr);
gap: 16px;

/* Style option */
display: flex;
flex-direction: column;
align-items: center;
gap: 8px;

/* Preview image */
width: 80px;
height: 80px;
border-radius: 40px;
overflow: hidden;

/* Label */
font-size: 13px;
```

**Styles include**: Cyberpunk, Anime, Dramatic Headshot, Coloring Book, Photo Shoot, Retro Cartoon, 80s Glam, Art Nouveau, Synthwave

### Feedback Component (In-chat)
```css
/* "Is this helpful so far?" card */
padding: 12px 16px;
border-radius: 12px;
background: var(--bg-secondary);
display: flex;
align-items: center;
gap: 12px;
```

### Memory/Saved Context Indicator
```css
/* Inline indicator */
display: flex;
align-items: center;
gap: 8px;
color: var(--text-secondary);
font-size: 14px;

/* Flag icon + "Updated saved memory" text */
```

### Research Panel (Deep Research)
```css
/* Panel header tabs */
display: flex;
gap: 0;
border-bottom: 1px solid var(--border-default);

/* Tab: Activity | Sources */

/* Activity content */
/* List of status updates with icons */

/* Sources content */
/* List of source cards with favicons */
```

---

## 12. Responsive Behavior

### Sidebar
- Desktop (>1024px): Always visible, 260px wide
- Tablet (768-1024px): Collapsible, icon-only mode
- Mobile (<768px): Hidden, overlay drawer

### Chat Width
- Desktop: max-width 768px, centered
- Mobile: Full width with 16px padding

### Canvas/Split View
- Desktop: Side-by-side split
- Tablet: Stacked or sheet overlay
- Mobile: Full-screen canvas, back navigation

### Input Composer
- Desktop: Fixed width matching content
- Mobile: Full width, sticky bottom

### Typography Scale
- Desktop: Full scale as specified
- Mobile: Slightly reduced (90-95% of desktop)

---

## 13. Additional Components (Extended Analysis)

### Promotional Modals

#### Study and Learn Modal
**Purpose**: Promote educational features

```css
/* Modal container */
max-width: 500px;
border-radius: 16px;
overflow: hidden;

/* Gradient header */
background: linear-gradient(135deg, #87CEEB 0%, #FFB6C1 50%, #98FB98 100%);
padding: 48px 24px;
position: relative;

/* Close button (X) */
position: absolute;
top: 16px;
right: 16px;

/* Quick action buttons in header */
display: flex;
flex-direction: column;
gap: 12px;
```

**Anatomy**:
- Gradient header with decorative shapes
- Quick action buttons ("Hey Chat!", "Help me with my homework")
- Title ("Study and Learn")
- Subtitle description
- Feature list with icons (homework help, prep for tests, explore subjects)
- CTA button ("Try it now")

#### Advanced Voice Mode Preview Modal
```css
/* Feature list */
display: flex;
flex-direction: column;
gap: 24px;
padding: 24px;

/* Feature item */
display: flex;
gap: 16px;
align-items: flex-start;

/* Icon container */
width: 40px;
height: 40px;
display: flex;
align-items: center;
justify-content: center;
```

**Features displayed**:
- Free monthly preview
- Natural conversations
- Personalized to you
- You're in control

**Footer**: Disclaimer text + Continue button

#### Temporary Chat Modal
**Purpose**: Explain temporary/incognito chat mode

```css
max-width: 480px;
padding: 24px;
border-radius: 16px;
```

**Anatomy**:
- Title: "Temporary Chat"
- Feature list with icons:
  - "Not in history" (clock icon)
  - "No model training" (settings icon)
  - "Memory off" (document icon)
- Continue button

### Permission & Confirmation Dialogs

#### GPT Permission Request
**Purpose**: Third-party GPT requesting external access

```css
/* Inline in chat */
padding: 12px 16px;
border-radius: 12px;
background: var(--bg-secondary);
```

**Anatomy**:
- Text: "[GPT name] wants to talk to [domain]"
- Three button options: Allow | Always Allow | Decline
- Warning text: "Only allow sites you trust."
- Standard message actions below

#### Delete Account Confirmation
**Purpose**: Multi-step account deletion confirmation

```css
max-width: 480px;
padding: 24px;

/* Warning list */
list-style: disc;
padding-left: 20px;
margin-bottom: 24px;
```

**Anatomy**:
- Title: "Delete account - are you sure?"
- Warning bullets explaining consequences
- Email input field (pre-filled, for confirmation)
- "DELETE" text input (type confirmation)
- Red destructive button: "Permanently delete my account" with warning icon

#### Clear Memory Confirmation
```css
/* Appears over saved memories panel */
padding: 24px;
border-radius: 16px;
```

**Anatomy**:
- Title: "Are you sure?"
- Warning text about memory deletion
- "Learn more" link
- Cancel + "Clear memory" (red) buttons

#### Canvas Close Confirmation
**Purpose**: Unsaved changes warning

```css
padding: 16px 24px;
border-radius: 12px;
```

**Anatomy**:
- Title: "Are you sure you want to close?"
- Two buttons: "Don't save and close" | "Save to chat"

### Feedback Components

#### Thumbs Down Feedback Modal
**Purpose**: Collect detailed feedback after negative rating

```css
max-width: 520px;
padding: 24px;

/* Chip grid */
display: flex;
flex-wrap: wrap;
gap: 8px;
margin-bottom: 16px;
```

**Feedback chips**:
- "Shouldn't have searched the web"
- "Don't like the sources it cited"
- "Shouldn't have used Memory"
- "Don't like the personality"
- "Don't like the style"
- "Not factually correct"
- "Didn't fully follow instructions"
- "Refused when it shouldn't have"
- "Being lazy"
- "Unsafe or problematic"
- "Biased"
- "Other"

**Additional elements**:
- Text input for custom feedback
- Privacy notice
- Submit button

#### Inline Quick Feedback
**Purpose**: Quick feedback chips that appear inline after thumbs down

```css
padding: 16px;
border-radius: 12px;
background: var(--bg-secondary);
```

**Anatomy**:
- "Tell us more:" label
- Horizontal chip row (dismissible with X)
- "More..." chip to expand options

#### Feedback Confirmation
```css
/* Inline message */
padding: 12px 16px;
border-radius: 12px;
background: var(--bg-secondary);
display: inline-block;
```

**Text**: "Thanks for your feedback!"

### Source Citations

#### Inline Source Citation Chip
**Purpose**: Embedded domain references in research content

```css
display: inline-flex;
align-items: center;
gap: 4px;
padding: 2px 8px;
border-radius: 4px;
background: var(--bg-secondary);
font-size: 12px;
vertical-align: middle;
```

**Anatomy**:
- Favicon (optional)
- Domain name (e.g., "britannica.com", "iwm.org.uk")

#### Source Citation Popover
**Purpose**: Expandable citation preview

```css
width: 320px;
padding: 16px;
border-radius: 12px;
background: var(--bg-elevated);
box-shadow: var(--shadow-lg);
```

**Anatomy**:
- Navigation arrows (←/→) with pagination (1/16)
- Source favicon + name
- Article title (linked)
- Date
- Preview text (truncated)

#### All Sources Row
**Purpose**: Show all cited sources in a row

```css
display: flex;
gap: 8px;
flex-wrap: wrap;
padding: 12px 0;
```

**Label**: "All Sources"
**Items**: Domain chips with favicons

### Deep Research Components

#### Research Progress Card (Extended)
```css
padding: 16px;
border-radius: 12px;
border: 1px solid var(--border-default);
```

**Anatomy**:
- Status text: "Reading more from [domain]"
- Progress bar with animated fill
- Source count badge: "5 sources"
- Stop button (square icon)

#### Research Activity Panel
**Purpose**: Show research thinking process

```css
/* Panel in split view */
width: 40%;
border-left: 1px solid var(--border-default);
```

**Tabs**: Activity | 16 Sources

**Activity Items**:
```css
display: flex;
gap: 12px;
padding: 12px 0;
border-bottom: 1px solid var(--border-subtle);
```

Each item shows:
- ChatGPT avatar icon
- Thinking/action text
- "Read [domain]" links

**Status indicators**:
- "Thinking..."
- "Searched for [query]"
- "Read more from [domain]"

#### Citations Panel
**Purpose**: List all research sources

```css
/* In Sources tab */
display: flex;
flex-direction: column;
gap: 12px;
padding: 16px;
```

**Citation Item**:
- Favicon + domain
- Article title
- Preview text (3 lines)

### Canvas Components (Extended)

#### Canvas Export Dropdown
```css
min-width: 220px;
padding: 8px;
border-radius: 12px;
```

**Options**:
- PDF Document (.pdf)
- Microsoft Word Document (.docx)
- Markdown Document (.md)

#### Canvas Rename Input
```css
/* In header, inline editing */
background: var(--bg-input);
border: 1px solid var(--border-focus);
border-radius: 8px;
padding: 4px 12px;
font-size: 16px;
```

#### Canvas Edit History Button
```css
display: inline-flex;
align-items: center;
gap: 6px;
padding: 6px 12px;
border-radius: 9999px;
background: var(--bg-secondary);
font-size: 14px;
```

**Anatomy**:
- Text: "12 more edits"
- Up arrow icon (↑)

#### Canvas Suggestion Popover
**Purpose**: AI suggestion on selected text

```css
padding: 12px 16px;
border-radius: 12px;
background: var(--bg-elevated);
box-shadow: var(--shadow-lg);
max-width: 280px;
```

**Anatomy**:
- ChatGPT logo + "ChatGPT" label
- Suggestion text
- "Apply" button
- Close button (X)

**Selected text highlight**: Yellow background (`#FEF3C7`)

### GPT Store Components

#### GPT Store Page Header
```css
text-align: center;
padding: 48px 24px;
```

**Elements**:
- Title: "GPTs"
- Subtitle description
- Search input with "No results found" empty state
- "+ Create" button (top right)

#### Category Tabs
```css
display: flex;
gap: 0;
overflow-x: auto;
border-bottom: 1px solid var(--border-default);

/* Right scroll indicator */
/* Arrow button when more tabs available */
```

**Categories**:
Top Picks, Writing, Productivity, Research & Analysis, Education, Lifestyle, DALL-E, Programming

#### Featured GPTs Section
```css
/* Section header */
margin-bottom: 16px;

/* Title + subtitle */
.title { font-size: 24px; font-weight: 600; }
.subtitle { font-size: 14px; color: var(--text-secondary); }

/* Grid */
display: grid;
grid-template-columns: repeat(2, 1fr);
gap: 16px;
```

#### GPT Detail Modal (Extended)
```css
max-width: 600px;
padding: 24px;
```

**Sections**:
1. Capabilities checklist (checkmarks):
   - DALL·E Images
   - Code Interpreter & Data Analysis
   - Web Search
   - Canvas
   - Actions

2. Ratings section:
   ```css
   /* Star rating bars */
   display: flex;
   flex-direction: column;
   gap: 8px;

   /* Rating row */
   display: flex;
   align-items: center;
   gap: 8px;

   /* Star icon */
   color: #10A37F;

   /* Progress bar */
   flex: 1;
   height: 8px;
   background: #10A37F;
   border-radius: 4px;
   ```

3. "More by [creator]" section with GPT cards

4. "Start Chat" CTA button

### Voice Mode Components (Extended)

#### Voice Selection Light Mode
```css
/* Full page voice selection */
text-align: center;
padding: 48px;
background: var(--bg-primary);
```

**Elements**:
- Title: "Choose a voice"
- Carousel with voice avatars
- Navigation arrows
- Voice name + personality description
- "Start new chat" primary button
- "Cancel" text link

**Voice personalities**:
- Cove: "Composed and direct"
- Breeze: "Animated and earnest"
- Maple: "Cheerful and candid"

#### Voice Mode Tooltip
```css
padding: 8px 12px;
border-radius: 8px;
background: var(--bg-elevated);
font-size: 13px;
```

**Shows**: "Turn off microphone" + device name (e.g., "MacBook Pro Microphone (Built-in)")

#### Voice Chat End Controls
```css
/* Bottom center of voice mode */
position: fixed;
bottom: 48px;
left: 50%;
transform: translateX(-50%);

/* End button with label */
display: flex;
flex-direction: column;
align-items: center;
gap: 8px;
```

**Elements**:
- "End" label
- Microphone button
- Close (X) button

### Notification & Banner Components

#### Archived Chat Banner
```css
display: flex;
align-items: center;
justify-content: space-between;
padding: 12px 16px;
background: var(--bg-secondary);
border-radius: 12px;
margin-bottom: 16px;
```

**Anatomy**:
- Text: "You can view archived chats in Settings"
- Dismiss button (X)

#### Link Copied Toast (Green)
```css
padding: 12px 16px;
border-radius: 9999px;
background: #10A37F;
color: #ffffff;
display: flex;
align-items: center;
gap: 8px;
```

**Anatomy**:
- Checkmark icon
- "Link copied!" text

#### Share Audio Warning Banner
```css
padding: 12px 16px;
border-radius: 8px;
background: #EF4444;
color: #ffffff;
```

**Text**: "Sharing conversations with audio is not yet supported"

### Content Display Components

#### TL;DR Summary Table
```css
width: 100%;
border-collapse: collapse;

/* Header row */
th {
  text-align: left;
  padding: 12px 16px;
  font-weight: 600;
  border-bottom: 1px solid var(--border-default);
}

/* Body row */
td {
  padding: 12px 16px;
  vertical-align: top;
}
```

**Columns**: "What I Can Do" | "How to Use It Best"

#### Related Articles Grid
```css
display: grid;
grid-template-columns: repeat(3, 1fr);
gap: 16px;
margin-top: 24px;
```

**Article Card**:
```css
border-radius: 12px;
overflow: hidden;
border: 1px solid var(--border-default);

/* Thumbnail */
aspect-ratio: 16/9;
background-size: cover;

/* Content */
padding: 12px;

/* Source row */
display: flex;
align-items: center;
gap: 8px;
font-size: 12px;
color: var(--text-secondary);

/* Title */
font-size: 14px;
font-weight: 500;
margin-top: 8px;
display: -webkit-box;
-webkit-line-clamp: 2;
overflow: hidden;

/* Date */
font-size: 12px;
color: var(--text-tertiary);
margin-top: 4px;
```

### Settings Components (Extended)

#### Notifications Settings
```css
/* Section */
margin-bottom: 24px;

/* Row */
display: flex;
justify-content: space-between;
align-items: flex-start;
padding: 16px 0;
border-bottom: 1px solid var(--border-subtle);
```

**Elements per row**:
- Label + description
- Dropdown (Push / Email / Push, Email)

**Dropdown options**:
- Push (toggle)
- Email (toggle)

#### Account Settings - Builder Profile
```css
/* Info banner */
padding: 16px;
border-radius: 12px;
background: var(--bg-secondary);
display: flex;
gap: 12px;
align-items: flex-start;
margin-bottom: 24px;
```

**Banner content**: Verification info with info icon

**Links section**:
- LinkedIn, GitHub, X with "Add" buttons

**Email section**:
- Email display
- "Receive feedback emails" checkbox

#### Model Improvement Settings (Nested Modal)
```css
max-width: 480px;
padding: 24px;
```

**Sections**:
1. "Improve the model for everyone" - Toggle switch (green when on)
2. "Voice mode" subsection:
   - "Include your audio recordings" - Toggle
   - "Include your video recordings" - Toggle
   - Description text
3. "Done" button

### Model Selector (Extended)

#### Model Options
```css
/* Dropdown menu */
min-width: 280px;
padding: 8px;
```

**Options**:
- **Auto** - Automatic model selection
- **GPT-4o** - "Great for most tasks"
- **o4-mini** - "Fastest at advanced reasoning"
- **GPT-4.1-mini** - "Faster for everyday tasks"

**Divider**

**Additional actions**:
- "Try again" with GPT-4o (refresh icon)
- "Search the web" (globe icon)

#### ChatGPT Plus Upsell Row
```css
display: flex;
align-items: center;
justify-content: space-between;
padding: 12px;
```

**Elements**:
- Sparkle icon + "ChatGPT Plus"
- "Our smartest model & more"
- "Upgrade" button (purple)

### Message Components (Extended)

#### Voice Transcription Message
```css
/* User message with voice indicator */
padding: 12px 16px;
border-radius: 20px;
background: var(--bg-chat-user);
font-style: italic;
```

**Anatomy**:
- Transcribed text in quotes
- Microphone icon + duration (e.g., "00:04")

#### Updated Memory Indicator
```css
display: flex;
align-items: center;
gap: 8px;
color: var(--text-secondary);
font-size: 14px;
margin-bottom: 8px;
```

**Anatomy**:
- Flag/note icon
- "Updated saved memory" text

#### Message Pagination
```css
display: flex;
align-items: center;
gap: 4px;
```

**Format**: `< 2/2 >` with left/right arrows

---

## Appendix: Component State Matrix

### Button States
| Component | Default | Hover | Active | Focus | Disabled | Loading |
|-----------|---------|-------|--------|-------|----------|---------|
| Primary | bg-black | bg-gray-800 | bg-gray-900 | ring | opacity-50 | spinner |
| Secondary | border | bg-gray-100 | bg-gray-200 | ring | opacity-50 | spinner |
| Destructive | border-red | bg-red-50 | bg-red-100 | ring-red | opacity-50 | spinner |
| Ghost | transparent | bg-gray-100 | bg-gray-200 | ring | opacity-50 | - |

### Input States
| Component | Default | Focus | Error | Disabled |
|-----------|---------|-------|-------|----------|
| Text Input | border-gray | border-black | border-red | opacity-50 |
| Textarea | border-gray | border-black | border-red | opacity-50 |
| Select | border-gray | border-black | border-red | opacity-50 |
| Toggle | bg-gray | - | - | opacity-50 |
| Checkbox | border-gray | ring | border-red | opacity-50 |

### Interactive Element States
| Component | Default | Hover | Active | Selected |
|-----------|---------|-------|--------|----------|
| Menu Item | transparent | bg-gray | bg-gray-dark | bg-gray + check |
| Tab | text-gray | text-black | - | text-black + border |
| Chip | border | bg-gray | - | bg-filled |
| Card | border | shadow-md | - | border-primary |
