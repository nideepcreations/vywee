---
Project: Vywee
Document: Design System
Version: 1.0.0
Status: Active
Owner: Product Team
---

# Vywee Design System

## Purpose

The Design System defines every reusable UI element used throughout Vywee.

Every page must reuse these components.

Never redesign the same component twice.

---

# Design Philosophy

The interface should feel like

• Apple
• Stripe
• Linear
• Notion
• Perplexity

NOT

• Amazon
• Flipkart
• Alibaba

The product is a research platform.

Not an online marketplace.

---

# Design Principles

1. Mobile First

2. Accessibility First

3. Consistency Over Creativity

4. Performance Before Animation

5. Reusable Components Only

---

# Color Palette

Primary

Orange

Secondary

Black

Background

White

Surface

Light Gray

Success

Green

Warning

Orange

Danger

Red

Information

Blue

Dark Mode

Supported

---

# Typography

Headings

Bold

Large spacing

Body

Readable

16px minimum

Buttons

Medium Weight

Uppercase NOT allowed

---

# Border Radius

Cards

16px

Buttons

14px

Inputs

14px

Dialogs

20px

---

# Shadows

Very subtle.

No floating UI.

No heavy shadows.

---

# Grid

Desktop

12 Columns

Tablet

6 Columns

Mobile

1 Column

---

# Breakpoints

Mobile

0–767

Tablet

768–1023

Desktop

1024+

Large Desktop

1440+

---

# Spacing Scale

4

8

12

16

20

24

32

40

48

64

80

96

Never use random spacing.

---

# Animation

Maximum

200ms

Fade

Slide

Scale

No bouncing animations.

No flashy effects.

---

# Icons

Lucide Icons

Only.

No mixed icon packs.

---

# Images

Rounded corners.

Lazy loading.

Optimized.

Responsive.

---

# Core Components

Button

Input

Textarea

Checkbox

Radio

Switch

Select

Dropdown

Badge

Chip

Avatar

Tooltip

Modal

Drawer

Tabs

Accordion

Pagination

Breadcrumb

Toast

Skeleton

Divider

Progress

Spinner

Empty State

Loading State

---

# Feature Components

Search Input

Product Card

Product List Card

Category Card

Brand Card

Offer Card

Buying Guide Card

AI Summary Card

Pros & Cons Card

Price Card

Rating Component

Comparison Table

Offer List

Price History

Filter Panel

Search Suggestion

Section Header

Hero Banner

Trust Card

---

# Layout Components

Header

Footer

Container

Sidebar

Bottom Navigation

Mobile Navigation

Section

Page Wrapper

Sticky Filter

Bottom Sheet

---

# Component Rules

Every component must

Be reusable

Support light and dark mode

Support loading state

Support empty state

Support responsive layout

Support accessibility

Never contain business logic

---

# Button Variants

Primary

Secondary

Outline

Ghost

Danger

Success

Link

Icon Button

Loading Button

Disabled Button

---

# Input Variants

Text

Email

Password

Search

Number

Phone

Textarea

---

# Card Rules

Every card should answer

What is this?

Why should I care?

What should I do next?

---

# Product Card

Contains

Image

Title

Price

Rating

Vywee Badge

Offer Badge

View Details

Save

Share

Quick Compare

---

# Search Input

Large

Rounded

Autocomplete

Suggestions

Voice Search (Future)

Image Search (Future)

---

# Empty States

Every empty state should

Explain

Encourage

Guide

Never simply say

"No Data"

---

# Loading States

Skeleton only.

No spinning screen.

---

# Accessibility

Keyboard Navigation

Screen Reader Labels

Visible Focus States

Minimum touch target

48px

WCAG AA

---

# Performance

Lazy Loading

Dynamic Imports

Optimized Images

Reusable Components

Memoization where required

---

# Naming Convention

Component Names

PascalCase

Example

ProductCard

SearchInput

SectionHeader

File Names

kebab-case

Example

product-card.tsx

search-input.tsx

---

# Folder Structure

components/

ui/

layout/

features/

shared/

---

# Quality Rules

No duplicate components

No inline styles

No hardcoded colors

No hardcoded spacing

No business logic inside UI

No API calls inside components

---

# Future Components

Charts

Price Alerts

AI Chat

Decision Timeline

Decision Score

Recommendation Engine

Browser Extension Widgets

---

# Final Principle

Every component should be reusable across

Homepage

Search

Product Page

Compare

Studio

Mobile App

without modification.

If a component cannot be reused,

redesign it.
