# Story Bank — Master STAR+R Stories

This file accumulates your best interview stories over time. Each evaluation (Block F) adds new stories here. Instead of memorizing 100 answers, maintain 5-10 deep stories that you can bend to answer almost any behavioral question.

## How it works

1. Every time `/career-ops oferta` generates Block F (Interview Plan), new STAR+R stories get appended here
2. Before your next interview, review this file — your stories are already organized by theme
3. The "Big Three" questions can be answered with stories from this bank:
   - "Tell me about yourself" → combine 2-3 stories into a narrative
   - "Tell me about your most impactful project" → pick your highest-impact story
   - "Tell me about a conflict you resolved" → find a story with a Reflection

## Stories

<!-- Stories will be added here as you evaluate offers -->
<!-- Format:
### [Theme] Story Title
**Source:** Report #NNN — Company — Role
**S (Situation):** ...
**T (Task):** ...
**A (Action):** ...
**R (Result):** ...
**Reflection:** What I learned / what I'd do differently
**Best for questions about:** [list of question types this story answers]
-->

---

### [Delivery] CHARGE.AI — Concept to Play Store
**Source:** Report #001 — Aithon — Flutter Developer
**S:** Cross-team Flutter project at Mulytic Energy building an EV charging app.
**T:** Ship production-quality app to Google Play Store, integrating Google Maps and SSLCOMMERZ payment.
**A:** Led Flutter frontend, integrated GraphQL API, Google Maps for real-time station location, SSLCOMMERZ for payment processing. Collaborated with design, backend, and QA teams through Scrum.
**R:** CHARGE.AI published on Google Play Store. Full delivery from concept to production.
**Reflection:** Would add automated widget tests earlier in the cycle — manual QA caught UI regressions that automated tests would have caught cheaper.
**Best for:** "Tell me about a project you shipped", "cross-team collaboration", "mobile app delivery", "Tell me about yourself"

---

### [State Management] Multi-project State Strategy — DeshIT-BD
**Source:** Report #001 — Aithon — Flutter Developer
**S:** Delivering 3+ concurrent client projects at DeshIT-BD as a junior developer, each with different complexity.
**T:** Choose and implement the right state management approach per project without a senior to guide the decision.
**A:** Used Provider for simple widget-level state, GetX for reactive patterns on more complex screens. Made the call independently on each project.
**R:** All 3 projects delivered to production. No state-related regressions reported post-launch.
**Reflection:** Learned to match state solution to complexity, not to habit. Overengineering state in small apps wastes time; under-engineering in complex ones creates bugs.
**Best for:** "Flutter state management", "technical decision-making", "working independently", "junior to mid growth"

---

### [Real-time Systems] Digital Menu WebSocket — DeshIT-BD
**Source:** Report #001 — Aithon — Flutter Developer
**S:** Building a QR-based digital menu system at DeshIT-BD for a restaurant client.
**T:** Kitchen and front-of-house staff needed live order updates without polling.
**A:** Implemented WebSocket connection for real-time order push to kitchen display. Used REST for standard CRUD (menu items, orders). Added reconnection retry handler after initial drop issues.
**R:** Real-time order system in production. No order sync delays reported.
**Reflection:** WebSocket connections drop silently — learned to always implement reconnection logic with exponential backoff. Would do this from day one next time.
**Best for:** "Real-time systems", "REST vs WebSocket decision", "debugging in production", "technical problem-solving"

---

### [Debugging] Production Bug Fix — Metal Plus / Grameenphone
**Source:** Report #001 — Aithon — Flutter Developer
**S:** Production bug in Grameenphone telecom integration at Metal Plus, live system.
**T:** Diagnose and fix without downtime, sole engineer on the project.
**A:** Used Sentry error monitoring to identify exact stacktrace. Isolated the failure to an API response shape change on Grameenphone's side. Deployed a patch same day with graceful fallback.
**R:** Zero downtime. Fixed within hours of detection.
**Reflection:** Production monitoring setup is always worth the upfront cost. Without Sentry, this would have taken hours of blind debugging instead of minutes of targeted reading.
**Best for:** "Debugging under pressure", "production incident", "working independently", "monitoring and observability"

---

### [Full-stack Ownership] Event Platform — Metal Plus (Sole Engineer)
**Source:** Report #001 — Aithon — Flutter Developer
**S:** Metal Plus needed an internal event management platform with no team to build it.
**T:** Architect and deliver the full product end-to-end as the only engineer.
**A:** Designed system architecture, built Flutter frontend, built Go backend with REST APIs, containerized with Docker, deployed to AWS.
**R:** Platform delivered to production, used across concurrent organizational events.
**Reflection:** Being the only engineer forces rigorous scope decisions — you can't build everything. Learned to define MVP ruthlessly and defer nice-to-haves.
**Best for:** "Full-stack experience", "ownership and autonomy", "architecture decisions", "Tell me about your most complex project", startup/founding engineer interviews
