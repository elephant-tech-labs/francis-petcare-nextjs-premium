# Francis Petcare Launch Checklist

## Purpose

This document defines the launch checklist for the Francis Petcare Hospital Next.js + Vercel website.

The goal is to launch safely without losing SEO, breaking forms, confusing Google Business Profile, or publishing unsupported claims.

The current WordPress website should remain live until the new Next.js site passes QA.

---

## Launch Strategy

Recommended launch approach:

1. Build and test on local environment.
2. Deploy to Vercel preview.
3. Attach staging domain:
   ```txt
   test.francispethospital.ca
QA staging site thoroughly.
Fix all issues.
Prepare redirect map.
Confirm analytics and form tracking.
Confirm final production DNS plan.
Launch production domain.
Monitor indexing, forms, analytics, rankings, and errors.
Critical No-Go Rules

Do not launch if any of these are true:

site claims 24/7 emergency care
site mentions bird care without confirmation
fake reviews are present
fake doctor photos are used
doctor credentials are invented or unsupported
contact or booking forms are untested
phone links do not work
staging domain can be indexed
production pages have staging canonicals
sitemap is broken
robots.txt blocks production
old important WordPress URLs do not redirect
homepage title/meta is missing or duplicated
site still feels visually generic or off-brand
CTA buttons use random unapproved green colors
mobile layout is weak or broken
there is no clear call/book path above the fold
Phase 1 Pages to QA

Core pages:

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

If some are deferred to Phase 2, verify they are not linked as live pages.

Local Development QA

Run locally:

npm install
npm run dev

Check:

homepage loads
navigation works
mobile menu works
service links work
doctor links work
review sections render correctly
image placeholders display correctly
no broken layout sections
forms display correctly
footer links work

Run production build:

npm run build

Launch cannot proceed until build passes.

Vercel Deployment QA

After pushing to GitHub and deploying to Vercel:

Check:

deployment completes successfully
no build errors
environment variables set
staging domain loads over HTTPS
no mixed content errors
images load
metadata renders
sitemap works
robots.txt works
forms work or show correct placeholder behavior if not functional yet
Staging Domain QA

Staging domain:

test.francispethospital.ca

Required:

HTTPS active
no browser security warning
no indexing by Google
no production canonical pointing to staging
no GBP links pointing to staging
no public marketing links sent to staging except for review

Recommended robots for staging:

User-agent: *
Disallow: /

or use page-level noindex for staging.

Brand & Design QA

The site must feel:

premium
medical
trustworthy
warm
local
calm
conversion-focused
exotic-pet capable

Check:

Francis logo appears clean and not distorted
header feels polished
CTA colors match brand
no random green CTAs
navy/medical blue is primary
section spacing feels premium
cards do not look generic
hero has strong visual hierarchy
above fold explains Richmond + animal hospital + exotic pets
doctor cards look credible
review cards look polished
appointment/contact section feels professional
footer feels complete

Compare against:

Angel Pet Hospital reference
Webflow inspiration screenshots
current WordPress screenshot

Goal:
The new site should clearly look more premium and trustworthy than the current WordPress site.

Content QA

Confirm:

no bird care mentions
no 24/7 emergency claim
urgent care wording is accurate
same-day wording includes availability/call-ahead context
doctors are described accurately
Dr. Martinez is used as exotic pet proof
Dr. Bhatia is used as owner/experienced veterinarian proof
no unsupported awards
no unsupported surgery volume claims
no fake testimonials
no old Catcare-era reviews used as primary proof
no weird placeholder text
no lorem ipsum
no spelling mistakes
no "Book Appoinment" typo
no generic “we care for your furry friends” copy as core positioning
SEO QA

Check every indexable page:

unique title
unique meta description
one H1
logical H2/H3 structure
canonical URL correct
Open Graph title/description
internal links
breadcrumb if applicable
image alt text
schema where appropriate
page loads without JS-only content issues

Homepage must clearly include:

Francis Petcare Hospital
Richmond, BC
animal hospital
cats and dogs
exotic pets
rabbits
reptiles
small mammals
phone/book CTA
Schema QA

Validate JSON-LD for:

LocalBusiness/VeterinaryCare
WebSite
BreadcrumbList
Service
FAQ where visible
Person for doctor profiles

Do not launch if schema contains:

fake aggregateRating
fake reviews
24/7 hours
bird services
unsupported credentials
wrong address/phone
staging URLs on production
Redirect QA

Before replacing WordPress, create a full URL inventory from the old site.

Minimum redirects:

/home-help-desk/ -> /
/exotic-pet-medicine-and-surgery/ -> /exotic-pet-vet-richmond/
/pet-dental-care-services/ -> /pet-dental-care-richmond/
/spay-neuter-services/ -> /spay-neuter-richmond/
/cat-boarding-services/ -> /cat-boarding-richmond/
/in-home-euthanasia-services/ -> /in-home-pet-euthanasia-richmond/
/emergency-and-or-extended-care/ -> /urgent-care-vet-richmond/
/pets-we-serve/ -> /services/

Also redirect malformed links if still accessible:

/https://francispetcare.ca/pet-vaccination-services/ -> appropriate service page
/https://francispetcare.ca/pet-dental-care-services/ -> /pet-dental-care-richmond/
/https://francispetcare.ca/spay-neuter-services/ -> /spay-neuter-richmond/

After launch, test redirects manually and with a crawler.

Form & Conversion QA

Test all conversion actions:

Phone

Test:

header phone link
hero phone link
mobile sticky phone link
service sticky card phone link
footer phone link
contact page phone link

Expected:

phone link uses tel:
click event fires in GA4 if tracking enabled
Booking

Test:

hero booking CTA
mobile sticky booking CTA
service page booking CTA
book appointment page form
appointment form submission
confirmation message
email notification delivery
Contact

Test:

contact form
email click
directions link
map link
Service Interest

If forms include service selection, verify options include:

General veterinary care
Exotic pet care
Rabbit care
Reptile care
Dental care
Surgery
Cat boarding
In-home euthanasia
Urgent care during clinic hours

Do not include bird care unless confirmed.

Analytics QA

Before launch:

GA4 installed
GA4 real-time events work
phone_click event works
appointment_click event works
booking_form_start works if applicable
booking_form_submit works if applicable
contact_form_submit works if applicable
email_click works
directions_click works
google_reviews_click works
service_cta_click works

After launch:

check GA4 real-time
test GBP UTM link
test direct website visit
test form submission
confirm events appear
Google Business Profile QA

Before final launch:

production website URL is correct
appointment URL is correct
UTM links are ready
phone matches GBP
address matches GBP
hours match GBP
services align with GBP
no bird mentions if not confirmed
urgent care language aligns with GBP
no 24/7 emergency conflict

GBP website URL:

https://francispetcare.ca/?utm_source=google&utm_medium=organic&utm_campaign=gbp

GBP appointment URL:

https://francispetcare.ca/book-appointment/?utm_source=google&utm_medium=organic&utm_campaign=gbp_booking

Only update GBP after final production domain is ready.

DNS / Vercel Launch QA

For staging:

attach test.francispethospital.ca
confirm CNAME points to Vercel
confirm SSL

For production:

Before DNS change:

confirm Vercel project is production-ready
confirm domain settings in Vercel
confirm old WordPress site backup exists
confirm rollback plan

After DNS change:

production domain loads
HTTPS active
www/non-www behavior correct
redirects work
sitemap accessible
robots correct
forms work
analytics works
GoDaddy DNS Notes

Do not change email/MX records.

Do not break Zoho Mail or any existing email system.

For subdomain testing:

Type: CNAME
Host: test
Value: cname.vercel-dns.com

For final launch, use Vercel’s exact recommended records.

Do not change production DNS until QA is complete.

Performance QA

Run Lighthouse/PageSpeed after staging deployment.

Check:

mobile performance
desktop performance
LCP
CLS
accessibility
best practices
SEO

Fix:

unoptimized hero image
layout shifts
oversized video
excessive JS
missing alt text
insufficient contrast
inaccessible forms
Mobile QA

Test on mobile width.

Required:

hero readable without zoom
CTAs visible above fold
sticky call/book bar works
menu opens/closes
service cards stack cleanly
appointment form usable
doctor cards readable
review cards readable
footer usable
no horizontal scroll
phone links work
Browser QA

Test:

Chrome
Safari
iPhone Safari
Android Chrome if available
desktop 1440px
laptop 1280px
tablet width
mobile 390px
Accessibility QA

Check:

keyboard navigation
focus states
contrast
labels
aria where needed
alt text
semantic buttons/links
no empty links
no div-only buttons
no heading skips that harm readability
Post-Launch Monitoring

First 24 hours:

check homepage
check service pages
test forms
check GA4
check Search Console
check Vercel logs
check 404s
check redirects
check GBP links if updated

First 7 days:

monitor GSC indexing
monitor GA4 events
monitor form submissions
monitor calls if tracked
monitor rankings manually
check 404s
fix missing redirects

First 30 days:

monitor rankings for:
animal hospital Richmond BC
pet hospital Richmond BC
vet Richmond BC
exotic pet vet Richmond
rabbit vet Richmond
reptile vet Richmond
rabbit dental Richmond
exotic pet surgery Richmond
pet dental Richmond
in-home pet euthanasia Richmond
monitor GBP:
calls
website clicks
booking clicks
directions
search terms
review growth
Rollback Plan

Before launch, keep:

WordPress backup
old DNS settings screenshot
Vercel deployment history
GitHub commit before launch
redirect map
launch checklist completion record

If serious issue occurs:

revert DNS to old hosting or previous deployment
restore previous Vercel deployment
pause GBP URL changes if not already made
fix issue
relaunch after QA
Final Approval Checklist

Do not launch until these are approved:

design quality
homepage content
service page content
doctor bios
review usage
no-go claims check
forms
tracking
schema
redirects
mobile UX
Vercel deployment
DNS plan
rollback plan

Final approval owner:
TODO: Add approver name.

Launch date:
TODO.

Production domain:
TODO.

Staging domain:
test.francispethospital.ca
