# Experience portfolio: Lovable update 1 (Nov 1, 2026)

Source: colleague review and decisions in chat, Nov 1 (all recommended options). Reference build: Experience_Portfolio_Update.zip (the same changes as finished HTML).

Scope: the nav label, shorter heroes, proof before "tell" on every page, the pipeline panel in the GTM & BizDev hero, the walkthrough order, and one walkthrough drawing fix. The Insights pages change only in their labels. Images, case-study popups and all copy not listed here stay as they are.

## Before you start

1. Download hero-pipeline.svg from the BizDevByDesign Website folder: https://drive.google.com/file/d/1yQBfpzUmn9tNp4RuuKR9PoPRQgBmP-LO/view
2. Upload it to the Lovable project with prompt 4.
3. Paste the prompts one at a time, in order, and check each against the list at the end.

---

## Prompt 1: Nav label, all pages

Make only these text changes, everywhere they appear. Change nothing else.
- In the top nav dropdown, "Exposure & Perspective" becomes "Insights". The dropdown items stay the same: Data & Analytics, AI Factory, Enterprise AI Stack.
- On the hub, the sidebar panel's eyebrow "Exposure & perspective" becomes "Insights". Its intro line becomes: "Perspectives on adjacent technical fields: the terrain, trends and interdependencies across complex systems."
- On the three Insights pages, the hero kicker ending "· Exposure & perspective" ends "· Insights" instead.

---

## Prompt 2: Hub page

1. Hero: keep the kicker and headline. Replace all three paragraphs under the headline with this one, in the existing lede style:
"Two decades in technology, clarifying complexity and turning strategy into action across marketing, business development, change, program leadership and AI go-to-market."

2. Add a new section directly under the hero, titled with a green mono eyebrow "Selected results". Below it, a band of three equal columns with a 2px ink top border (#181b1a) and 1px line-colored dividers between columns (#d4d8d5). No cards, no icons, no fill. On mobile it stacks to one column, with 1px rules between items. Each column is a link:
   - Figure "161,000" / label "Lowe's · employees across 1,710 stores" / text "A customer-experience behavior change, carried by a network of change agents in every store." / link "See the work →" to adoption-change.html#work
   - Figure "Board-adopted" / label "ICANN · meetings strategy" / text "A 21-person working group, stalled for a year, moved to one framework the Board adopted." / link "See the work →" to adoption-change.html#work
   - Figure "$6.8M to $10.9M" / label "XPLANE · 2007 to 2010" / text "Firm revenue growth behind the consultative selling motion built and run there." / link "See the record →" to gtm-bizdev.html#record
   Type: figure in Barlow Condensed 700, green (#1e4d34), about 36px on desktop. Label in IBM Plex Mono 10.5px uppercase, umber (#824f30). Text in Inter 14.5px graphite (#2b302e). Link in IBM Plex Mono 11.5px uppercase, green (#2c6a48).

3. Domain cards, replace the body text only:
   - AI Adoption & Change: "Fifteen years making complex change land inside enterprises, now grounded in building AI systems firsthand. Finding the real problem, then making the new way of working the default."
   - GTM & BizDev: "A consultative, relationship-led selling motion, built and run with real teams, now carried by AI and automation that handle the research, timing and targeting."

4. "Why these fit together": keep the heading. Replace its three paragraphs with this one:
"Potential is everything a technology could do. Value is the part an organization actually captures. Closing that gap is a human problem: understanding what was built, and mapping it onto the outcomes people inside the business are already trying to reach, in terms they can act on."

---

## Prompt 3: Adoption & Change page

1. Hero: keep the kicker, headline and discipline pills. Replace both paragraphs with this one, in the lede style:
"Twenty-five years making technology understandable, the last fifteen making complex change land inside enterprises. Now grounded in building AI systems firsthand."

2. Move the "Selected work" section so it sits directly under the hero, above "Approach". Replace its subhead with:
"Retail, higher education, internet governance, semiconductor manufacturing, footwear and apparel, and AI practice. Reach is stated as measured; models are labeled as models."

3. Reorder the case cards to: Lowe's ("Turning 161,000 employees into creators"), the university system ("Adoption that outlived the project"), ICANN ("Breaking a stalled working group to a Board-adopted recommendation"), semiconductor ("Mapping the flagship product-launch lifecycle for the first time"), semiconductor ("Rebuilding decision rights after a reorganization"), ICANN ("Trust in a change-fatigued community"), footwear ("Eight critical builds at once"), Sephora, XPLANE frameworks ("Frameworks and tools I helped build"), then "One operator, an agentic team". Keep the top-border colors alternating green, umber, green, umber down the new order. Each card keeps its popup.

4. Approach, now below the work: keep the heading, the "three things" lead-in and list, and the green "culture eats strategy" callout. Replace the four paragraphs after the callout with this one:
"On most of this work I held two overlapping seats: account and program lead, shaping the challenge, the proposal and the strategy, and executive relationship owner, accountable for delivery and often in the room doing it. The last two years of hands-on building AI-native systems ground that experience in what these tools actually do."

---

## Prompt 4: GTM & BizDev page

1. Hero, new layout. Keep the kicker and the headline "Relationship-led growth, carried by AI and data." at full width, then the short umber rule. Below them, two columns (about 55/45, 44px gap):
   - Left: this one paragraph in the lede style, replacing both current paragraphs: "A consultative, relationship-led selling motion, built and run with real teams, now carried by AI and data that handle the research, timing and targeting. The relationship stays human." The discipline pills sit under it, unchanged.
   - Right: a panel with a 1px line-colored border (#d4d8d5), paper background (#e9ebe9), 16px padding and square corners. Inside it, the heading "Build a sustainable relationship and opportunity pipeline." (Barlow Condensed 700, about 26px, ink), and below that the uploaded hero-pipeline.svg. Render the SVG inline, not as an img tag, so IBM Plex Mono applies to its labels, and don't edit its contents. Size only the top-level svg to width 100%: use a selector like ".panel > svg", never ".panel svg", because the file contains nested svg elements that break if they are resized. Under the panel, a link "See how it works →" in IBM Plex Mono 12px uppercase, green (#2c6a48).
   - Clicking the panel, or the link (or pressing Enter or Space on either), opens the existing three-panel walkthrough overlay. Give the panel aria-label "Open the walkthrough: Current state, Future state, The path forward" and a visible focus outline.
   - Under 900px wide, the columns stack: text first, then the panel.

2. Remove "The shift, in three panels." section entirely: the three cards, the "See the full three-panel walkthrough" bar and the paragraph under it. Keep the walkthrough overlay itself, since the new panel opens it.

3. Reorder the sections after the hero to: Track record, Capabilities, AI intelligence systems in the channel, The method, Where to go.

4. Track record:
   - Replace the subhead with "Figures are measured and drawn from the full career record."
   - Remove two cards: "The measurement discipline under the selling" and "One motion, three eras".
   - Show the remaining three cards (XPLANE, Momentive / SurveyMonkey, Sephora) in three equal columns on desktop, stacking to one column under 900px.

---

## Prompt 5: Walkthrough (experience.html)

1. Change the order to Current state, Future state, The path forward. Move the section marked data-beat="2" (eyebrow "THE RESULTS", headline "Same people. Same effort. Aimed better.") so it sits second, between the current-state section and the "A NEW PLAYBOOK FOR TODAY'S ENVIRONMENT" section. Keep its data-beat="2" attribute, because the CSS uses it. The script steps through the sections in page order.

2. Step buttons at the top, in this order, with data-go 0, 1, 2: 1 CURRENT STATE, 2 FUTURE STATE, 3 THE PATH FORWARD.

3. In the script, change the Next button labels to:
var labels=['See the future state →','How to get there →','✓ That’s the shift'];
and change the Next button's starting text to "See the future state →".

4. Drawing fix: change the CSS rule `.gfx svg{display:block;width:100%;height:auto}` to `.gfx > svg{display:block;width:100%;height:auto}`. The current rule also stretches the small svg drawings nested inside the future-state picture, which blows up the engine icon and crops the pool and chute.

---

## Check after Lovable applies it

- Every page's nav shows "Insights ▾" with the three Insights pages under it. The hub sidebar and the Insights page kickers say Insights.
- Hub: one-line hero, then the Selected results band with three linked items, then the trimmed domain cards and the one-paragraph through-line.
- Adoption & Change: one-line hero, then Selected work starting with Lowe's, then Approach with one paragraph after the callout. Card colors alternate, and every card's popup still opens.
- GTM & BizDev: two-column hero with the pipeline panel on the right. The panel and "See how it works →" both open the walkthrough. The three-card "shift" section is gone. Sections run Track record (three cards), Capabilities, Channel, Method, Where to go.
- Walkthrough: steps read Current state, Future state, The path forward. Panel 2's drawing shows the whole pool, chute and sales-plan tank, with a small engine icon at the left.
- On a phone, the GTM hero stacks, and the results band and record cards stack to one column.
