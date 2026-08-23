# Perspective Suite

A hub-and-spoke portal of linkable pages, one per domain, that together show one person reading across adjacent fields. Each spoke is a discrete URL sent for a role-fit; the suite nav exposes the siblings so a single link lands on the primary and indicates breadth.

Built to `Perspective_Suite_Spec_v1_0.md`. Greenfield, single pass. Supersedes the two prior GitHub sites.

## Structure

```
index.html            Hub: through-line statement + spoke directory
adoption-change.html  AI Adoption & Change   (Tier 1, first-person authoritative)
gtm-bizdev.html       GTM & BizDev           (Tier 1, first-person authoritative)
data-analytics.html   Data & Analytics       (Tier 2, practitioner-with-perspective)
ai-factory.html       AI Factory Stack       (Tier 3, observer/translator)
assets/suite.css      Shared shell: tokens, type, top bar, hero, section, cards, routes, footer
```

Register tiers are a construction decision only. They are never printed, labeled, or named on any page.

## Design system

Paper-and-forest. Barlow Condensed / Inter / IBM Plex Mono, green-and-umber over a paper ground.

The shared shell is **inlined into every page** so each spoke is fully self-contained and renders styled when opened on its own, with no external dependency. `assets/suite.css` is kept as the canonical master source: edit it there, then re-inline into the pages (replace each page's inlined shell block), or edit a page directly for a one-off. Page-specific diagram CSS lives in a second `<style>` block on each page.

## Landing-page hierarchy

The hub does not give all four domains equal weight. The two home-turf spokes (Adoption & Change, GTM & BizDev) are featured as the primary pair. The two adjacency reads (Data & Analytics, AI Factory) sit beneath them in a lighter "Other perspectives" panel, and in the nav they live under an "Other perspectives" dropdown rather than as top-level items.

Green is the credible/practitioner accent; umber is the attention/current accent. On the Tier 2 and Tier 3 pages the split is visual: opinionated POV content in green, observer-register map content in neutrals, "where the industry missteps" callouts in umber.

## Through-line

AI's constraint moved from "can we build it" to "will the organization adopt it and can we prove it moved the business." Each spoke expresses that in its domain:

- Adoption & Change: the discipline itself, direct.
- GTM & BizDev: the discipline applied to revenue, direct.
- Data & Analytics: the lab-to-applied gap.
- AI Factory Stack: the infrastructure-to-applied gap, one layer down.

## Deploy

Static. Enable GitHub Pages on the default branch, root. No build step, no dependencies beyond the Google Fonts link in each page head.

## Cross-linking

Hub links every spoke. Every spoke's top-bar nav links every other spoke and the hub. Each spoke's "where to go" routes to one or two most-related siblings plus a conversation path. No dead ends.
