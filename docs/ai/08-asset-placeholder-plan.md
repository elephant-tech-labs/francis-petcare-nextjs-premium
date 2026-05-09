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

Recommended structure:

public/images/brand/
  francis-petcare-logo.svg
  francis-petcare-logo-mark.svg

public/images/clinic/
  clinic-exterior-placeholder.jpg
  reception-placeholder.jpg
  exam-room-placeholder.jpg
  treatment-room-placeholder.jpg
  front-desk-placeholder.jpg
  hallway-placeholder.jpg

public/images/doctors/
  dr-bhatia-placeholder.jpg
  dr-martinez-placeholder.jpg
  team-placeholder.jpg
  doctor-with-pet-placeholder.jpg
  doctor-with-exotic-pet-placeholder.jpg

public/images/pets/
  dog-care-placeholder.jpg
  puppy-care-placeholder.jpg
  cat-care-placeholder.jpg
  kitten-care-placeholder.jpg
  senior-pet-care-placeholder.jpg

public/images/exotic/
  rabbit-care-placeholder.jpg
  reptile-care-placeholder.jpg
  snake-care-placeholder.jpg
  lizard-care-placeholder.jpg
  hamster-care-placeholder.jpg
  guinea-pig-care-placeholder.jpg
  ferret-care-placeholder.jpg
  hedgehog-care-placeholder.jpg
  small-mammal-care-placeholder.jpg

public/images/services/
  dental-care-placeholder.jpg
  surgery-placeholder.jpg
  spay-neuter-placeholder.jpg
  diagnostics-placeholder.jpg
  vaccinations-placeholder.jpg
  urgent-care-placeholder.jpg
  cat-boarding-placeholder.jpg
  in-home-euthanasia-placeholder.jpg
  hospice-care-placeholder.jpg

public/images/reviews/
  google-review-placeholder.jpg

public/images/videos/
  clinic-walkthrough-placeholder.mp4
  exotic-care-placeholder.mp4
  doctor-introduction-placeholder.mp4
