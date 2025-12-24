# 🍑 Peach Mango Page Creation Workflow

## Quick Start Guide

This guide will help you create new pages for your Peach Mango site with a consistent title section and two-column layout.

---

## Creating a New Page

### Step 1: Copy the Template

Copy `_page-template.html` to create your new page:

```bash
cp _page-template.html your-new-page.html
```

### Step 2: Customize Your Page

Open `your-new-page.html` and customize these sections:

#### 1. Page Title (Line 6)
```html
<title>Your Page Name - Peach Mango</title>
```

#### 2. Title Section (Lines 250-253)
```html
<h1 class="page-title">Your Page Title</h1>
<p class="page-subtitle">Add your subtitle or description here</p>
```

#### 3. Two Columns (Lines 258-283)
- **Left Column**: Edit the content starting at line 260
- **Right Column**: Edit the content starting at line 273

#### 4. Cloud Index Navigation (Lines 236-241)
Add your new page to the navigation menu:
```html
<a href="your-new-page.html" class="cloud-index-link active">🎯 Your Page</a>
```

### Step 3: Update All Pages

Add your new page to the cloud index on **ALL existing pages**:
- `index.html`
- `personal-dashboard.html`
- `hi-brian.html`
- `emperical-luxe.html`

Find the cloud index section in each file and add:
```html
<a href="your-new-page.html" class="cloud-index-link">🎯 Your Page</a>
```

---

## Template Features

### ✅ Included Components

- **Cloud Index Navigation**: Floating navigation on the right (auto-included)
- **Title Section**: Large centered title with subtitle
- **Two-Column Layout**: Responsive columns that stack on mobile
- **Footer**: Fixed footer matching site design
- **Peach Mango Theme**: Consistent colors and styling
- **Responsive Design**: Works on desktop, tablet, and mobile

### 🎨 Color Palette

- Background: `#fdf5e6`
- Primary Orange: `#ff6b35`
- Secondary Orange: `#ffb366`
- Text: `#333`

### 📱 Responsive Breakpoints

- Desktop: Full two-column layout
- Tablet (< 968px): Stacked columns
- Mobile (< 600px): Compressed padding and fonts

---

## Customization Options

### Adding More Content Sections

You can add more sections after the two-column layout:

```html
<div class="two-column-section">
    <!-- Your additional two-column content -->
</div>
```

### Changing Column Widths

Modify the grid template in the `.two-column-section` class:

```css
grid-template-columns: 2fr 1fr;  /* Left column wider */
/* or */
grid-template-columns: 1fr 2fr;  /* Right column wider */
```

### Adding More Columns

Change to three columns:

```css
.two-column-section {
    grid-template-columns: 1fr 1fr 1fr;
    gap: 30px;
}
```

---

## Quick Tips

1. **Emoji Icons**: Add emojis to your cloud index links for visual appeal
2. **Active State**: Mark the current page's link with `class="cloud-index-link active"`
3. **Action Buttons**: Use the `.action-button` class for call-to-action links
4. **Consistent Footer**: Keep the same footer on all pages

---

## Example Workflow

```bash
# 1. Create a new page
cp _page-template.html my-awesome-page.html

# 2. Edit the file
# - Update the title
# - Add your content to both columns
# - Add your page to the cloud index

# 3. Update other pages
# - Add link to your new page in all existing cloud indexes

# 4. Test in browser
# - Open the page and verify all links work
# - Check responsive design on different screen sizes
```

---

## Need Help?

- The template uses standard HTML/CSS
- All styling is inline in the `<style>` tag
- Modify colors, fonts, and layouts as needed
- Check existing pages for examples

---

**Version 1.0** - Peach Mango Site Builder
