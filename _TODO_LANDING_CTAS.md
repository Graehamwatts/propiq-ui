# ⚠️ Open loop — Landing page CTAs will 404 until built

**File:** `propcast-landing.html`
**Status:** Live, but two CTA destinations don't exist yet.

## Dead links to fix after the next screens are built

| Where it lives | Target href | Build status | Tie back in when |
|---|---|---|---|
| Nav bar "Start free" button | `propcast-signup.html` | Not built | Signup screen shipped |
| Hero "Start free — no card required" | `propcast-signup.html` | Not built | Signup screen shipped |
| Closing CTA "Start free — see my market" | `propcast-signup.html` | Not built | Signup screen shipped |
| Nav "Pricing" anchor | `#pricing` (works — on-page anchor) | ✅ Live | — |

## Build order reminder (per Graeham's direction, April 16 2026)

1. ✅ Landing page (`propcast-landing.html`)
2. ⏭️ **NEXT:** Signup / hook-input screen (`propcast-signup.html`) — Step 1 of Hook-First Funnel per PropCast NX
3. Hook analysis result (`propcast-hook-analysis.html`) — Step 2, free value before any recording ask (addresses F6)
4. Pricing page (`propcast-pricing.html`) — if we want a standalone deep-dive beyond the landing section
5. Onboarding rebuild (`propcast-onboarding.html`) — already exists, to be updated
6. Recording scorecard (`propcast-recording-scorecard.html`)
7. Execute dashboard (`propcast-execute.html`)

## Once signup + pricing screens are built

Search-replace in `propcast-landing.html`:
- Both instances of `href="propcast-signup.html"` → confirm file exists, no change needed
- If a standalone pricing page is built, consider updating `href="#pricing"` in the nav to `propcast-pricing.html` for users who want the deep-dive page

## Don't delete this file until

All three signup-linked CTAs are verified to land on a real page (not a 404), AND the landing page has been smoke-tested on mobile + desktop.
