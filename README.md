KaribAfrika
Africa–Caribbean Digital Trade & Collaboration Platform

A production-ready web platform connecting African and Caribbean entrepreneurs, SMEs, creatives, and investors for cross-regional trade, investment, and collaboration.

Live Demo: https://YOUR-SITE.netlify.app
Developer: Oladimeji Ayanleke
Organisation: Honorary Consulate of Barbados in Rwanda
Institution: African Leadership University (ALU)
Version: 1.0 — Sprint 1 (Frontend Prototype)

Table of Contents

Project Overview
Problem Statement
Proposed Solution
Features Built
System Requirements Coverage
Tech Stack
Project Structure
How to Run Locally
How to Deploy
Screens & Navigation
Design System
Development Model
Author


1. Project Overview
KaribAfrika is a centralised digital platform built to facilitate business cooperation, trade discovery, investment matching, and cultural collaboration between African and Caribbean communities.
The platform was developed as a final-year software engineering project at the African Leadership University (ALU), following a full Software Requirements Specification (SRS) process that included problem research, stakeholder analysis, UML system design (Use Case, Class, Sequence, and Component diagrams), and Agile sprint planning.

2. Problem Statement
Africa and the Caribbean share deep historical, cultural, and social ties. Political frameworks such as Africa–CARICOM Summits and trade forums have reinforced commitments toward stronger economic cooperation. However, despite this momentum, Africa–Caribbean trade and investment remain significantly underdeveloped and fragmented at the private-sector level.
Key barriers identified through research:
BarrierDescriptionInformation asymmetryBusinesses on both sides do not know what opportunities exist across regionsNo unified platformThere is no verified digital space for Africa–Caribbean business discoveryInformal networksEntrepreneurs rely on personal contacts with no structured discovery mechanismRegulatory fragmentationDifferent legal and trade frameworks create coordination gapsLimited market intelligenceSMEs lack access to cross-regional data and qualified partners
This was confirmed through primary research including attendance at the Africa-Caribbean Trade and Investment Webinar hosted by the Africa Business Council, the CARICOM Private Sector Organisation, and the International Trade Centre with support from Afreximbank (January 2026).
Investment flows to Africa dropped to $45 billion in 2022 and 2023 (UNCTAD), and SMEs in developing regions face persistent barriers due to weak digital trade infrastructure and coordination gaps (World Bank, 2024).

3. Proposed Solution
KaribAfrika addresses these barriers by providing:

A centralised opportunity feed covering trade, investment, creative, and event listings
Real-time search and filtering by keyword, category, and region
Direct messaging between users across both regions
Profile management for entrepreneurs, SMEs, investors, and institutions
Event listings for summits, webinars, and trade fairs
Admin moderation for platform content quality control
Analytics dashboard for platform usage insights

SMART Hypothesis: Within one year, the creation and implementation of KaribAfrika will result in tangible increases in cross-border partnerships, trade opportunities, and investment collaborations among African and Caribbean SMEs and creatives — measured by registered users, partnerships formed, and opportunities posted.

4. Features Built
Fully Functional in This Release
FeatureDescriptionLanding pageHero section, feature cards, stats, footerUser Registration (FR1)Role selection, full form validation, inline errors, loading statesUser Authentication (FR2)Login with validation, name personalisation throughout the appProfile Management (FR3)Full profile page with bio, skills, listings, and statsOpportunity Posting (FR4)4-type selector, live preview, form validation, success confirmationOpportunity Browsing (FR5)12 listings, real-time search, category filters, region filter, sort, empty statesMessaging (FR6)Multi-conversation chat, send/receive, auto-reply, conversation searchEvent Listings (FR7)4 events with registration, confirmed state, category filtersAdmin Moderation (FR8)KPI dashboard, approve/reject with live status updatesAnalytics Dashboard (FR9)KPI cards, bar chart, donut chart, country breakdown tableNotificationsDropdown with unread state and mark all readMobile ResponsiveFull responsive layout with mobile bottom navigation bar

5. System Requirements Coverage
Functional Requirements
IDRequirementStatusFR1User Registration✅ CompleteFR2User Authentication✅ CompleteFR3Profile Management✅ CompleteFR4Opportunity Posting✅ CompleteFR5Opportunity Browsing & Search✅ CompleteFR6Messaging✅ CompleteFR7Event Listings✅ CompleteFR8Admin Moderation✅ CompleteFR9Analytics Dashboard✅ Complete
Non-Functional Requirements
IDRequirementHow MetNFR1SecurityHTTPS on Netlify. Input validation on all forms.NFR2PerformanceSingle-file, zero dependencies, fast loadNFR3UsabilityInline errors, empty states, loading indicators, clear labelsNFR4ScalabilityModular code, ready for backend in Sprint 2NFR5ReliabilityNetlify CDN — global availabilityNFR6CompatibilityChrome, Edge, Firefox, Safari — desktop and mobileNFR7MaintainabilityCSS variables, modular JS functions, well-commented

6. Tech Stack
LayerTechnologyReasonMarkupHTML5Semantic, accessible structureStylingCSS3 + CSS VariablesConsistent design system tokensLogicVanilla JavaScriptNo framework overhead for prototypeFontsGoogle Fonts — Libre Baskerville + OutfitPremium editorial + clean UI pairingIconsInline SVGZero dependencies, crisp at all sizesDeploymentNetlifyFree, fast, HTTPS automatic, global CDNVersion ControlGitHubPublic repository for assessment
Sprint 2 planned: React.js · Node.js · Express.js · PostgreSQL · JWT Auth · Socket.io

7. Project Structure
karibafrika/
│
├── index.html        # Complete application — all screens, CSS, and JS
├── README.md         # This documentation file
│
└── docs/
    └── SRS.pdf       # Software Requirements Specification

The prototype is self-contained in a single file for portability and ease of assessment. Sprint 2 separates this into a full component-based architecture with a live backend.


8. How to Run Locally
Option 1 — Open directly (zero setup)
bash# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/karibafrika.git

# 2. Navigate into the folder
cd karibafrika

# 3. Open in your browser

# Mac:
open index.html

# Windows:
start index.html

# Linux:
xdg-open index.html
Option 2 — Local server with Node.js
bash# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/karibafrika.git
cd karibafrika

# 2. Install serve globally (one-time)
npm install -g serve

# 3. Start the server
serve .

# 4. Open your browser at:
http://localhost:3000
Option 3 — Local server with Python
bash# Python 3
python -m http.server 8000

# Then open: http://localhost:8000
Option 4 — VS Code Live Server

Install the Live Server extension in VS Code
Open the project folder
Right-click index.html
Select Open with Live Server


9. How to Deploy
Netlify Drop (fastest — 2 minutes, no account needed)

Go to netlify.com/drop
Drag your index.html file onto the page
Wait 30 seconds
Copy your live URL — done

Netlify with GitHub (auto-deploys on every push)

Create a free account at netlify.com
Click Add new site → Import an existing project
Connect GitHub and select this repository
Leave all settings as default
Click Deploy site
Go to Site Settings → Change site name → set karibafrika
Live at https://karibafrika.netlify.app


10. Screens & Navigation
ScreenHow to AccessFR CoveredLanding PageDefault on load—RegisterClick Get StartedFR1LoginClick Sign InFR2Opportunities FeedDefault after loginFR5Opportunity DetailClick any cardFR5Post OpportunityClick + Post OpportunityFR4MessagesMessages in navFR6EventsEvents in navFR7My ProfileProfile in navFR3Admin PanelAdmin in navFR8AnalyticsAnalytics in navFR9NotificationsBell icon in top nav—
How to use the search (FR5):

Type any keyword in the large search bar — cards filter instantly
Select a region from the dropdown — cards filter by location
Click a category chip — shows only that category
Change the sort order — reorders results

How to use messaging (FR6):

Click any conversation in the left panel to open it
Type in the input field and press Enter or click send
The other party will auto-reply within 1.5 seconds
Search conversations using the search input


11. Design System
Colour Palette
NameHexUsageForest#1B3A2DPrimary brand colourGold#C9972AAccent and highlightsIvory#FAFAF7Page backgroundWhite#FFFFFFCard surfacesSand#F0EBE1Secondary backgroundsInk#1A1A18Primary textMuted#7A7A72Secondary textRed#C0392BErrors and deadlines
Typography
FontRoleLibre BaskervilleAll headings and display text — editorial, authoritativeOutfitAll UI text, labels, buttons — clean and modern

12. Development Model
Agile (Iterative) — ISO/IEC 33202:2024
SprintDeliverableStatus
Sprint 1Full frontend prototype — all 9 FRs, mobile responsive, deployed✅ 
Sprint 2Backend — Node.js, Express, PostgreSQL, JWT, Socket.io Planned
Sprint 3Production — email, file uploads, testing, scaling Planned

13. Author
Oladimeji Ayanleke
African Leadership University (ALU) · Kigali, Rwanda · 2026

LinkURLLive Site(https://karibafrika.netlify.app/)
GitHub Repo[Replace with your GitHub URL]
SRS Document (https://docs.google.com/document/d/1AXvp4KUXvWvBp6L_8ZBtKowOeTjzGv0Yw9Oq7VOg_hc/edit?usp=sharing)
Video Presentation[Replace with your video link]

