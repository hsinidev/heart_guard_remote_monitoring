---
name: Clinical Vigilance
colors:
  surface: '#f5fafc'
  surface-dim: '#d6dbdd'
  surface-bright: '#f5fafc'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eff4f6'
  surface-container: '#eaeff1'
  surface-container-high: '#e4e9eb'
  surface-container-highest: '#dee3e5'
  on-surface: '#171c1e'
  on-surface-variant: '#5d3f3d'
  inverse-surface: '#2c3133'
  inverse-on-surface: '#ecf1f3'
  outline: '#926e6c'
  outline-variant: '#e7bcba'
  surface-tint: '#bf0022'
  primary: '#ac001e'
  on-primary: '#ffffff'
  primary-container: '#d90429'
  on-primary-container: '#ffeae8'
  inverse-primary: '#ffb3af'
  secondary: '#5b5d74'
  on-secondary: '#ffffff'
  secondary-container: '#ddddf9'
  on-secondary-container: '#5f6178'
  tertiary: '#495567'
  on-tertiary: '#ffffff'
  tertiary-container: '#616d81'
  on-tertiary-container: '#e8efff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdad7'
  primary-fixed-dim: '#ffb3af'
  on-primary-fixed: '#410005'
  on-primary-fixed-variant: '#930018'
  secondary-fixed: '#e0e0fc'
  secondary-fixed-dim: '#c4c4df'
  on-secondary-fixed: '#181a2e'
  on-secondary-fixed-variant: '#43455b'
  tertiary-fixed: '#d7e3fa'
  tertiary-fixed-dim: '#bbc7dd'
  on-tertiary-fixed: '#101c2c'
  on-tertiary-fixed-variant: '#3c475a'
  background: '#f5fafc'
  on-background: '#171c1e'
  surface-variant: '#dee3e5'
typography:
  display-critical:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 52px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
  data-mono:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '500'
    lineHeight: 24px
    letterSpacing: -0.01em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 12px
  md: 24px
  lg: 40px
  xl: 64px
  margin-mobile: 16px
  gutter-mobile: 12px
---

## Brand & Style

The design system is engineered for the high-stakes environment of remote cardiac monitoring. The brand personality is **Vigilant, Authoritative, and Precise**. It balances the clinical coldness of medical equipment with the urgent responsiveness required for life-saving interventions.

The visual style is **Corporate / Modern** with a lean toward **Minimalism**. Every pixel serves a functional purpose; there is no room for decorative clutter. The UI mimics high-fidelity medical instrument displays—clean, high-contrast, and strictly organized. The "Urgent & Professional" aesthetic is achieved through the tension between a calm, stable Slate foundation and the sharp, piercing presence of Signal Red for critical data points. 

Mobile-first constraints dictate a layout that prioritizes thumb-reach for emergency actions and ultra-legible data visualizations that remain clear even under stress or in low-light conditions.

## Colors

The palette is restricted to three core pillars to ensure cognitive load remains low during critical events. 

- **Signal Red (#D90429):** Reserved exclusively for alerts, critical heart rate fluctuations, and primary emergency actions. It must be used sparingly to maintain its "alarm" psychological impact.
- **Slate (#2B2D42):** Used for deep backgrounds, primary navigation, and stable data points. It provides the "professional stability" and high contrast required for the Silk White surfaces.
- **Silk White (#EDF2F4):** The primary surface color. It represents a sterile, clean clinical environment, providing a neutral stage for data to live on.

Additional shades of Slate are used for subtle borders and secondary text, ensuring that the hierarchy remains clear without introducing distracting new hues.

## Typography

This design system utilizes **Inter** for all applications. Inter’s tall x-height and tabular num features make it ideal for mission-critical medical data where mistaking a '3' for an '8' is not an option.

- **Display & Headlines:** Used for real-time BPM and patient names. Heavy weights ensure immediate recognition.
- **Label Caps:** Used for metadata (e.g., "LAST SYNC," "DEVICE ID") to differentiate instructional text from live patient data.
- **Data Mono:** While Inter is a sans-serif, its numerical characters are highly legible and should be set with "tnum" (tabular figures) features enabled for fluctuating heart rate displays to prevent horizontal jitter during "Pulse" animations.

## Layout & Spacing

The layout utilizes a **fluid grid** optimized for mobile devices, based on an **8px rhythmic scale**. 

On mobile, a 4-column grid with 16px side margins is standard. In "Emergency Mode," margins compress to 12px to maximize the visibility of waveforms and critical metrics. 

Spacing is used to group related physiological data. Components like heart rate graphs and oxygen saturation levels are separated by `md` (24px) spacing, while internal labels within those components use `xs` (4px) or `sm` (12px) to maintain a tight, instrumental feel.

## Elevation & Depth

To maintain a "clinical" and "precise" feel, this design system avoids heavy, fuzzy shadows which can feel "dreamy" or imprecise. Instead, it uses **Tonal Layers** and **Low-Contrast Outlines**.

- **Level 0 (Floor):** Silk White (#EDF2F4) for the main application background.
- **Level 1 (Cards):** Pure White (#FFFFFF) surfaces with a 1px Slate (#2B2D42) border at 10% opacity.
- **Level 2 (Alerts/Modals):** Subtle, crisp shadows (4px offset, 8px blur, 5% Slate opacity) to lift critical notifications above the primary data stream.

Depth is also conveyed through the "Pulse" animation—a soft, concentric ring that radiates from critical data points (like heart rate) in Signal Red, indicating active monitoring.

## Shapes

The shape language is **Soft (0.25rem / 4px)**. This creates a professional, "tool-like" appearance that is more approachable than sharp corners but more serious than highly rounded "consumer" apps.

- **Buttons & Inputs:** Use the standard 4px radius.
- **Status Pills:** Use a fully rounded/pill shape to distinguish them as non-interactive status indicators.
- **Data Containers:** Large cards use `rounded-lg` (8px) to frame complex information like EKG waveforms, providing a subtle "enclosure" feel that suggests the data is being safely contained and monitored.

## Components

### Buttons
- **Action Primary:** Slate (#2B2D42) background with Silk White text. High-contrast, stable.
- **Critical Alert:** Signal Red (#D90429) with white text. Reserved for "Call Emergency" or "Stop Monitoring."
- **Ghost/Secondary:** 1px Slate border (20% opacity) for routine actions like "View History."

### Cards (Data Monitors)
Clinical cards feature a top-aligned `Label Caps` title. The primary metric (e.g., 72 BPM) is centered in `display-critical`. If the state is "Alert," the card border thickens to 2px Signal Red and initiates a subtle "Pulse" glow.

### Pulse Indicator
A small (8px) dot next to live data. In stable mode, it pulses in Slate. In critical mode, it pulses in Signal Red at a higher frequency to visually communicate heart rate rhythm and urgency.

### Input Fields
Strict, rectangular fields with 1px Slate borders. Focused states use a 2px Slate border. Error states use a 2px Signal Red border with no "glow"—just a sharp, clear indication of an error.

### Progress & Waveforms
EKG Waveforms must be rendered in Slate on a Silk White background. In an alert state, the waveform line color transitions instantly to Signal Red.