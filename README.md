🏠 NaijaRent
Find Your Space, Own Your Peace
Nigeria's verified, AI-powered rental marketplace — live, transparent, and built for every Nigerian.

📋 Table of Contents

1.  The Problem
2.  The Solution
3.  Features
4.  Three AI Models — RentMatch · RentRec · EcoTrace
5.  User Roles
6.  Technology Stack
7.  Getting Started
8.  Demo Accounts
9. Roadmap
10. License & Author


### 1. The Problem
House hunting in Nigeria is broken — and it hurts millions of people every year.

Problem	Reality
🏚️  **Agent extortion:**	Local agents charge illegal fees of 15–20% annual rent — cash only, no receipts, no accountability, no recourse for tenants.
⏳  **Exhausting search:** 	Tenants spend weeks or months visiting fake, misrepresented, or already-taken properties before finding anything real.
💸  **Hidden costs:**  	Agreement, caution, and agent fees only appear at signing — when the tenant is already emotionally invested and pressured to proceed.
♿  **Inaccessibility:** 	No Nigerian rental platform collects accessibility data. Persons with disabilities cannot evaluate properties remotely.
🔇  **No tenant voice:**	There is no formal channel to report bad landlords, fraudulent agents, or scam listings.
💵  **Cash only:**	No digital payment trail means disputes are unresolvable and theft is undetectable.



### 2. The Solution
NaijaRent is a single-file, fully operational web application that eliminates every one of these problems through verified listings, capped fees, AI guidance, and transparent digital payments.

•	🔒  No hidden fees — full itemised breakdown before every payment
•	🤖  Three AI models — recommendation engine, financial advisor, environmental monitor
•	♿  Remote-first — persons with disabilities can complete the full rental journey from home
•	🌱  Environmental data — Nigeria's first property-level air quality and eco-score database
•	📱  PWA-ready — install on Android or iPhone, no app store needed
•	☁️  Cloud-native — Firebase Firestore for real-time persistent data across all devices



### 3.  Features
For Tenants
•	Personalised recommendations powered by RentMatch AI engine
•	AI financial advisor (RentRec) — budget analysis, fee explanations, red flag detection
•	Browse and filter by city, property type, price range, occupancy, and EcoTrace grade
•	Full media gallery (photos + videos) per listing — evaluate any property remotely
•	Apply, pay, and track — all in-platform with full audit trail
•	Save listings, file complaints, message landlords directly
•	Screen-reader compatible layout, mobile bottom navigation

For Landlords & Agents
•	Create and edit listings anytime — auto re-submission for admin approval on each edit
•	Review applications with NIN last-4 verification and next-of-kin details
•	Toggle occupancy status manually or automatically via payment
•	Track earnings with full transaction history and split receipts
•	Message tenants directly from any listing

For Admin
•	Approve or reject listings and affiliate agent applications
•	Full user management across all roles
•	Transaction oversight with complete fee breakdowns
•	Complaints queue — 9 categories, 4 resolution stages (Open → Reviewing → Resolved → Dismissed)

Platform-Wide
•	15 verified demo listings across 10 Nigerian cities
•	8 pre-loaded demo accounts across all roles
•	Responsive design with full mobile and tablet navigation (v10)
•	Installable PWA with service worker caching
•	Firebase Firestore real-time cloud database


### 4.  Three AI Models
🏠  RentMatch — Recommendation Engine
Custom-built · No external API · Always free
A weighted multi-factor scoring algorithm that ranks every verified listing for each tenant in real time.

Score  =  (Affordability × 0.4)  +  (Location × 0.3)  +  (Type × 0.2)  +  (Amenities × 0.1)

Tier	Score	Meaning
🟢  Comfortable	≥ 70	Rent below 30% of annual income
🟡  Stretch	40 – 69	Achievable with budgeting
🔴  Aspirational	< 40	Above comfortable range



💬  RentRec — AI Financial Advisor
Powered by Google Gemini AI (gemini-2.0-flash-lite) · Free tier
A conversational AI chatbot embedded in the tenant dashboard:
•	Personalised income-to-rent affordability analysis
•	Plain-language explanations of Nigerian rental fees
•	Document checklist before signing any tenancy agreement
•	Red flag and scam pattern detection
•	Nigerian rental law and tenant rights guidance
•	Full session memory — greets tenants by name

🌱  EcoTrace — Environmental Monitor
Powered by OpenWeatherMap Air Pollution API · Free tier · 1,000 calls/day
Nigeria's first property-level environmental database. Data collected per listing:
•	⚡  Power source — Solar / Hybrid / NEPA-only / Generator
•	💧  Water source — Pipe-borne / Borehole / Tanker / Well
•	🗑️  Waste disposal — Recycling / Gov Truck / Private / Open burning
•	🌊  Flood history — Never / Occasionally / Frequently

Live AQI layer — fetches real PM2.5, PM10, and AQI for all 10 cities. Falls back to a population-density model when live data is unavailable.

Grade	Score	Meaning
A	90–120	Excellent environmental conditions
B	75–89	Good
C	60–74	Moderate
D	40–59	Poor
E	0–39	Very Poor


###  5.  User Roles
Role	Access	Registration
🏠  Tenant:	Browse, apply, pay, RentRec, RentMatch, EcoTrace, complaints	Username + NIN + next-of-kin details
🏢  Landlord:	List properties, review applications, track earnings	Username + bank details
🤝  Agent:	Same as landlord + verified agent badge	Admin approval required
💼  Affiliate: Agent	List properties, earn 10% per deal	NIN + bank details + admin approval
⚡  Admin:	Full platform control	Pre-configured


###  6.  Technology Stack
Layer	Technology	Notes
Frontend	HTML5 · CSS3 · Vanilla JavaScript	Single optimised file, no build step
Database	Google Firebase Firestore	Real-time, persistent, cloud-native
AI — RentRec	Google Gemini AI (gemini-2.0-flash-lite)	Free tier
AI — RentMatch	Custom weighted scoring engine	No external API
AI — EcoTrace	OpenWeatherMap Air Pollution API	Free tier · 1,000 calls/day
Hosting	Netlify	Global CDN · HTTPS · Instant deploy
PWA	Service Worker + Web App Manifest	Installable on Android and iOS
Identity	NIN capture + role-based access control	Firebase security rules

Zero dependencies. No build step. Open in any browser and run.


###  7.  Getting Started
Option 1 — Use it live (recommended)
Visit naijarent.netlify.app — no setup required. Use any of the demo accounts below.



###  8.  Demo Accounts
All demo passwords are demo123 (admin: admin123).

Role	            Username	        Notes
Tenant	          chioma_naija	    Lagos-based, salary N150k/month
Tenant	          adewale_ibadan	  Ibadan-based
Tenant	          fatima_abuja	    Abuja-based
Landlord	        emeka_landlord	  Multiple Lagos listings
Landlord	        mrs_bello	        Abuja listings
Agent	            tunde_agent	      Verified agent badge
Affiliate Agent	  amaka_affiliate   Akure listings
Admin	admin_nr	    Password: admin123


###  9.  Roadmap
Version	Feature
v10  ✅	EcoTrace environmental monitoring · Mobile navigation · Platform fee 15%
v11	  Paystack / Flutterwave payment gateway integration
v12	  Accessibility data fields and filter per listing
v13	  Virtual 360° property tours
v14	  Rent-to-own pipeline and instalment payment plans
v15	  Commercial property listings
v16	  All 36 Nigerian states + FCT onboarding
Future	Native Android and iOS apps



###  10.  License & Author
This project is licensed under the MIT License.

Author	Olanrewaju Joseph Sunday
Platform	NaijaRent — Built with purpose. Designed for Nigeria.
Live URL	naijarent.netlify.app
Bank	GTBank · Account: 0235949599
Stack	Firebase · Google Gemini AI · OpenWeatherMap · PWA · Netlify


