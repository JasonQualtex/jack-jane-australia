# Jack & Jane — Australia University Visit

This is the single working copy of the itinerary. Everything — itinerary
days, the Checklist tab, styling and JS — lives in one file: `index.html`.
There are no separate CSS/JS files to keep in sync.

**Editing this file:** GitHub's web editor (pencil icon on `index.html`) works
for small text changes. For anything bigger, it's easier to download the
file, edit locally, then use "Upload files" at the repo root to replace
`index.html` (same filename = same file, so this just updates it — no need
to delete the old one first) and commit.

**Checklist sync:** the Checklist tab syncs ticks/notes across devices via a
Firebase Realtime Database. The URL is set in the `SYNC_URL` constant near
the top of the `<script>` block. If sync ever stops working, check that
constant first — everything falls back to local-device-only storage
(`localStorage`) if the URL is unset or unreachable.

**Day structure:** each day is one object in the `DAYS` array (search for
`id:"mon21"` etc. to jump to a specific day) with a `html` template literal
for its content. Cards use consistent classes (`.card`, `.flag`, `.plain`,
`.transit`, `.flight`) — copy an existing card's markup rather than
inventing new structure.

## 2026-09-14
- Monash (Mon 21): added confirmed on-campus accommodation tour (1:30–2:15pm, 58 College Way), alongside the existing 10am Engineering tour
- UQ (Fri 25): added a confirmed St Leo's College card (2:30pm); reordered the three accommodation options chronologically — International House (10am, TBC) → Kev Carmody House (1pm, TBC) → St Leo's College (2:30pm, confirmed); trimmed each to a one-line status
- UQ: added "Hockey turfs on campus" to Visit Objectives
- Added hockey club links for Newcastle and UQ (matching Monash's existing one); all three (Monash/Newcastle/UQ) now point to the clubs' Facebook pages rather than official websites, since the Facebook pages had more current content
- Removed all parking/driving references throughout (Newcastle Car Park 2, St Leo's driving directions, hotel confirmation "Parking" rows) — trip is not self-driving at any location


## 2026-09-11
- Shortened checklist item titles/descriptions; CCRF folded into Application Systems
- Key Dates: removed subtitle, moved deadline times into detail view, kept only early-bird/timely dates, dropped hard deadlines and the "other requested deadlines" section

## 2026-09-11 (earlier)
- Added checklist and Key Dates accordions, fact-checked deadline info
