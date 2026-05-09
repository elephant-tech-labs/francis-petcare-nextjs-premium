Below is the Phase 1 rebuild blueprint I’d use before development for Francis Petcare Hospital.

**1. Final Recommendation**

Rebuild in **Next.js + Vercel** instead of continuing to patch WordPress.

The current WordPress site has too much accumulated risk: Elementor/theme debt, WooCommerce clutter, AIOSEO index bloat, broken links, demo copy, wrong emergency language, unconfirmed bird content, Catcare/Karen brand confusion, and unclear form/conversion tracking.

A clean Next.js rebuild gives Francis Petcare:

- faster page speed and cleaner Core Web Vitals
- precise control over titles, metadata, schema, canonicals, and redirects
- fewer plugin conflicts
- cleaner tracking for calls, forms, GBP clicks, and appointment intent
- a tighter conversion path on mobile
- a more serious medical brand presentation
- better protection against accidental WordPress/plugin SEO bloat

WordPress should stay live until the new site is complete, QA’d, redirected, and ready to launch.

---

# 2. Phase 1 Site Scope

Phase 1 should be focused. The goal is not to create a giant site; the goal is to launch the smallest site that can rank, convert, and clarify Francis Petcare’s positioning.

**Phase 1 launch pages:**

1. Homepage
2. Veterinary Services overview
3. Exotic Pet Vet Richmond
4. Rabbit Vet Richmond
5. Reptile Vet Richmond
6. Rabbit Dental Care Richmond
7. Exotic Pet Surgery Richmond
8. Pet Dental Care Richmond
9. Surgery, Spay & Neuter
10. Urgent Care Vet Richmond
11. Cat Boarding Richmond
12. In-Home Pet Euthanasia Richmond
13. About / Team
14. Contact / Book Appointment
15. FAQ

**Not Phase 1 unless confirmed later:**

- Bird care page
- Individual pages for ferrets, guinea pigs, hamsters, hedgehogs, snakes, and lizards
- Blog
- Online store
- Coupon-heavy landing pages
- WooCommerce functionality

---

# 3. Final Sitemap

| Page | URL Slug | SEO Purpose | Target Intent | Priority | Phase |
|---|---|---:|---|---:|---|
| Homepage | `/` | Rank for core hospital + exotic positioning | animal hospital Richmond BC, exotic pet vet Richmond | Critical | Phase 1 |
| Services | `/veterinary-services/` | Service hub and internal linking | veterinary services Richmond BC | High | Phase 1 |
| Exotic Pet Vet | `/exotic-pet-vet-richmond-bc/` | Main differentiator page | exotic pet vet Richmond, exotic vet near me | Critical | Phase 1 |
| Rabbit Vet | `/rabbit-vet-richmond-bc/` | Species-specific local ranking | rabbit vet Richmond BC | Critical | Phase 1 |
| Reptile Vet | `/reptile-vet-richmond-bc/` | Species-specific exotic ranking | reptile vet Richmond BC | High | Phase 1 |
| Rabbit Dental Care | `/rabbit-dental-care-richmond-bc/` | High-value exotic service page | rabbit dental care Richmond | Critical | Phase 1 |
| Exotic Pet Surgery | `/exotic-pet-surgery-richmond-bc/` | High-value exotic service page | exotic pet surgery Richmond | Critical | Phase 1 |
| Pet Dental Care | `/pet-dental-care-richmond-bc/` | Core dog/cat service ranking | pet dental care Richmond BC | High | Phase 1 |
| Surgery / Spay & Neuter | `/pet-surgery-spay-neuter-richmond-bc/` | Core surgical service ranking | pet surgery Richmond, spay neuter Richmond | High | Phase 1 |
| Urgent Care | `/urgent-care-vet-richmond-bc/` | Replace bad 24/7 emergency language | urgent care vet Richmond, same day vet Richmond | Critical | Phase 1 |
| Cat Boarding | `/cat-boarding-richmond-bc/` | GBP secondary category support | cat boarding Richmond BC | Medium | Phase 1 |
| In-Home Euthanasia | `/in-home-pet-euthanasia-richmond-bc/` | Sensitive high-intent service | in home pet euthanasia Richmond | High | Phase 1 |
| About / Team | `/about/` | Trust, doctors, local proof | Francis Petcare doctors, animal hospital team | High | Phase 1 |
| Contact / Booking | `/contact/` | Calls, forms, directions | vet appointment Richmond BC | Critical | Phase 1 |
| FAQ | `/faq/` | Objection handling + FAQ schema | clinic hours, urgent care, exotic pets | Medium | Phase 1 |
| Ferret Vet | `/ferret-vet-richmond-bc/` | Species expansion | ferret vet Richmond | Medium | Phase 2 |
| Guinea Pig Vet | `/guinea-pig-vet-richmond-bc/` | Species expansion | guinea pig vet Richmond | Medium | Phase 2 |
| Small Mammal Vet | `/small-mammal-vet-richmond-bc/` | Broader exotic coverage | hamster hedgehog vet Richmond | Medium | Phase 2 |
| Blog / Pet Care Articles | `/resources/` | Long-tail SEO | rabbit teeth, reptile care, dental signs | Low | Phase 2 |

---

# 4. Homepage Wireframe

## Section 1: Hero

**Goal:** Immediately clarify who Francis Petcare is and why to call.

**Copy angle:**  
“Animal Hospital & Exotic Pet Vet in Richmond, BC”

**Trust purpose:**  
Position as a real local hospital, not a generic clinic or old Catcare brand.

**SEO purpose:**  
Strong H1 with Richmond + animal hospital + exotic pet vet language.

**Conversion purpose:**  
Push phone calls and appointment requests above the fold.

**CTA:**  
Primary: `Book Appointment`  
Secondary: `Call Francis Petcare`

Recommended hero copy:

**H1:** Animal Hospital & Exotic Pet Vet in Richmond, BC  
**Subheadline:** Veterinary care for cats, dogs, rabbits, reptiles, ferrets, guinea pigs, hamsters, hedgehogs, snakes, and lizards, with same-day urgent care available during clinic hours.

No bird mention. No 24/7 emergency claim.

---

## Section 2: Fast Action Bar

**Goal:** Make mobile and desktop conversion immediate.

**Copy angle:**  
Call, book, get directions.

**Trust purpose:**  
Shows clinic is accessible and local.

**SEO purpose:**  
NAP consistency.

**Conversion purpose:**  
Reduce friction.

**CTA:**  
`Call Now`, `Book Appointment`, `Get Directions`

---

## Section 3: Core Services Snapshot

**Goal:** Show breadth without overwhelming.

**Copy angle:**  
“Complete care for everyday visits, urgent concerns, surgery, dental care, and exotics.”

**Trust purpose:**  
Signals full-service hospital.

**SEO purpose:**  
Internal links to service pages.

**Conversion purpose:**  
Let users self-select.

**CTA:**  
`View Veterinary Services`

Cards:

- Wellness & Preventive Care
- Dental Care
- Surgery, Spay & Neuter
- Urgent Care During Clinic Hours
- Exotic Pet Care
- Cat Boarding
- In-Home Euthanasia

---

## Section 4: Exotic Pet Care Feature

**Goal:** Make exotic care the central differentiator.

**Copy angle:**  
“Care for rabbits, reptiles, and small mammals requires a clinic comfortable with species-specific needs.”

**Trust purpose:**  
Shows capability without overclaiming.

**SEO purpose:**  
Internal links to exotic, rabbit, reptile, rabbit dental, exotic surgery pages.

**Conversion purpose:**  
Route exotic owners directly to booking.

**CTA:**  
`Explore Exotic Pet Care`

---

## Section 5: Rabbit Dental + Exotic Surgery Highlight

**Goal:** Promote high-value, newly added GBP services.

**Copy angle:**  
“Specialized care for complex exotic needs.”

**Trust purpose:**  
Build authority around services many clinics do not offer.

**SEO purpose:**  
Support Rabbit Dental Care and Exotic Pet Surgery pages.

**Conversion purpose:**  
Encourage calls for condition-specific questions.

**CTA:**  
`Call About Exotic Care`

---

## Section 6: Same-Day Urgent Care

**Goal:** Replace false 24/7 emergency claims with safe, honest language.

**Copy angle:**  
“Same-day urgent appointments may be available during clinic hours. Please call ahead.”

**Trust purpose:**  
Transparent and medically responsible.

**SEO purpose:**  
Rank for urgent care vet Richmond.

**Conversion purpose:**  
Drive phone calls, not passive form fills.

**CTA:**  
`Call for Urgent Care Availability`

---

## Section 7: Meet the Team

**Goal:** Repair trust bottleneck and humanize the clinic.

**Copy angle:**  
“Experienced veterinary care from a local Richmond team.”

**Trust purpose:**  
Doctor/team proof matters because rating is currently a bottleneck.

**SEO purpose:**  
Entity and local trust support.

**Conversion purpose:**  
Reduce hesitation.

**CTA:**  
`Meet Our Team`

---

## Section 8: Reviews / Reputation Section

**Goal:** Use real reviews honestly while acknowledging trust through action.

**Copy angle:**  
“Pet owners choose Francis Petcare for accessible, compassionate care.”

**Trust purpose:**  
Show recent positive real feedback only. No fake reviews, no review gating.

**SEO purpose:**  
Supports local conversion, not direct markup abuse.

**Conversion purpose:**  
Encourage confidence.

**CTA:**  
`Read Reviews` / `Book Appointment`

Important: do not add aggregate review schema unless compliant and sourced correctly.

---

## Section 9: New Patient Offer

**Goal:** Keep the existing offer but stop making it the whole brand.

**Copy angle:**  
“New to Francis Petcare? Ask about current new patient offers.”

**Trust purpose:**  
Offer supports trial, but hospital quality remains the lead.

**SEO purpose:**  
Minimal.

**Conversion purpose:**  
Encourage first appointment.

**CTA:**  
`Book First Visit`

---

## Section 10: Location / Contact

**Goal:** Make Richmond relevance unmistakable.

**Copy angle:**  
“Located in Richmond, BC.”

**Trust purpose:**  
NAP, map, hours, parking/visit info.

**SEO purpose:**  
LocalBusiness schema + NAP consistency.

**Conversion purpose:**  
Calls, directions, appointments.

**CTA:**  
`Get Directions`

---

# 5. Page Templates

## Service Page Template

Use for dental, surgery, urgent care, cat boarding.

Sections:

1. Hero with service + Richmond
2. Who this service is for
3. Common reasons to book
4. What to expect
5. Related services
6. Doctor/team trust block
7. FAQs
8. Final CTA

Primary CTA: `Book Appointment`  
Urgent care CTA: `Call Now`

Schema: `Service`, `FAQPage`, `BreadcrumbList`, local business reference.

---

## Exotic Pet Page Template

Use for main exotic care page.

Sections:

1. Hero: Exotic Pet Vet in Richmond, BC
2. Species treated, excluding birds
3. Why exotic pets need species-aware care
4. Common exotic pet visits
5. Rabbit dental and exotic surgery links
6. Urgent signs: call the clinic
7. Team trust
8. FAQs
9. CTA

Primary CTA: `Book Exotic Pet Appointment`  
Secondary CTA: `Call About Your Pet`

---

## Species Page Template

Use for rabbit and reptile Phase 1 pages.

Sections:

1. Hero: species + Richmond
2. Common health concerns
3. Preventive care
4. Dental/surgery relevance where applicable
5. When to call urgently
6. Related exotic services
7. FAQs
8. CTA

No diagnosis-heavy medical advice.

---

## Doctor / Team Page Template

Sections:

1. Hero: Meet Francis Petcare Hospital
2. Clinic positioning
3. Doctor/team profiles
4. Exotic care capability
5. Hospital values
6. Real photos
7. CTA

Schema: `VeterinaryCare` / `LocalBusiness`, `Person` only if credentials are confirmed.

---

## In-Home Euthanasia Page Template

Tone should be calm, compassionate, and plain.

Sections:

1. Hero: In-Home Pet Euthanasia in Richmond, BC
2. Gentle explanation
3. When families consider this service
4. What to expect
5. Service area disclaimer
6. Aftercare options if confirmed
7. FAQs
8. Phone-first CTA

Primary CTA: `Call to Discuss Availability`  
Secondary CTA: `Contact the Clinic`

---

## Contact / Book Appointment Template

Sections:

1. Hero: Book an Appointment
2. Phone, address, hours, directions
3. Booking form
4. Urgent care callout
5. New patient offer callout
6. Parking / arrival notes
7. Map
8. FAQ mini-block

Primary CTA: `Call Now`  
Secondary CTA: `Submit Appointment Request`

---

## FAQ Page Template

Sections:

1. Hero
2. Appointment FAQs
3. Exotic pet FAQs
4. Urgent care FAQs
5. Dental/surgery FAQs
6. Cat boarding FAQs
7. Euthanasia FAQs
8. CTA

Schema: `FAQPage`

---

# 6. Content Briefs For Launch Pages

## Homepage

**SEO Title:** Animal Hospital & Exotic Pet Vet in Richmond, BC | Francis Petcare Hospital  
**Meta Description:** Francis Petcare Hospital provides veterinary care for cats, dogs, rabbits, reptiles, and small mammals in Richmond, BC. Book an appointment or call for same-day urgent care availability during clinic hours.  
**H1:** Animal Hospital & Exotic Pet Vet in Richmond, BC  
**Hero Headline:** Animal Hospital & Exotic Pet Vet in Richmond, BC  
**Hero Subheadline:** Veterinary care for cats, dogs, rabbits, reptiles, ferrets, guinea pigs, hamsters, hedgehogs, snakes, and lizards. Same-day urgent care may be available during clinic hours.  
**Primary CTA:** Book Appointment  
**Secondary CTA:** Call Now  
**Required Sections:** Hero, action bar, services, exotic care, rabbit dental/exotic surgery, urgent care, team, reviews, offer, location.  
**FAQs:** Do you treat exotic pets? Do you offer urgent care? Do you treat birds? Do you offer cat boarding?  
**Internal Links:** Services, Exotic Pet Vet, Rabbit Vet, Reptile Vet, Contact.  
**Schema:** LocalBusiness/VeterinaryCare, WebPage, BreadcrumbList, FAQPage if FAQs are visible.

---

## Veterinary Services

**SEO Title:** Veterinary Services in Richmond, BC | Francis Petcare Hospital  
**Meta Description:** Explore veterinary services at Francis Petcare Hospital, including wellness care, dental care, surgery, urgent care, cat boarding, exotic pet care, and in-home euthanasia.  
**H1:** Veterinary Services in Richmond, BC  
**Hero Headline:** Full-Service Veterinary Care for Richmond Pets  
**Hero Subheadline:** From preventive care to dental procedures, surgery, urgent visits, and exotic pet care, our team supports cats, dogs, rabbits, reptiles, and small mammals.  
**Primary CTA:** Book Appointment  
**Secondary CTA:** Call the Clinic  
**Required Sections:** Service grid, exotic care feature, urgent care note, related pages, CTA.  
**FAQs:** What services do you offer? Do you treat exotic pets? Do you offer same-day appointments?  
**Internal Links:** All service pages.  
**Schema:** CollectionPage, Service, BreadcrumbList, FAQPage.

---

## Exotic Pet Vet

**SEO Title:** Exotic Pet Vet in Richmond, BC | Rabbits, Reptiles & Small Mammals  
**Meta Description:** Francis Petcare Hospital provides exotic pet veterinary care in Richmond, BC for rabbits, reptiles, ferrets, guinea pigs, hamsters, hedgehogs, snakes, and lizards.  
**H1:** Exotic Pet Vet in Richmond, BC  
**Hero Headline:** Veterinary Care for Exotic Pets in Richmond  
**Hero Subheadline:** Exotic pets need species-aware veterinary care. Francis Petcare Hospital sees rabbits, reptiles, ferrets, guinea pigs, hamsters, hedgehogs, snakes, and lizards.  
**Primary CTA:** Book Exotic Pet Appointment  
**Secondary CTA:** Call About Your Pet  
**Required Sections:** Species treated, common visit reasons, rabbit dental care, exotic surgery, urgent signs, FAQs.  
**FAQs:** What exotic pets do you treat? Do you treat birds? Do rabbits need dental care? Do you provide exotic pet surgery?  
**Internal Links:** Rabbit Vet, Reptile Vet, Rabbit Dental, Exotic Surgery, Contact.  
**Schema:** Service, FAQPage, BreadcrumbList.

---

## Rabbit Vet

**SEO Title:** Rabbit Vet in Richmond, BC | Francis Petcare Hospital  
**Meta Description:** Rabbit veterinary care in Richmond, BC, including wellness visits, dental concerns, appetite changes, and surgery consultations at Francis Petcare Hospital.  
**H1:** Rabbit Vet in Richmond, BC  
**Hero Headline:** Rabbit Veterinary Care in Richmond  
**Hero Subheadline:** Rabbits have unique health and dental needs. Our team provides veterinary care for rabbits, including exams, dental evaluations, and surgery consultations.  
**Primary CTA:** Book Rabbit Appointment  
**Secondary CTA:** Call About Rabbit Care  
**Required Sections:** Why rabbits need specialized care, dental signs, appetite/stool urgency, preventive care, related services.  
**FAQs:** Do rabbits need regular vet visits? What are signs of dental problems? When should I call urgently?  
**Internal Links:** Exotic Pet Vet, Rabbit Dental Care, Exotic Surgery, Contact.  
**Schema:** Service, FAQPage, BreadcrumbList.

---

## Reptile Vet

**SEO Title:** Reptile Vet in Richmond, BC | Francis Petcare Hospital  
**Meta Description:** Reptile veterinary care in Richmond, BC for snakes, lizards, and other confirmed reptiles. Book an appointment with Francis Petcare Hospital.  
**H1:** Reptile Vet in Richmond, BC  
**Hero Headline:** Reptile Veterinary Care in Richmond  
**Hero Subheadline:** Reptiles require careful handling and species-aware veterinary care. Francis Petcare Hospital sees reptiles including snakes and lizards.  
**Primary CTA:** Book Reptile Appointment  
**Secondary CTA:** Call About Reptile Care  
**Required Sections:** Species treated, common reasons for visits, husbandry-aware care, surgery/urgent notes, FAQs.  
**FAQs:** Do you see snakes and lizards? Should I bring habitat details? When should I call the clinic?  
**Internal Links:** Exotic Pet Vet, Exotic Surgery, Urgent Care, Contact.  
**Schema:** Service, FAQPage, BreadcrumbList.

---

## Rabbit Dental Care

**SEO Title:** Rabbit Dental Care in Richmond, BC | Francis Petcare Hospital  
**Meta Description:** Rabbit dental care in Richmond, BC for overgrown teeth, eating changes, drooling, and suspected dental discomfort. Call Francis Petcare Hospital.  
**H1:** Rabbit Dental Care in Richmond, BC  
**Hero Headline:** Dental Care for Rabbits in Richmond  
**Hero Subheadline:** Rabbit dental issues can affect eating, comfort, and overall health. Francis Petcare Hospital provides rabbit dental evaluations and care planning.  
**Primary CTA:** Book Rabbit Dental Visit  
**Secondary CTA:** Call About Symptoms  
**Required Sections:** Signs of dental issues, why rabbit teeth matter, what to expect, urgent signs, related exotic care.  
**FAQs:** What are signs of rabbit dental problems? Is not eating urgent? Do rabbits need dental checks?  
**Internal Links:** Rabbit Vet, Exotic Pet Vet, Exotic Surgery, Contact.  
**Schema:** Service, FAQPage, BreadcrumbList.

---

## Exotic Pet Surgery

**SEO Title:** Exotic Pet Surgery in Richmond, BC | Francis Petcare Hospital  
**Meta Description:** Exotic pet surgery consultations and surgical care in Richmond, BC for confirmed species including rabbits, reptiles, and small mammals. Call to discuss your pet’s needs.  
**H1:** Exotic Pet Surgery in Richmond, BC  
**Hero Headline:** Surgical Care for Exotic Pets  
**Hero Subheadline:** Francis Petcare Hospital provides surgical consultations and care planning for exotic pets, including rabbits, reptiles, and small mammals.  
**Primary CTA:** Call About Exotic Surgery  
**Secondary CTA:** Book Consultation  
**Required Sections:** Surgery scope disclaimer, pre-surgical exam, species considerations, recovery, related services.  
**FAQs:** What exotic pets do you perform surgery on? Is a consultation required? How do I prepare?  
**Internal Links:** Exotic Pet Vet, Rabbit Vet, Reptile Vet, Contact.  
**Schema:** Service, FAQPage, BreadcrumbList.

---

## Pet Dental Care

**SEO Title:** Pet Dental Care in Richmond, BC | Dog & Cat Dental Services  
**Meta Description:** Pet dental care in Richmond, BC for dogs and cats, including dental exams, cleanings, and treatment planning at Francis Petcare Hospital.  
**H1:** Pet Dental Care in Richmond, BC  
**Hero Headline:** Dental Care for Dogs and Cats  
**Hero Subheadline:** Dental health affects your pet’s comfort and overall wellness. Our team provides dental evaluations and care for dogs and cats.  
**Primary CTA:** Book Dental Appointment  
**Secondary CTA:** Call the Clinic  
**Required Sections:** Signs of dental disease, dental exam process, cleanings/treatment planning, related rabbit dental link.  
**FAQs:** How do I know if my pet has dental pain? Do pets need dental cleanings? Do you offer rabbit dental care?  
**Internal Links:** Services, Rabbit Dental Care, Contact.  
**Schema:** Service, FAQPage, BreadcrumbList.

---

## Surgery / Spay & Neuter

**SEO Title:** Pet Surgery, Spay & Neuter in Richmond, BC | Francis Petcare Hospital  
**Meta Description:** Veterinary surgery, spay, and neuter services in Richmond, BC for pets. Book a surgical consultation with Francis Petcare Hospital.  
**H1:** Pet Surgery, Spay & Neuter in Richmond, BC  
**Hero Headline:** Veterinary Surgery for Richmond Pets  
**Hero Subheadline:** Francis Petcare Hospital provides surgical consultations and common procedures including spay and neuter care.  
**Primary CTA:** Book Surgical Consultation  
**Secondary CTA:** Call the Clinic  
**Required Sections:** Procedures, pre-surgical exam, safety planning, recovery, exotic surgery link.  
**FAQs:** Do you offer spay and neuter? Is an exam required first? Do you perform exotic pet surgery?  
**Internal Links:** Exotic Surgery, Services, Contact.  
**Schema:** Service, FAQPage, BreadcrumbList.

---

## Urgent Care

**SEO Title:** Urgent Care Vet in Richmond, BC | Same-Day Availability During Clinic Hours  
**Meta Description:** Francis Petcare Hospital offers urgent veterinary care during clinic hours when same-day appointments are available. Call ahead for urgent concerns in Richmond, BC.  
**H1:** Urgent Care Vet in Richmond, BC  
**Hero Headline:** Urgent Veterinary Care During Clinic Hours  
**Hero Subheadline:** If your pet needs timely care, call Francis Petcare Hospital. Same-day urgent appointments may be available during regular clinic hours.  
**Primary CTA:** Call Now  
**Secondary CTA:** Book Appointment  
**Required Sections:** What urgent care means, when to call, not 24/7 emergency disclaimer, exotic urgent concerns, contact block.  
**FAQs:** Are you a 24/7 emergency hospital? Do you offer same-day appointments? Should I call before coming in?  
**Internal Links:** Contact, Exotic Pet Vet, Rabbit Vet, Services.  
**Schema:** Service, FAQPage, BreadcrumbList.

---

## Cat Boarding

**SEO Title:** Cat Boarding in Richmond, BC | Francis Petcare Hospital  
**Meta Description:** Cat boarding in Richmond, BC at Francis Petcare Hospital. Call to ask about availability, requirements, and booking.  
**H1:** Cat Boarding in Richmond, BC  
**Hero Headline:** Cat Boarding at Francis Petcare Hospital  
**Hero Subheadline:** Francis Petcare Hospital offers cat boarding for Richmond families. Call to confirm availability, requirements, and booking details.  
**Primary CTA:** Call About Cat Boarding  
**Secondary CTA:** Book Appointment  
**Required Sections:** Boarding overview, requirements, what to bring, availability disclaimer, contact.  
**FAQs:** Do I need to book ahead? Are vaccines required? What should I bring?  
**Internal Links:** Services, Contact, About.  
**Schema:** Service, FAQPage, BreadcrumbList.

---

## In-Home Pet Euthanasia

**SEO Title:** In-Home Pet Euthanasia in Richmond, BC | Francis Petcare Hospital  
**Meta Description:** Compassionate in-home pet euthanasia in Richmond, BC. Call Francis Petcare Hospital to discuss availability and next steps.  
**H1:** In-Home Pet Euthanasia in Richmond, BC  
**Hero Headline:** Compassionate In-Home Pet Euthanasia  
**Hero Subheadline:** When it is time to say goodbye, our team can help families understand available options with care and respect.  
**Primary CTA:** Call to Discuss Availability  
**Secondary CTA:** Contact the Clinic  
**Required Sections:** Gentle intro, what to expect, service area, aftercare if confirmed, FAQs.  
**FAQs:** Do you offer in-home euthanasia? What areas do you serve? How do I know when to call?  
**Internal Links:** Contact, About.  
**Schema:** Service, FAQPage, BreadcrumbList.

---

## About / Team

**SEO Title:** About Francis Petcare Hospital | Richmond, BC Animal Hospital  
**Meta Description:** Meet Francis Petcare Hospital, a Richmond, BC animal hospital providing care for cats, dogs, rabbits, reptiles, and small mammals.  
**H1:** About Francis Petcare Hospital  
**Hero Headline:** A Richmond Animal Hospital for Dogs, Cats, and Exotic Pets  
**Hero Subheadline:** Francis Petcare Hospital provides local veterinary care with a focus on clear communication, compassion, and species-aware care.  
**Primary CTA:** Book Appointment  
**Secondary CTA:** Call the Clinic  
**Required Sections:** Clinic story, team, doctor proof, exotic care positioning, hospital photos, CTA.  
**FAQs:** What pets do you see? Where are you located? How do I book?  
**Internal Links:** Exotic Pet Vet, Services, Contact.  
**Schema:** AboutPage, LocalBusiness/VeterinaryCare, BreadcrumbList.

---

## Contact / Book Appointment

**SEO Title:** Contact Francis Petcare Hospital | Book a Vet Appointment in Richmond, BC  
**Meta Description:** Contact Francis Petcare Hospital in Richmond, BC to book an appointment, call the clinic, or get directions.  
**H1:** Contact Francis Petcare Hospital  
**Hero Headline:** Book an Appointment  
**Hero Subheadline:** Call Francis Petcare Hospital or request an appointment online. For urgent concerns, please call during clinic hours.  
**Primary CTA:** Call Now  
**Secondary CTA:** Request Appointment  
**Required Sections:** Phone, form, address, hours, map, urgent care note, new patient offer, email.  
**FAQs:** Should I call for urgent concerns? How do I request an appointment? Where are you located?  
**Internal Links:** Urgent Care, Services, FAQ.  
**Schema:** ContactPage, LocalBusiness/VeterinaryCare, BreadcrumbList.

---

## FAQ

**SEO Title:** Francis Petcare Hospital FAQ | Richmond Vet Questions  
**Meta Description:** Answers to common questions about appointments, exotic pet care, urgent care, cat boarding, dental care, and in-home euthanasia at Francis Petcare Hospital.  
**H1:** Frequently Asked Questions  
**Hero Headline:** Questions About Visiting Francis Petcare Hospital  
**Hero Subheadline:** Find quick answers about appointments, exotic pet care, urgent visits, boarding, and services.  
**Primary CTA:** Book Appointment  
**Secondary CTA:** Call the Clinic  
**Required Sections:** Appointment, exotic, urgent care, dental/surgery, boarding, euthanasia.  
**FAQs:** All visible questions should be eligible for FAQ schema.  
**Internal Links:** Contact, Exotic Pet Vet, Urgent Care, Services.  
**Schema:** FAQPage, BreadcrumbList.

---

# 7. Conversion Architecture

**Mobile sticky call button**

- Sticky bottom bar on mobile.
- Buttons: `Call`, `Book`, `Directions`.
- For urgent care pages, `Call` should be visually primary.

**Booking CTA**

- Use consistent `Book Appointment`.
- On exotic pages: `Book Exotic Pet Appointment`.
- On urgent care: `Call Now`.

**Phone CTA**

- Phone number should be clickable everywhere.
- Above fold on homepage.
- Sticky on mobile.
- Repeated at bottom of every page.

**Form flow**

Recommended fields:

- Name
- Phone
- Email
- Pet species
- Pet name
- New or existing client
- Preferred appointment date
- Reason for visit
- Urgent concern checkbox
- Consent to contact

After submit:

- Thank-you state
- “If this is urgent, please call the clinic.”
- Track form submission event
- Send email notification
- Optional Google Sheet / CRM capture

**Trust signals**

Use:

- real hospital photos
- real team photos
- doctor names and credentials if confirmed
- Richmond address and map
- species treated
- years/experience only if verified
- recent real reviews
- clear urgent care limitations

**Review usage**

Use only real reviews. Do not fabricate, rewrite, or gate.

Best placement:

- homepage trust section
- service page sidebar/CTA area
- contact page near form
- about page

**Doctor proof usage**

Doctor/team proof should appear on:

- homepage
- About page
- exotic page
- rabbit dental page
- exotic surgery page

**Emergency / urgent care wording**

Use:

> Same-day urgent care may be available during regular clinic hours. Please call ahead.

Avoid:

- 24/7 emergency
- emergency hospital
- always open
- walk in anytime
- critical care facility unless confirmed

**New patient offer placement**

Use sparingly:

- homepage lower-middle
- contact page near form
- optional thin banner
- not the H1
- not the main brand message

---

# 8. SEO Architecture

**Metadata system**

Every page needs:

- unique title
- unique meta description
- one H1
- canonical URL
- Open Graph title/description/image
- no accidental indexable utility pages

**Canonical rules**

- Each page self-canonicalizes.
- No query parameters indexed.
- No duplicate trailing slash variants.
- Old WordPress URLs redirect to clean canonical destinations.

**Sitemap**

Generate XML sitemap with only indexable public pages.

Include:

- Phase 1 pages
- no admin pages
- no attachment pages
- no Elementor templates
- no WooCommerce URLs
- no tag/category bloat unless resources launch later

**robots.txt**

Allow public pages. Block non-public technical routes.

Do not block the whole site.

**Redirect requirements**

Create a redirect map from old WordPress URLs to new URLs.

Known fixes:

- old emergency page should redirect to `/urgent-care-vet-richmond-bc/`
- broken `/service` should redirect to `/veterinary-services/`
- broken absolute URL paths should redirect to their correct service pages
- WooCommerce pages should either 410 or redirect to relevant pages
- duplicate privacy/terms should resolve to one canonical page if retained

**Schema**

Use:

- `VeterinaryCare` / `LocalBusiness`
- `Service`
- `FAQPage`
- `BreadcrumbList`
- `ContactPage`
- `AboutPage`

Avoid unsupported medical claims.

**Image alt-text strategy**

Alt text should describe real content and local/service relevance.

Examples:

- “Francis Petcare Hospital exterior in Richmond BC”
- “Veterinary team examining a rabbit”
- “Cat boarding area at Francis Petcare Hospital”

Avoid keyword stuffing.

**Internal linking strategy**

Homepage links to all priority service pages.  
Services page links to every service page.  
Exotic page links to rabbit, reptile, rabbit dental, exotic surgery.  
Rabbit page links to rabbit dental.  
Urgent care page links to contact and exotic care.  
Every page links to contact.

---

# 9. Tracking Architecture

**GA4 events**

Track:

- `click_call`
- `click_book_appointment`
- `click_directions`
- `click_email`
- `form_start`
- `form_submit`
- `form_error`
- `urgent_call_click`
- `exotic_booking_click`
- `new_patient_offer_click`

**Google Search Console**

- Verify domain property if possible.
- Submit new sitemap after launch.
- Inspect homepage and top service pages immediately after launch.

**GBP UTM links**

Use UTM-tagged links from Google Business Profile.

Example structure:

- Website: `/?utm_source=google&utm_medium=organic&utm_campaign=gbp`
- Appointment: `/contact/?utm_source=google&utm_medium=organic&utm_campaign=gbp_booking`
- Services/posts can use campaign-specific UTMs.

**Phone click tracking**

All `tel:` links should trigger GA4 events.

Separate tracking for:

- homepage phone click
- sticky mobile phone click
- urgent care phone click
- contact page phone click

**Booking form tracking**

Track:

- form view
- field start
- successful submit
- validation error
- source page
- pet species selected
- urgent concern checkbox

**Contact form tracking**

Same as booking form, with conversion event in GA4.

**Email click tracking**

Track all `mailto:` clicks, but do not treat email clicks as primary conversions.

---

# 10. Migration Checklist

**Before launch**

1. Crawl current WordPress site.
2. Export all live URLs.
3. Export indexed URLs from GSC.
4. Identify top traffic pages.
5. Identify backlinks if available.
6. Create redirect map.
7. Confirm NAP.
8. Confirm exact phone, hours, services, species, and booking email.
9. Confirm no bird care language.
10. Confirm no 24/7 emergency language.

**Redirect handling**

- Map every valuable old URL to the closest new page.
- Redirect irrelevant demo/plugin pages to homepage only if there is no better match.
- Consider 410 for pure junk URLs if they have no SEO value.
- Fix broken service links.
- Remove WooCommerce URLs from index.

**Launch**

1. Deploy production Vercel site.
2. Connect domain.
3. Force HTTPS.
4. Test redirects.
5. Submit sitemap.
6. Update GBP website and appointment links if URLs change.
7. Verify GA4 events.
8. Verify form delivery.
9. Inspect key pages in GSC.

**Post-launch QA**

Check:

- mobile sticky buttons
- phone links
- appointment form
- map/directions link
- schema validation
- sitemap availability
- robots.txt
- canonical tags
- redirects
- 404s
- speed
- desktop and mobile layout
- no birds
- no 24/7 emergency language
- no Catcare/Karen confusion

---

# 11. Design Direction

The site should feel:

- medical
- warm
- local
- trustworthy
- calm
- premium
- practical
- mobile-first
- clearly exotic-capable

It should not feel:

- like a generic SaaS startup
- flashy
- coupon-heavy
- overly playful
- like a stock veterinary template
- like an exotic-only clinic
- like a legacy WordPress demo site

Visual direction:

- clean white/soft neutral medical base
- restrained accent color
- real hospital/team/pet photography
- strong readable typography
- clear service navigation
- high-contrast CTAs
- calm spacing
- no cluttered hero
- no fake review walls
- no oversized coupon messaging

The homepage should make the clinic look established and competent within the first screen.

---

# 12. Development Plan

**Step 1: Setup**

- Create Next.js project.
- Configure Vercel.
- Set routing structure.
- Add SEO defaults.
- Add environment variables for forms/tracking.

**Step 2: Design System**

- Define typography.
- Define colors.
- Define buttons.
- Define cards.
- Define service grids.
- Define CTA blocks.
- Define mobile sticky action bar.

**Step 3: Homepage**

- Build homepage sections in final order.
- Add service links.
- Add exotic care differentiator.
- Add urgent care wording.
- Add trust/reviews/team blocks.

**Step 4: Service Pages**

- Build reusable page templates.
- Create launch service pages.
- Add FAQs and internal links.

**Step 5: Forms**

- Build contact/booking form.
- Configure delivery.
- Add validation.
- Add thank-you state.
- Add urgent care callout.

**Step 6: Schema**

- Add LocalBusiness/VeterinaryCare schema.
- Add Service schema.
- Add FAQ schema.
- Add Breadcrumb schema.

**Step 7: Tracking**

- Add GA4.
- Track CTA clicks.
- Track phone clicks.
- Track form events.
- Track GBP UTM traffic.

**Step 8: Migration**

- Crawl old WordPress site.
- Build redirect map.
- Add redirects.
- Test 301 behavior.

**Step 9: QA**

- Mobile QA.
- Desktop QA.
- Form QA.
- Tracking QA.
- Schema QA.
- SEO QA.
- Copy compliance QA.

**Step 10: Launch**

- Connect domain.
- Submit sitemap.
- Inspect key URLs in GSC.
- Monitor 404s, calls, forms, rankings, and GBP behavior.

The north star for Phase 1: **rank for Richmond animal hospital + exotic pet vet searches, make the clinic look more trustworthy, and turn mobile visitors into calls or appointment requests.**
