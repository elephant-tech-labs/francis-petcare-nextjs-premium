# Francis Petcare SEO, Schema & Tracking Plan

## Purpose

This document defines the SEO, structured data, analytics, and tracking requirements for the Francis Petcare Hospital Next.js rebuild.

The website is not only a design project.

It must support:
- local SEO rankings
- Google Business Profile relevance
- organic traffic
- service-specific rankings
- calls
- appointment requests
- form submissions
- Richmond location relevance
- exotic pet authority
- measurable conversion reporting

---

## Core SEO Positioning

Francis Petcare Hospital should be positioned as:

A full-service animal hospital in Richmond, BC for cats, dogs, rabbits, reptiles, ferrets, guinea pigs, hamsters, hedgehogs, and small mammals.

Main differentiator:
Exotic pet care.

Primary local SEO themes:
- animal hospital Richmond BC
- pet hospital Richmond BC
- veterinarian Richmond BC
- vet Richmond BC
- exotic pet vet Richmond
- exotic vet Richmond BC
- rabbit vet Richmond
- reptile vet Richmond
- rabbit dental care Richmond
- exotic pet surgery Richmond
- pet dental care Richmond
- cat boarding Richmond
- in-home pet euthanasia Richmond
- urgent care vet Richmond

---

## Critical SEO Rules

Do not:
- mention bird care unless confirmed
- claim 24/7 emergency care
- use “emergency vet” unless the clinic confirms true emergency service
- create thin doorway pages
- duplicate the same content across many pages
- invent credentials or reviews
- add fake review schema
- mark up third-party reviews improperly
- publish pages with placeholder metadata
- index irrelevant technical/demo pages

Use:
- urgent care during clinic hours
- same-day appointments when available
- call ahead
- Richmond, BC naturally in key locations
- service-specific page titles
- strong internal linking
- structured data
- local business consistency
- human, trustworthy copy

---

## Phase 1 SEO Page Structure

Recommended Phase 1 routes:

```txt
/
 /about/
 /veterinarians/
 /services/
 /exotic-pet-vet-richmond/
 /rabbit-vet-richmond/
 /reptile-vet-richmond/
 /rabbit-dental-care-richmond/
 /exotic-pet-surgery-richmond/
 /pet-dental-care-richmond/
 /pet-surgery-richmond/
 /spay-neuter-richmond/
 /cat-boarding-richmond/
 /in-home-pet-euthanasia-richmond/
 /urgent-care-vet-richmond/
 /book-appointment/
 /contact/
 /faq/

If Phase 1 must be smaller, prioritize:

/
 /services/
 /exotic-pet-vet-richmond/
 /rabbit-vet-richmond/
 /reptile-vet-richmond/
 /pet-dental-care-richmond/
 /in-home-pet-euthanasia-richmond/
 /urgent-care-vet-richmond/
 /veterinarians/
 /contact/
 /book-appointment/
Metadata Requirements

Every page must have:

unique title
unique meta description
canonical URL
Open Graph title
Open Graph description
Open Graph image
Twitter card metadata if used
no placeholder metadata
no duplicate titles across service pages

Title format examples:

Homepage:

Animal Hospital & Exotic Pet Vet in Richmond BC | Francis Petcare

Exotic page:

Exotic Pet Vet in Richmond BC | Francis Petcare Hospital

Rabbit page:

Rabbit Vet in Richmond BC | Francis Petcare Hospital

Reptile page:

Reptile Vet in Richmond BC | Francis Petcare Hospital

Dental page:

Pet Dental Care in Richmond BC | Francis Petcare Hospital

In-home euthanasia page:

In-Home Pet Euthanasia in Richmond BC | Francis Petcare

Urgent care page:

Urgent Care Vet in Richmond BC | Call Ahead
Metadata Implementation

Use the Next.js App Router metadata system.

Recommended:

lib/seo.ts
data/site.ts
data/pages.ts

Example structure:

export const siteConfig = {
  name: "Francis Petcare Hospital",
  baseUrl: "https://francispetcare.ca",
  phone: "(604) 277-8511",
  address: {
    street: "100-8980 No. 3 Road",
    city: "Richmond",
    region: "BC",
    postalCode: "V6Y 2E8",
    country: "CA",
  },
};

Each route should export metadata from page-specific data.

Canonical Rules

Use self-referencing canonical URLs for all indexable pages.

Example:

https://francispetcare.ca/exotic-pet-vet-richmond/

Avoid:

query parameter canonicals
trailing/non-trailing inconsistency
canonical pointing to old WordPress URLs
canonical pointing to staging/test domain

For staging:

do not allow test.francispethospital.ca to become the canonical production domain unless intentionally approved
staging can use noindex or be blocked from indexing until launch
Robots.txt Requirements

For production:

User-agent: *
Allow: /

Sitemap: https://francispetcare.ca/sitemap.xml

For staging/test subdomain:

Recommended:

User-agent: *
Disallow: /

Or apply noindex headers/meta on staging.

Important:
Do not let Google index test.francispethospital.ca.

Sitemap Requirements

Generate sitemap dynamically or statically with all indexable Phase 1 routes.

Include:

homepage
services
service landing pages
doctor/team page
contact/book pages
FAQ if used

Exclude:

admin/docs pages
demo pages
test pages
old WordPress-only URLs
utility/API routes
placeholder pages not ready for public indexing

Sitemap URL:

/sitemap.xml
Redirect Map Requirements

Create redirect support for old WordPress URLs.

Suggested file:

data/redirects.ts

or next.config.ts redirects.

Important old URLs to map if they exist:

/home-help-desk/ -> /
/exotic-pet-medicine-and-surgery/ -> /exotic-pet-vet-richmond/
/pet-dental-care-services/ -> /pet-dental-care-richmond/
/spay-neuter-services/ -> /spay-neuter-richmond/
/cat-boarding-services/ -> /cat-boarding-richmond/
/in-home-euthanasia-services/ -> /in-home-pet-euthanasia-richmond/
/emergency-and-or-extended-care/ -> /urgent-care-vet-richmond/
/pets-we-serve/ -> /services/

Also handle malformed old links if found:

/https://francispetcare.ca/pet-vaccination-services/ -> relevant service page
/https://francispetcare.ca/pet-dental-care-services/ -> /pet-dental-care-richmond/
/https://francispetcare.ca/spay-neuter-services/ -> /spay-neuter-richmond/

Before launch, run a full crawl of the current WordPress site and finalize redirects.

Structured Data Requirements

Use JSON-LD components.

Recommended folder:

components/schema/
  LocalBusinessSchema.tsx
  VeterinaryCareSchema.tsx
  ServiceSchema.tsx
  FAQSchema.tsx
  BreadcrumbSchema.tsx
  WebSiteSchema.tsx
  PersonSchema.tsx
Local Business / Veterinary Schema

Use a local business schema appropriate for a veterinary clinic.

Recommended type:

VeterinaryCare if supported/appropriate
LocalBusiness
MedicalBusiness only if implementation is correct and not misleading

Include:

business name
URL
phone
address
geo coordinates if confirmed
opening hours
sameAs links if confirmed
image/logo
priceRange if approved
areaServed
services
department/service references if useful

Do not include:

fake aggregate rating
unsupported awards
unverified doctor credentials
24/7 hours
bird services unless confirmed
Service Schema

Each major service page should have Service schema.

Examples:

Exotic Pet Veterinary Care
Rabbit Veterinary Care
Reptile Veterinary Care
Pet Dental Care
Rabbit Dental Care
Pet Surgery
Exotic Pet Surgery
Spay and Neuter Surgery
Cat Boarding
In-Home Pet Euthanasia
Urgent Care During Clinic Hours

Each Service schema should include:

service name
description
provider: Francis Petcare Hospital
areaServed: Richmond, BC
URL
serviceType
FAQ Schema

Use FAQ schema only when the FAQ content is visible on the page.

Good pages for FAQ schema:

Exotic Pet Vet
Rabbit Vet
Reptile Vet
Pet Dental Care
Urgent Care
In-Home Euthanasia
Cat Boarding
Contact/Booking

Do not:

add hidden FAQ schema
spam too many FAQs
include unsupported claims
include emergency 24/7 claims

Example FAQ topics:

Exotic:

Do you treat rabbits?
Do you treat reptiles?
Do you treat snakes and lizards?
Do you treat hamsters and guinea pigs?
Do exotic pets need special handling?

Urgent:

Do you offer same-day appointments?
Are you a 24/7 emergency vet?
Answer: No. Francis Petcare Hospital offers urgent care during clinic hours when availability allows. Please call ahead.

Euthanasia:

Do you offer in-home pet euthanasia?
What should I expect?
How do I know when it may be time?
Breadcrumb Schema

Use breadcrumb schema on all pages except possibly homepage.

Example:

Home > Services > Exotic Pet Vet Richmond
Person Schema

Use Person schema for doctors only with verified information.

Doctor pages:

Dr. Tejpaul Bhatia
Dr. Joseph Martinez

Include:

name
jobTitle
worksFor
image if real or approved placeholder
description
URL

Do not include:

invented credentials
unsupported awards
fake alumni details
unconfirmed certifications
Review Schema Rules

Be careful.

Do not add aggregate rating schema unless:

rating is verified
ratings are visible on the page
implementation complies with Google review snippet rules
manually approved

Do not mark up third-party Google reviews as first-party review schema without approval.

Use reviews visually for trust, but avoid risky schema.

Internal Linking Strategy

Homepage should link to:

Services
Exotic Pet Vet
Rabbit Vet
Reptile Vet
Pet Dental Care
Surgery
Cat Boarding
In-Home Euthanasia
Urgent Care
Veterinarians
Contact/Book

Exotic Pet Vet page should link to:

Rabbit Vet
Reptile Vet
Rabbit Dental
Exotic Pet Surgery
Dr. Martinez
Urgent Care
Contact/Book

Rabbit Vet page should link to:

Exotic Pet Vet
Rabbit Dental
Dr. Martinez
Urgent Care
Contact/Book

Reptile Vet page should link to:

Exotic Pet Vet
Dr. Martinez
Contact/Book

Dental page should link to:

Rabbit Dental if applicable
Surgery
Contact/Book

Urgent Care page should link to:

Contact/Book
Services
Exotic Pet Vet
In-Home Euthanasia only if contextually appropriate

In-Home Euthanasia page should link gently to:

Contact
About/Team
Hospice/Comfort care if available
Image SEO

Every image must include meaningful alt text.

Alt text should be:

descriptive
local when relevant
not keyword-stuffed
honest about placeholders only in code comments, not public alt text

Good examples:

Rabbit receiving veterinary care at Francis Petcare Hospital in Richmond BC
Dr. Joseph Martinez, exotic pet veterinarian at Francis Petcare Hospital
Cat boarding area at Francis Petcare Hospital
Veterinary exam room at Francis Petcare Hospital in Richmond BC

Bad examples:

best exotic pet vet Richmond BC rabbit vet near me
image
placeholder
cute pet
Tracking Requirements

Use GA4 and event tracking.

Recommended environment variable:

NEXT_PUBLIC_GA_ID=G-XXXXXXXXXX

Tracking file:

lib/analytics.ts
components/GoogleAnalytics.tsx
Required GA4 Events
Phone Click

Event:

phone_click

Parameters:

location: header | hero | sticky_mobile | footer | service_sticky_card | contact_page
page_path
Appointment Click

Event:

appointment_click

Parameters:

location
page_path
cta_text
Booking Form Start

Event:

booking_form_start

Parameters:

page_path
form_name
Booking Form Submit

Event:

booking_form_submit

Parameters:

page_path
form_name
service_interest
Contact Form Submit

Event:

contact_form_submit

Parameters:

page_path
form_name
Email Click

Event:

email_click

Parameters:

location
page_path
Directions Click

Event:

directions_click

Parameters:

location
page_path
Review Link Click

Event:

google_reviews_click

Parameters:

location
page_path
Service CTA Click

Event:

service_cta_click

Parameters:

service_name
page_path
cta_text
GBP UTM Tracking

Use UTM links on Google Business Profile.

Website URL:

https://francispetcare.ca/?utm_source=google&utm_medium=organic&utm_campaign=gbp

Appointment URL:

https://francispetcare.ca/book-appointment/?utm_source=google&utm_medium=organic&utm_campaign=gbp_booking

If using test/staging, do not put staging URLs in GBP.

Search Console Setup

Before launch:

verify domain/property
submit sitemap
inspect homepage
inspect key service pages
confirm no staging domain indexed
check redirects
check indexing report after launch

After launch:

monitor 404s
monitor excluded pages
monitor core service page indexing
monitor queries for exotic/rabbit/reptile/dental
Conversion Tracking QA

Before launch, test:

header phone click
hero phone click
mobile sticky phone click
book appointment CTA
contact form
booking form
service sticky form
email link
directions link
review link
GBP UTM traffic in GA4
form notification delivery
Performance SEO Requirements

The site should aim for:

fast LCP
minimal layout shift
optimized images
no unnecessary JavaScript
static pages where possible
accessible HTML
semantic headings
clean internal links
no bloated third-party scripts

Avoid:

large unoptimized hero images
heavy animation libraries unless truly needed
autoplay video with large files
layout shifts from image placeholders
unnecessary sliders/carousels
loading all form code globally if not needed
Accessibility Requirements

SEO and accessibility overlap.

Required:

one H1 per page
logical heading order
descriptive link text
accessible buttons
visible focus states
form labels
error states
sufficient color contrast
alt text
keyboard navigable navigation
no CTA text like "click here"
Staging Domain Rules

For test.francispethospital.ca:

do not allow indexing
do not use as canonical
do not submit to Search Console as production unless intentionally testing
do not add to GBP
use only for review/QA

Production canonical should be final approved domain only.

Pre-Launch SEO Checklist

Before final launch:

all page titles unique
all meta descriptions unique
canonical URLs correct
schema validates
sitemap works
robots.txt correct
no staging noindex accidentally on production
redirect map implemented
no old broken WordPress links
no 24/7 emergency claim
no bird care
phone and address consistent with GBP
forms tested
GA4 events tested
GSC sitemap submitted
pages manually inspected
