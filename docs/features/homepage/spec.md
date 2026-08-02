---
Project: Vywee
Feature: Homepage
Document: Build Specification
Version: 1.0.0
Status: Active
---

# Homepage Build Specification

## Purpose

Build a premium homepage for Vywee.

The homepage should immediately communicate that Vywee helps users make smarter buying decisions.

The page should feel closer to Apple, Stripe and Perplexity than to Amazon or Flipkart.

---

# Target User

First-time visitor.

The visitor should understand the purpose of Vywee within five seconds.

---

# Primary Goal

Encourage users to start researching a product.

The Search Bar is the most important element on the page.

---

# Technology

Frontend

- Next.js 15
- React
- TypeScript
- Tailwind CSS
- shadcn/ui
- Framer Motion

---

# Sections

The homepage should contain the following sections.

1. Header

2. Hero

3. AI Search

4. Popular Categories

5. Vywee Choice

6. Trending Products

7. Buying Guides

8. Why Trust Vywee

9. Footer

---

# Header

Contains

- Logo
- Search (Desktop)
- Navigation
- Theme Toggle (Future)
- Login (Future)

Sticky

Yes

---

# Hero

Contains

Headline

Subheading

Search Bar

Quick Search Suggestions

---

# Search

Large rounded search bar.

Placeholder

"What are you looking to buy today?"

Below it display chips.

Examples

- Best Laptop under ₹60,000

- Best Smartwatch

- Best AC

- Best Phone

---

# Categories

Initially

Electronics

Fashion

Home

Beauty

Kitchen

Travel (Future)

Finance (Future)

Each category uses an icon.

---

# Vywee Choice

Display

4 featured products.

Each card contains

- Image
- Name
- Current Price
- Rating
- Vywee Choice Badge
- View Details Button

---

# Trending Products

Same card layout.

Trending badge instead.

---

# Buying Guides

Display latest guides.

Each guide contains

- Cover Image

- Title

- Short Description

- Read Guide Button

---

# Why Trust Vywee

Display four cards.

AI Research

Honest Recommendations

Compare Products

Best Offers

---

# Footer

Contains

Company

Resources

Legal

Social Links

---

# Design Rules

White background.

Premium spacing.

Rounded corners.

Minimal shadows.

Large typography.

Mobile First.

---

# Responsive Behaviour

Desktop

Maximum Width

1280px

Tablet

Responsive Grid

Mobile

Single Column

---

# Loading State

Skeleton cards.

Never blank page.

---

# Empty State

Helpful message.

Guide users to search.

---

# Accessibility

Keyboard Navigation

Screen Reader Labels

Proper Heading Structure

High Contrast

---

# Performance

Homepage should load under 2 seconds.

Images should use lazy loading.

---

# Mock Data

Use static JSON.

Do NOT connect database.

Do NOT call APIs.

---

# Future Integration

Search API

Categories API

Product API

Guide API

Authentication

---

# Acceptance Criteria

✓ Mobile Responsive

✓ Desktop Responsive

✓ Accessible

✓ SEO Friendly

✓ Reusable Components

✓ Mock Data

✓ Clean Folder Structure

✓ Production Ready

---

# Important

The homepage should never feel like an online shopping website.

It should feel like a premium buying research platform.
