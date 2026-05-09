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
Image Design Style

Images should support the brand position:

Francis Petcare Hospital is a Richmond, BC animal hospital for cats, dogs, rabbits, reptiles, ferrets, guinea pigs, hamsters, hedgehogs, and small mammals.

Visual mood:

clean
calm
medical
warm
trustworthy
local
professional
not overly playful
not overly corporate

Use:

rounded image cards
subtle shadows
soft blue-gray backgrounds
navy borders or small accent lines
image overlays only when needed for readability
premium cropping
consistent aspect ratios

Avoid:

random stock photos with unrealistic clinic scenes
cluttered backgrounds
cartoonish pet graphics
fake-looking doctor images
overuse of paw prints
overuse of bright green or orange
images that imply bird care unless bird care is confirmed
emergency-room visuals that imply 24/7 emergency care
Required Homepage Asset Slots

The homepage should be designed with these asset slots:

1. Hero Image Collage

Purpose:
Create immediate trust and warmth above the fold.

Suggested slots:

large main clinic/doctor/pet image
smaller exotic pet image
small clinic/location image
floating review card

Placeholder paths:

/images/clinic/exam-room-placeholder.jpg
/images/exotic/rabbit-care-placeholder.jpg
/images/clinic/clinic-exterior-placeholder.jpg

Alt text examples:

"Veterinary exam room at Francis Petcare Hospital in Richmond BC"
"Rabbit receiving veterinary care at Francis Petcare Hospital"
"Francis Petcare Hospital exterior in Richmond BC"
2. Trust Strip / Quick Facts

Can use icons instead of images.

Icon style:

simple line icons
medical/veterinary feel
navy or blue-gray
no cartoon style

Suggested facts:

Richmond, BC animal hospital
Cats, dogs and exotic pets
Same-day appointments when available
Cat boarding
In-home euthanasia
3. Signature Exotic Pet Section

Purpose:
This must visually establish Francis Petcare as exotic-capable.

Suggested slots:

/images/doctors/dr-martinez-placeholder.jpg
/images/exotic/rabbit-care-placeholder.jpg
/images/exotic/reptile-care-placeholder.jpg
/images/exotic/hamster-care-placeholder.jpg

Alt text examples:

"Dr. Joseph Martinez, exotic pet veterinarian at Francis Petcare Hospital"
"Rabbit veterinary care in Richmond BC"
"Reptile veterinary care in Richmond BC"
"Hamster and small mammal veterinary care in Richmond BC"
4. Doctor Section

Required doctor image slots:

/images/doctors/dr-bhatia-placeholder.jpg
/images/doctors/dr-martinez-placeholder.jpg

Alt text:

"Dr. Tejpaul Bhatia, veterinarian and owner of Francis Petcare Hospital"
"Dr. Joseph Martinez, exotic pet veterinarian in Richmond BC"

If real portraits are not available:

use premium silhouette/photo placeholder cards
clearly mark TODO in data
do not use fake doctor images
5. Service Cards

Each major service should have either a premium icon or image.

Recommended:

use image cards for signature services
use icons for routine services

Service image slots:

/images/services/dental-care-placeholder.jpg
/images/services/surgery-placeholder.jpg
/images/services/urgent-care-placeholder.jpg
/images/services/cat-boarding-placeholder.jpg
/images/services/in-home-euthanasia-placeholder.jpg
/images/exotic/rabbit-care-placeholder.jpg
/images/exotic/reptile-care-placeholder.jpg
6. Appointment / Contact Section

Suggested image:

/images/clinic/reception-placeholder.jpg

Alt:
"Reception area at Francis Petcare Hospital in Richmond BC"

7. Final CTA

Suggested image or background:

/images/clinic/clinic-exterior-placeholder.jpg

Or use a dark navy gradient section without image.

Service Page Asset Slots

Every service page should support:

Hero image
Inline supporting image
Doctor proof image, if relevant
Review card
Sticky appointment form
Exotic Pet Vet Page

Primary image:

/images/exotic/rabbit-care-placeholder.jpg

Supporting images:

/images/exotic/reptile-care-placeholder.jpg
/images/doctors/dr-martinez-placeholder.jpg
Rabbit Vet Page

Primary image:

/images/exotic/rabbit-care-placeholder.jpg

Supporting:

/images/doctors/dr-martinez-placeholder.jpg
/images/services/dental-care-placeholder.jpg
Reptile Vet Page

Primary image:

/images/exotic/reptile-care-placeholder.jpg

Supporting:

/images/exotic/snake-care-placeholder.jpg
/images/exotic/lizard-care-placeholder.jpg
Pet Dental Care Page

Primary:

/images/services/dental-care-placeholder.jpg

Supporting:

/images/pets/cat-care-placeholder.jpg
/images/pets/dog-care-placeholder.jpg
Surgery Page

Primary:

/images/services/surgery-placeholder.jpg

Supporting:

/images/clinic/treatment-room-placeholder.jpg
Urgent Care Page

Primary:

/images/services/urgent-care-placeholder.jpg

Important:
Do not use imagery that suggests a 24/7 emergency hospital.

Use wording:

urgent care during clinic hours
same-day appointments when available
call ahead
In-Home Euthanasia Page

Primary:

/images/services/in-home-euthanasia-placeholder.jpg

Tone:

soft
calm
compassionate
not clinical/cold
no graphic images
no aggressive CTA styling

CTA wording:

"Talk to our team"
"Call for guidance"
"Request a compassionate appointment"
Cat Boarding Page

Primary:

/images/services/cat-boarding-placeholder.jpg

Supporting:

/images/pets/cat-care-placeholder.jpg
Video Placeholder Plan

Videos are optional for Phase 1 but the layout should support them.

Recommended future videos:

Homepage Clinic Walkthrough

Path:

/videos/clinic-walkthrough.mp4

Use:
Homepage trust section or appointment section.

Purpose:
Show real clinic environment.

Exotic Pet Care Short Clip

Path:

/videos/exotic-pet-care.mp4

Use:
Exotic Pet Vet page or homepage exotic section.

Purpose:
Build confidence that the clinic truly sees rabbits/reptiles/small mammals.

Doctor Intro Video

Path:

/videos/dr-martinez-intro.mp4
/videos/dr-bhatia-intro.mp4

Use:
Doctor profile pages.

Purpose:
Increase trust and human connection.

Cat Boarding Walkthrough

Path:

/videos/cat-boarding-walkthrough.mp4

Use:
Cat boarding page.

Purpose:
Show boarding area and reduce anxiety.

Placeholder Component Requirements

Create reusable components such as:

ImageFrame
HeroImageCollage
VideoPlaceholder
DoctorImageCard
ServiceImageCard
BeforeAfterNotUsed
ReviewCard
StickyAppointmentCard

Image components should:

use Next.js Image where possible
include required alt text
maintain aspect ratio
avoid layout shift
support real replacement image paths later
avoid remote image dependency for Phase 1
Image Data Model

Use structured data so assets are easy to replace.

Example:

export const imageAssets = {
  clinicExterior: {
    src: "/images/clinic/clinic-exterior-placeholder.jpg",
    alt: "Francis Petcare Hospital exterior in Richmond BC",
    status: "placeholder",
    replacementNeeded: true,
  },
  drBhatia: {
    src: "/images/doctors/dr-bhatia-placeholder.jpg",
    alt: "Dr. Tejpaul Bhatia, veterinarian and owner of Francis Petcare Hospital",
    status: "placeholder",
    replacementNeeded: true,
  },
  drMartinez: {
    src: "/images/doctors/dr-martinez-placeholder.jpg",
    alt: "Dr. Joseph Martinez, exotic pet veterinarian in Richmond BC",
    status: "placeholder",
    replacementNeeded: true,
  },
};
Real Asset Collection Checklist

Request from the clinic:

Clinic Photos
exterior with signage
front desk/reception
waiting area
exam room
treatment area
dental/surgery equipment, non-graphic
cat boarding area
team working naturally
Doctor / Team Photos
Dr. Bhatia portrait
Dr. Martinez portrait
doctors with pets, if consented
team group photo
front desk team
technician/nurse team
Pet Photos

Only use with proper permission.

Needed:

rabbit
reptile
hamster
guinea pig
ferret
hedgehog
cat
dog/puppy
Video
short clinic walkthrough
doctor introduction
exotic pet care clip
cat boarding clip
Consent and Compliance

Do not use client/pet photos unless the clinic confirms permission.

Do not show:

identifiable clients without permission
medical procedures in a graphic way
distressing pet images
surgery images
emergency imagery that overstates capability
bird images unless bird care is confirmed
Design Quality Bar

The design should still look complete with placeholders.

A user should not feel:
"This site is unfinished."

They should feel:
"This is a polished premium clinic website and the final real photos will make it even stronger."

Codex Implementation Rules

Before coding asset-heavy sections, Codex must:

Create or preserve the asset data structure.
Use descriptive placeholder paths.
Add meaningful alt text.
Mark missing real assets as TODO.
Avoid random external images.
Avoid fake doctor photos.
Avoid bird imagery.
Ensure image cards are premium and brand-aligned.
Ensure homepage and service pages can be upgraded by replacing image files only
