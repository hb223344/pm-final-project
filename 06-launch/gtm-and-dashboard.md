# GTM Strategy & Success Dashboard (Module 6)

## Get your prior work ready
- **The feature you're launching from your M4 PRD, one feature, not a list:** B3: One balance view. It shows everything Lena owes on the card and her pay-later orders as one total, on one screen.
- **What your M5 experiment will test your hypothesis, primary metric and ship / iterate rule, the evidence the launch rests on:** Whether one balance view lifts the share of heavy users still buying in the month after their first bill by +5 points (baseline 66.3%), while partner merchant share and on-time repayment hold. We ship if the lift is significant and at least +3 points with no guardrail breached, iterate if it’s positive but smaller, and kill if it’s flat or negative or a guardrail breaks.
- **Your persona pull your M2 persona, this anchors your audience:** Lena, 32, a heavy pay-later user who shops on her phone, has 2–3 pay-later apps, and has a middling salary with little cushion. She wants to know exactly what she owes and when.

## Set your goal, then your audience
- **Primary GTM goal awareness · engagement · conversion, pick one:** Engagement
- **Why this goal? what makes this the right goal for this feature right now:** B3 lives inside the card app, so it doesn’t win new customers. Its job is to keep card holders using the card after their first bill, which is exactly where activity drops (77.6% → 66.3% → 51.0%).
- **Target audience the specific segment your goal implies, be precise:** Primary: new heavy-user card holders (4+ pay-later orders a month), from activation through the month after their first bill. Assumption: if 5% of the 300,000 heavy users take the card in year 1, that’s about 15,000, or about 290 new ones a week. Both are practice or assumed figures (gtm_audience.csv).
Secondary: all other card holders. They see the new screen, but get no targeted messages.

## Size your launch
- **Launch tier S (minimal) · M (targeted) · L (multi-channel) · XL (full GTM):** M
- **Justification reach + revenue impact + what silence would risk:** Reach: it only affects card holders, not the whole base.
Revenue: no new revenue line, just better retention of existing users.
Risk of silence: medium. Users will see the new screen anyway, but if nobody explains it at their first bill, they may still not trust the total. And if support isn’t briefed, they’ll answer the old way
- **Is this a launch or a release? does it need go-to-market, or can it just ship?:** Launch or release?
A small launch. The screen itself could just ship, but it needs a targeted nudge at the first-bill moment and a briefed support team, so it isn’t a silent release.

## Choose your top three channels and plan assets
- **Channel 1 owned / earned / paid, and why it reaches your audience:** Owned: one added line in the existing payment reminder (push and email), linking to the one balance view: “See all your Riverty payments in one place.” It reaches users even if they’ve stopped opening the app, and it adds no new messages, so it doesn’t add to the “two reminders” problem (T-104).
- **Channel 2 owned / earned / paid, and why:** Owned: an in-app message on the Home screen the first time a user opens the app after launch. It reaches users who still check the app before payday (N-02).
- **Channel 3 owned / earned / paid, and why:** Owned: the help centre article “Your total, explained,” linked from the new screen. It’s for users who want to check what’s in the total and whether it affects their credit score (T-107).

No paid or earned channels: the audience is already inside the product. No launch messages are sent during the A/B test, to keep notifications the same in both groups.
- **Enablement & assets what Sales / CS / Support need, plus the assets to build (one-pager, demo, etc.):** Support briefing and FAQ: what’s in the total, why Klarna and PayPal aren’t included, and how card statements differ from pay-later due dates
Copy: the reminder line, the in-app message and the help article, in German, signed off by Compliance
Merchant note: a short note for merchant account managers explaining the change and the guardrail
Copy rule: never say “everything you owe,” only “all your Riverty payments”
Where to use AI: drafting copy options and summarizing support tickets
Where not to use AI: generating or explaining amounts owed, or a chatbot answering “what do I owe?”

## Make it executable
- **Ownership named owner per key activity, individual, not department:** PM: plan, test read, rollout decision, post-launch metrics
 Engineering lead: feature flag, staged rollout and rollback
 CRM manager: reminder line in push and email
 Product designer: in-app message
 Content writer: German copy and help article
 Support lead: briefing and FAQ
 Compliance officer: copy sign-off, with the review slot booked now
 Account management lead: merchant note
 Data analyst: baselines, dashboard and support tags
- **Budget & resource gaps what costs extra, and any asset you can't currently build:** No paid media. The costs are internal time plus German copy review.
Missing data: no heavy-user baseline and no count of “which total?” tickets yet. Both need setting up before launch.
Can’t build: Klarna and PayPal orders in the view.
Risk: Compliance sign-off is a dependency, so book it early.
- **Timeline Phase 1 beta → Phase 2 launch moment → Phase 3 post-launch:** Phase 1, beta (weeks 1–18): the M5 A/B test, 50/50 on new heavy users. About 10 weeks to enroll 1,347 per arm at roughly 290 a week, then 8 weeks of follow-up. Assets and Compliance sign-off are ready by week 16.
Phase 2, launch moment (weeks 19–20): ship decision at week 19. If it ships, roll out 25% → 50% → 95%, keeping a 5% holdout. Add the reminder line and in-app message.
Phase 3, post-launch (weeks 21–30): weekly checks. Roll back within 24 hours if the error state shows in more than 0.1% of sessions. Final decision at week 30.

## Define how you'll know it worked
- **Success metrics 2 to 3 metrics that match your GTM goal:** Retention: the share of heavy users still buying in the month after their first bill, from 66.3% to 71.3%, compared with the 5% holdout.
Check-and-pay: the share of card holders who check the one balance view before a due date and then pay on time. Set the baseline before launch.
Clarity: “which total is real?” support contacts per 1,000 active cards fall. Set the baseline before launch.
- **Bad signal to watch for e.g. high reach, zero signups = message-market mismatch:** Early, in week 1: support contacts aren’t falling, the error state shows in more than 0.1% of sessions, or reminder opt-outs rise.
Later: people check the view but retention doesn’t lift, which means the real blocker is something else, like declines or habit.
- **Most likely post-launch decision double-down · iterate · pivot · deprioritize, and what would trigger it:** Iterate. Checking will likely be high, but the lift may land below +5, because the separate reminders (T-104) still exist. The trigger to move on to B8 (one due date) is high check-and-pay with a small retention lift. Double down if the lift is +5 or more and support contacts fall.
