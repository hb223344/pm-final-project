# GTM Launch Plan, Riverty BU Pay & Credit, First Consumer Card

| Field | Value |
|---|---|
| Feature | B3: One balance view for card and regular pay-later orders |
| Goal | Engagement |
| Launch tier | M, Targeted |

## Goal & Audience
- **Goal:** Engagement, B3 lives inside the card app, so it doesn’t win new customers. Its job is to keep existing card holders using the card after their first bill, which is exactly where activity drops (77.6% → 66.3% → 51.0%). Awareness would be the wrong trap here.
- **Target audience:** Primary: card holders who are heavy pay-later users (4+ orders a month), timed around their first bill. Assumption: if 5% of the 300,000 heavy users take the card in year 1, that’s about 15,000 people. Both numbers are practice or assumed figures (gtm_audience.csv), and card take-up isn’t measurable yet.
Secondary: all other card holders, who get the same screen without targeted messages.

## Launch Tier
- **M, Targeted**, Reach: it only affects card holders, not the whole base.
Revenue: no new revenue line, just better retention of existing users.
Risk of silence: medium. Users will see the new screen anyway, but if nobody explains it at their first bill, they may still not trust the total. And if support isn’t briefed, they’ll answer the old way

## Channels
1. **Owned: in-app message on the Home screen, shown when the user opens the app before their first bill. Lena checks the app before payday (N-02), so this reaches her at exactly the right moment.**
2. **Owned: push notification and email a few days before each due date: “See everything you owe in one place.” This reaches users who don’t open the app often. Of the base, 25% allow push and 40% have opted into email (assumed practice figures).**
3. **Owned: customer support and the help centre. When someone asks “which total is the real one?” (T-103), agents point them to the one balance view, and a help article explains what’s included.  Why no paid or earned channels: the audience is already inside the product. Paying to reach your own users would waste budget.**

## Enablement & Assets
Enablement & assets

Support briefing and FAQ: what’s in the total, why Klarna and PayPal orders aren’t shown, and how card statements differ from pay-later due dates
Help article: “Your total, explained,” which also answers the credit score question (T-107)
Copy: in-app announcement, push and email texts, in German, reviewed and signed off by Compliance (money and credit messages are regulated)
Account managers: a short note for merchant account managers explaining the change and the guardrail
Where to use AI: drafting copy options and summarizing support tickets after launch
Where not to use AI: generating or explaining amounts owed, or a chatbot answering “what do I owe?” A wrong number is exactly Lena’s moment of misery, and Compliance needs every amount to be explainable.

## Ownership, Budget & Timeline
- **Ownership & budget:** PM: owns the plan, the test read, the rollout decision and post-launch metrics
Engineering lead: feature flag and staged rollout
CRM manager: push and email
Product designer: in-app announcement
Support lead: briefing, FAQ and help article
Compliance officer: sign-off on all copy
 Data analyst: dashboard and support tagging
- **Timeline:** Phase 1, beta (weeks 1–12): the M5 A/B test, 50/50 on new heavy users. Support is briefed for both groups, and the assets and Compliance sign-off are ready by week 10.
Phase 2, launch moment (weeks 13–14): ship decision at week 13. If it ships, roll out 25% → 50% → 100% over two weeks, with the in-app message and push timed to each user’s next bill.
Phase 3, post-launch (weeks 15–24): weekly metric checks and support tag reviews, then a final decision at week 24.
Budget & resource gaps

No paid media. The costs are internal time plus German copy and translation review.
Missing data: no heavy-user baseline and no count of “which total?” tickets yet. Both need setting up before launch.
Out of scope: Klarna and PayPal orders can’t be included, so the copy must not promise “everything you owe, everywhere.”

## Success Metrics
- **Metrics:** Adoption: the share of active card holders who open the one balance view in the 7 days before a due date. Target 60% or more (my assumption).
Retention: the share of heavy users still buying in the month after their first bill, from 66.3% to 71.3%.
Clarity: fewer “which total is real?” support contacts per 1,000 active cards. Set the baseline before launch.
- **Bad signal to watch for:** High adoption but no retention lift. That means Lena sees the total but still drifts away, so the real blocker is something else, like declines or habit. Rising support contacts or a drop in on-time repayment would also mean the total is confusing or misleading.
- **Likely post-launch decision:** Iterate. Adoption will likely be high, but the retention lift may land below +5, because B3 fixes the screen while the two reminders (T-104) remain. In that case, the trigger to move on to B8 (one due date) is high adoption with a small lift. Double down if the lift is +5 or more and support contacts fall.
