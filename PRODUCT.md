# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

Python with Flask, Flask-SQLAlchemy, Jinja templates, and Supabase-hosted PostgreSQL. Keep the project beginner-friendly and avoid React or complex tooling. Hosting target is undecided.

## Users

Digital marketers and content teams are the confirmed primary audience. Users create and manage campaign links and review their traffic. Platform admins manage the whole service, disable abusive links, and maintain a blocked-domain list.

## Product Purpose

LinkPulse helps digital marketers and content teams shorten and manage campaign links, control redirect behavior, and understand visits through analytics. Success means the core flow works end to end: create a link, redirect through it, and see its click data.

## Positioning

The product's central record is a Link, connected to campaigns, redirect rules, click events, and reports. The PRD supplies this as the product mechanism; it does not make a competitive or market-leadership claim.

## Operating Context

LinkPulse is being built for the Event Tech Geeks hackathon. The five-minute demo should show account access, link creation, redirect, and analytics; the PRD also asks to demonstrate CSV import and admin disable behavior as those capabilities are built. The user prefers beginner-friendly explanations and one implementation step at a time.

## Capabilities and Constraints

- P0: registration/login/logout with user and admin roles; create links with generated or custom codes; HTTP 302 redirects; click tracking with hashed IPs; per-link analytics; public deployment.
- P1: redirect expiry, click limits, password protection, pre-publish validation, campaigns, tags, admin disable and blocked domains, bot filtering, asynchronous logging, rate limiting, and analytics dashboard.
- P2: QR codes, CSV import, approximate unique visitors, and a link-in-bio page.
- P3 items are roadmap only for the hackathon: device targeting, custom domains, public API, workspaces/folders, scheduled reports/email alerts, and Google Safe Browsing.
- Product values and analytics must come from database records, not hard-coded demo data.
- Roles: visitors use public short links; users manage only their own records; admins manage the platform. Authorization must be checked on protected routes.
- Store hashed IP addresses only; hash account and optional link passwords; preserve analytics for disabled or expired links.
- The user chose Supabase PostgreSQL instead of the SQLite option in the original prompt. The database project already exists.

## Brand Commitments

The product name is LinkPulse. No logo, visual identity, font, palette, or product voice has been provided yet.

## Evidence on Hand

The supplied LinkPulse PRD, version 1.0 dated 2026-10-15, is the current product source. No customer testimonials, performance benchmarks, or production analytics were supplied. Demo data is requested but has not been created.

## Product Principles

- Finish a working core before adding breadth.
- Use real stored data for links and analytics.
- Keep user data isolated and give admins explicit governance tools.
- Explain technical concepts plainly and keep implementation steps small.
