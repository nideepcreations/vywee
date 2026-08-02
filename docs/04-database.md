---
Project: Vywee
Document: Database Design
Version: 1.0.0
Status: Active
Owner: Product Team
---

# Database Design

## Objective

Design a scalable database that supports products, comparisons, research, AI content, offers and future categories without redesign.

---

# Database Principles

- UUID for all primary keys
- Soft Delete
- Audit Fields
- Optimized Indexes
- Scalable Relationships

---

# Core Tables

## users

Purpose

Stores user information.

Columns

- id
- name
- email
- avatar
- role
- created_at
- updated_at

---

## categories

Stores product categories.

Examples

- Electronics
- Fashion
- Home
- Beauty
- Finance

Columns

- id
- name
- slug
- icon
- description

---

## brands

Stores manufacturers.

Examples

- Apple
- Samsung
- Sony
- LG

Columns

- id
- name
- slug
- logo

---

## retailers

Stores affiliate partners.

Examples

- Amazon
- Flipkart
- Croma
- Reliance Digital

Columns

- id
- name
- website
- affiliate_enabled

---

## products

Main product table.

Columns

- id
- title
- slug
- category_id
- brand_id
- description
- image
- status
- created_at
- updated_at

---

## product_images

Stores multiple product images.

Columns

- id
- product_id
- image_url
- display_order

---

## specifications

Stores technical specifications.

Columns

- id
- product_id
- key
- value

Example

RAM → 16 GB

Storage → 512 GB

---

## offers

Stores live offers.

Columns

- id
- product_id
- retailer_id
- price
- original_price
- affiliate_url
- cashback
- updated_at

---

## price_history

Stores historical prices.

Columns

- id
- product_id
- retailer_id
- price
- captured_at

---

## buying_guides

Stores editorial buying guides.

Columns

- id
- title
- slug
- category_id
- content
- status

---

## comparisons

Stores saved comparisons.

Columns

- id
- title
- created_by

---

## comparison_products

Relationship table.

Columns

- comparison_id
- product_id

---

## my_research

Stores user research.

Columns

- id
- user_id
- product_id
- notes
- created_at

---

## my_picks

Stores user collections.

Columns

- id
- user_id
- title
- description

---

## my_pick_products

Relationship table.

Columns

- pick_id
- product_id

---

## opinions

Stores Ask Someone sessions.

Columns

- id
- product_id
- share_token
- expires_at

---

## opinion_votes

Stores votes.

Columns

- opinion_id
- vote
- comment

---

## ai_content

Stores AI generated content.

Columns

- id
- product_id
- summary
- why_buy
- why_skip
- best_for
- alternatives

---

## activity_logs

Stores admin activity.

Columns

- id
- user_id
- action
- entity
- entity_id
- created_at

---

# Relationships

Category

↓

Products

↓

Offers

↓

Price History

↓

AI Content

---

User

↓

My Research

↓

My Picks

↓

Comparisons

---

# Database Rules

- Never hard delete production data.
- Store timestamps in UTC.
- Use UUIDs.
- Index frequently searched columns.
- Normalize data where practical.
- Avoid duplicate product information.

---

# Future Tables

Reserved for:

- Finance Products
- Travel
- Insurance
- Browser Extension
- AI Memory
- Notifications
- Decision Rooms

---

# Version History

## 1.0.0

Initial Database Design
