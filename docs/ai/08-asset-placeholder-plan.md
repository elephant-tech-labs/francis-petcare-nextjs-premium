# Francis Petcare Asset & Placeholder Plan

## Purpose

This document defines how images, videos, and visual placeholders should be handled in the Francis Petcare Hospital Next.js rebuild.

The website must be designed like a premium veterinary hospital website even if final real photos are not yet available.

Do not weaken the layout because assets are missing.

Use premium placeholders now and structure the site so real clinic photos, doctor photos, pet photos, exotic pet photos, and videos can be dropped into `/public/images/` later.

---

## Core Principle

Design as if the clinic will eventually provide high-quality original assets.

The site should not feel empty, generic, or unfinished because final photos are not ready.

Placeholders should be:
- clean
- premium
- medically appropriate
- brand-aligned
- descriptive
- easy to replace
- optimized for layout consistency

Placeholders should not feel like:
- random stock photography
- fake pet-shop imagery
- playful daycare visuals
- low-quality AI art
- generic SaaS illustrations
- unrelated icons or blobs

---

## Asset Storage

Use this folder structure:

```txt
public/
  images/
    brand/
    clinic/
    doctors/
    pets/
    exotic/
    services/
    reviews/
    videos/
