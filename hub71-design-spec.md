# Hub71 Design System Specification

Based on analysis of https://www.hub71.com

## Color Palette

### Primary Colors
```css
--hub71-blue-primary: #124ef5;        /* Main brand blue - used for buttons, links, accents */
--hub71-blue-dark: #0026ab;          /* Darker blue - used for backgrounds, headers */
--hub71-blue-light: #4bace9;         /* Light blue - used for filters, secondary elements */
```

### Background Colors
```css
--hub71-bg-white: #FFFFFF;           /* Primary background */
--hub71-bg-light: #eff1f5;           /* Light gray background (footer, cards) */
--hub71-bg-light-alt: #EFF1F5;       /* Alternative light background */
```

### Text Colors
```css
--hub71-text-black: #000000;        /* Primary text color */
--hub71-text-gray: rgba(0,0,0,0.7);  /* Secondary text (70% opacity) */
--hub71-text-light: rgba(0,0,0,0.49); /* Light text (49% opacity) */
```

### Accent Colors
```css
--hub71-green: #6bce96;              /* Success/CTA green (also #6bce97) */
--hub71-orange: #dc4f33;             /* Accent orange */
--hub71-purple: #6b43c9;             /* Info boxes purple */
```

### Border Colors
```css
--hub71-border-light: #E1E5F0;       /* Light borders */
--hub71-border-gray: #E2E2E2;        /* Gray borders */
--hub71-border-blue: rgba(19,80,244,.32); /* Blue dashed borders */
```

## Typography

### Font Families
```css
--hub71-font-primary: 'Poppins', sans-serif;     /* Main body font */
--hub71-font-heading: 'roc-grotesk-wide', sans-serif; /* Headings (custom font) */
--hub71-font-arabic: 'Cairo', sans-serif;       /* Arabic support */
```

### Font Weights
- Regular: 400
- Medium: 500
- Semi-bold: 600
- Bold: 700
- Extra Bold: 800
- Black: 900

### Font Sizes
```css
--hub71-text-xs: 10px;      /* Small labels, dates */
--hub71-text-sm: 12px;      /* Buttons, small text */
--hub71-text-base: 13px;     /* Default body */
--hub71-text-md: 14px;       /* Secondary text */
--hub71-text-lg: 15px;       /* Larger body */
--hub71-text-xl: 16px;       /* Large body */
--hub71-heading-sm: 20px;    /* Small headings */
--hub71-heading-md: 22px;    /* Medium headings */
--hub71-heading-lg: 30px;    /* Large headings */
--hub71-heading-xl: 50px;    /* Extra large headings */
--hub71-heading-2xl: 67px;   /* Hero headings */
```

### Line Heights
```css
--hub71-leading-tight: 15px;
--hub71-leading-normal: 18px;
--hub71-leading-relaxed: 20px;
--hub71-leading-loose: 26px;
```

## Border Radius

**Minimal/None** - Hub71 uses square/rectangular elements:
```css
--hub71-radius-none: 0;
--hub71-radius-sm: 0.25rem;   /* Minimal rounding - rarely used */
--hub71-radius-md: 0.5rem;    /* Used sparingly */
```

**Note:** Most elements are square with `border-radius: 0` or very minimal rounding.

## Buttons

### Primary Button
```css
.btn-primary {
  background-color: #124ef5;
  color: #FFFFFF;
  border: 1px solid #124EF5;
  padding: 20px 23px;
  font-family: 'roc-grotesk-wide', sans-serif;
  font-weight: 600;
  font-size: 12px;
  line-height: 21px;
  text-transform: uppercase;
  border-radius: 0; /* Square */
  transition: all 0.2s;
}

.btn-primary:hover {
  background-color: #FFFFFF;
  color: #124ef5;
}
```

### Secondary Button
```css
.btn-secondary {
  background-color: transparent;
  color: #000000;
  border: 1px solid #E2E2E2;
  padding: 20px 23px;
  font-family: 'roc-grotesk-wide', sans-serif;
  font-weight: 600;
  font-size: 12px;
  line-height: 21px;
  text-transform: uppercase;
  border-radius: 0; /* Square */
}

.btn-secondary:hover {
  border-color: #124ef5;
  color: #124ef5;
}
```

### Green CTA Button
```css
.btn-green {
  background-color: #6bce96;
  color: #FFFFFF;
  border: 1px solid #6BCE97;
  padding: 20px 23px;
  font-family: 'roc-grotesk-wide', sans-serif;
  font-weight: 600;
  font-size: 12px;
  line-height: 21px;
  text-transform: uppercase;
  border-radius: 0; /* Square */
}

.btn-green:hover {
  background-color: #FFFFFF;
  color: #6bce96;
}
```

## Cards

### Standard Card
```css
.card {
  background-color: #FFFFFF;
  border: 1px solid #E1E5F0;
  padding: 30px;
  border-radius: 0; /* Square */
  transition: all 0.2s;
}

.card:hover {
  box-shadow: 0 0 8px rgba(0,0,0,0.12);
}
```

### Light Background Card
```css
.card-light {
  background-color: #eff1f5;
  border: 1px solid #E1E5F0;
  padding: 30px;
  border-radius: 0; /* Square */
}
```

## Form Elements

### Input Fields
```css
input[type="text"],
input[type="email"],
input[type="url"],
select {
  width: 100%;
  height: 50px;
  border: 1px solid #E2E2E2;
  background-color: #FFFFFF;
  padding: 5px 10px;
  font-family: 'Poppins', sans-serif;
  font-weight: 400;
  border-radius: 0; /* Square */
}

input:focus {
  outline: none;
  border-color: #124ef5;
}
```

## Complete CSS Variables

```css
:root {
  /* Colors - Primary */
  --hub71-blue-primary: #124ef5;
  --hub71-blue-dark: #0026ab;
  --hub71-blue-light: #4bace9;
  
  /* Colors - Backgrounds */
  --hub71-bg-white: #FFFFFF;
  --hub71-bg-light: #eff1f5;
  
  /* Colors - Text */
  --hub71-text-black: #000000;
  --hub71-text-gray: rgba(0,0,0,0.7);
  --hub71-text-light: rgba(0,0,0,0.49);
  
  /* Colors - Accents */
  --hub71-green: #6bce96;
  --hub71-orange: #dc4f33;
  --hub71-purple: #6b43c9;
  
  /* Colors - Borders */
  --hub71-border-light: #E1E5F0;
  --hub71-border-gray: #E2E2E2;
  --hub71-border-blue: rgba(19,80,244,0.32);
  
  /* Typography */
  --hub71-font-primary: 'Poppins', sans-serif;
  --hub71-font-heading: 'roc-grotesk-wide', sans-serif;
  --hub71-font-arabic: 'Cairo', sans-serif;
  
  /* Spacing */
  --hub71-spacing-xs: 10px;
  --hub71-spacing-sm: 15px;
  --hub71-spacing-md: 20px;
  --hub71-spacing-lg: 30px;
  --hub71-spacing-xl: 40px;
  
  /* Border Radius */
  --hub71-radius-none: 0;
  --hub71-radius-sm: 0.25rem;
  
  /* Shadows */
  --hub71-shadow-sm: 0 0 8px rgba(0,0,0,0.12);
  --hub71-shadow-md: 0 3px 6px rgba(0,0,0,0.16);
}
```

## Design Principles

1. **Light Theme**: White backgrounds with light gray accents
2. **Blue Primary**: Corporate blue (#124ef5) as main brand color
3. **Square Elements**: Minimal to no border-radius (0 or 0.25rem max)
4. **Clean Typography**: Sans-serif fonts (Poppins for body, custom for headings)
5. **Professional Look**: Corporate, clean, minimal design
6. **High Contrast**: Black text on white backgrounds
7. **Subtle Shadows**: Light shadows for depth (0 0 8px rgba(0,0,0,0.12))

## Google Fonts Alternative

Since `roc-grotesk-wide` is a custom font, use these Google Fonts alternatives:

```html
<!-- Primary font -->
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800;900&display=swap" rel="stylesheet">

<!-- Heading font alternative (similar to roc-grotesk-wide) -->
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
<!-- Or -->
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&display=swap" rel="stylesheet">
```

Use `Inter` or `Space Grotesk` for headings as they have a similar geometric, modern sans-serif feel.
