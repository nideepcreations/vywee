---
Project: Vywee
Document: API Specification
Version: 1.0.0
Status: Active
Owner: Engineering Team
---

# API Specification

## Purpose

This document defines the API standards and endpoints used throughout Vywee.

The frontend must never communicate directly with the database.

All requests go through the Backend API.

---

# API Principles

- REST API
- JSON Responses
- Stateless
- Versioned
- Secure
- Cache Friendly

---

# Base URL

/api/v1

Example

/api/v1/products

/api/v1/search

---

# Standard Response

Success

{
  "success": true,
  "message": "Success",
  "data": {}
}

Error

{
  "success": false,
  "message": "Product not found",
  "errorCode": "PRODUCT_NOT_FOUND"
}

---

# Authentication

Public

- Homepage
- Search
- Product Pages
- Compare
- Buying Guides

Protected

- My Research
- My Picks
- Studio
- User Profile

Admin

- Product Import
- AI Generation
- Analytics
- User Management

---

# Homepage API

GET

/homepage

Returns

- Featured Categories
- Trending Products
- Vywee Choice
- Buying Guides

---

# Search API

GET

/search

Query Parameters

- keyword
- category
- brand
- budget
- sort

Returns

- AI Summary
- Products
- Guides
- Suggestions

---

# Product API

GET

/products/{slug}

Returns

Complete product information.

Includes

- Images
- Specifications
- Offers
- AI Summary
- Price History
- Alternatives

---

# Compare API

POST

/compare

Input

2–4 Product IDs

Returns

- Winner
- Feature Comparison
- AI Verdict
- Best Value

---

# Offer API

GET

/products/{id}/offers

Returns

Top Offers

View All Offers

Affiliate Links

---

# Buying Guide API

GET

/guides

GET

/guides/{slug}

Returns

Buying Guide

Related Products

Related Guides

---

# Categories API

GET

/categories

GET

/categories/{slug}

---

# Brands API

GET

/brands

GET

/brands/{slug}

---

# My Research API

GET

/my-research

POST

/my-research

DELETE

/my-research/{id}

---

# My Picks API

GET

/my-picks

POST

/my-picks

PUT

/my-picks/{id}

DELETE

/my-picks/{id}

---

# Ask Someone API

POST

/opinion

Creates a shareable decision page.

GET

/opinion/{token}

Loads voting page.

POST

/opinion/{token}/vote

Stores vote.

---

# AI API

Internal Only

Functions

- Product Summary
- Compare
- Buying Guide
- SEO
- Search Explanation

Never exposed directly to users.

---

# Import API

POST

/import

Supports

- Product URL
- Search URL
- Category URL
- Brand URL

Returns

Draft Products

---

# Analytics API

Admin Only

Returns

- Clicks
- Searches
- Revenue
- CTR
- Top Products
- Top Categories

---

# Error Codes

400

Bad Request

401

Unauthorized

403

Forbidden

404

Not Found

409

Conflict

422

Validation Failed

500

Server Error

---

# API Versioning

Current

v1

Future

v2

Older versions should remain supported whenever practical.

---

# Security

- HTTPS Only
- JWT Authentication
- Input Validation
- Rate Limiting
- Secure Headers
- Role-Based Access

---

# Performance Goals

Homepage

<200 ms

Search

<800 ms

Product

<300 ms

Compare

<500 ms

---

# Future APIs

- Browser Extension
- Mobile Sync
- Price Alerts
- Finance
- Travel
- Decision Rooms

---

# Version History

## 1.0.0

Initial API Specification
