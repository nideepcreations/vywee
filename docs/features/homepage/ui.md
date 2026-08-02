---
Project: Vywee
Feature: Homepage
Document: UI Specification
Version: 1.0.0
Status: Active
---

# Homepage UI Specification

## Design Philosophy

The homepage should immediately communicate:

> "Vywee helps you decide what to buy."

The design should feel:

- Premium
- Minimal
- Trustworthy
- Fast
- Modern

Avoid looking like an e-commerce marketplace.

---

# Page Layout

```
--------------------------------------------------

Header

Hero

AI Search

Popular Categories

Vywee Choice

Trending Products

Buying Guides

Why Trust Vywee

Footer

--------------------------------------------------
```

---

# Header

Height

72px Desktop

64px Mobile

Left

- Vywee Logo

Center

- Search (Desktop)

Right

- Theme Toggle (Future)
- Sign In (Future)

Sticky

Yes

Transparent on top

No

---

# Hero Section

Maximum Width

1280px

Centered

Yes

Padding

80px Desktop

48px Mobile

Contains

- Headline
- Description
- Search
- Quick Search Suggestions

---

# Headline

Large.

Maximum two lines.

Example

Stop Searching.

Start Selecting.

---

# Search Box

Width

Desktop

700px

Mobile

100%

Height

60px

Rounded

16px

Contains

- Search Icon
- Placeholder
- Search Button

Placeholder

"What are you looking to buy today?"

---

# Quick Search Chips

Examples

- Best Laptop under ₹60K

- Best Phone

- Best Smartwatch

- Best AC

Clickable

Yes

---

# Popular Categories

Grid

Desktop

6 Columns

Tablet

3 Columns

Mobile

2 Columns

Each Card

Contains

- Icon
- Category Name

---

# Vywee Choice

Horizontal product cards.

Desktop

4 Cards

Tablet

2 Cards

Mobile

1 Card

Each Card

Contains

- Product Image
- Product Name
- Price
- Vywee Choice Badge
- View Details

---

# Trending Products

Same layout as Vywee Choice.

Difference

Shows Trending Badge.

---

# Buying Guides

Card Layout

Desktop

3 Columns

Mobile

1 Column

Each Card

- Image
- Title
- Short Description
- Read Guide

---

# Why Trust Vywee

Four Cards

AI Research

Honest Reviews

Compare Easily

Best Offers

Simple icons.

No animations.

---

# Footer

Contains

Company

Resources

Legal

Social Links

Copyright

---

# Color Principles

Primary

Orange

Secondary

Black

Background

White

Text

Dark Gray

Success

Green

Error

Red

---

# Border Radius

Cards

16px

Buttons

14px

Search

16px

---

# Shadows

Very subtle.

No floating UI.

---

# Animations

Maximum

200ms

Fade

Slide

Scale

Only where necessary.

---

# Mobile Rules

Everything stacked vertically.

Large touch targets.

Minimum button height

48px

---

# Accessibility

Keyboard friendly.

Screen reader friendly.

WCAG AA compliant.

---

# Performance

Homepage should avoid unnecessary animations and large assets.

Images should use lazy loading where appropriate.

---

# Final User Feeling

When a user lands on the homepage, they should immediately feel:

"I've finally found a place that helps me decide—not just sell."
