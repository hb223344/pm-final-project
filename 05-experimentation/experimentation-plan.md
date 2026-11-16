# Experimentation Plan (Module 5)

## Get your documents ready
- **From M3, your hypothesis sentence:** Based on Lena’s frustration that she “could not see in one place what I owe” (N-07), and on activity dropping from 77.6% to 51.0% in the two months after users’ first bills, I believe that giving heavy pay-later users like Lena one screen with one total and one clear reminder will keep them using the card after their first bill arrives. I’ll measure this as a 5-point increase in the share of heavy users still buying the month after their first bill. I will protect partner merchant share of volume (at or above 63.1%) and make a go/no-go decision after 12 weeks.
- **From M3, your primary success metric & guardrail metric:** Primary: share of heavy users still buying in the month after their first bill.
Guardrail: partner merchant share of card volume, at or above 63.1%.
- **From M4, the feature you scoped in your PRD this is what you're testing:** B3: One balance view for card and regular pay-later orders.

## Define your experiment parameters
- **Feature under test pull from your M4 PRD:** Feature under test
B3, one balance view.

Control: today’s app, with the card balance and pay-later orders on two separate screens.
Variant: one screen showing a single total owed (card plus pay-later orders), a list of each item with its amount and due date, and the next due date highlighted at the top.
Out of scope: no change to payment terms or reminder timing (that’s B8).
- **Persona pull your M2 persona:** Lena, 32, a heavy pay-later user who shops mostly on her phone, has two or three pay-later apps, and lives on a middling salary with little cushion.
- **Expected outcome the behaviour change you expect, from your M3 hypothesis:** Heavy users keep using the card after their first bill arrives, instead of fading out.
- **Primary success metric the one number that defines success, from M3:** Share of heavy users who make at least one purchase in the month after their first bill.
- **Baseline rate today's rate of your primary metric, from your M3 data:** 66.3%. That’s the weighted average of month-after-activation activity across the three groups in cohort_activity.csv (66.3%, 69.2% and 64.0%). The pack doesn’t split this by heavy users, so treat it as an approximate starting point.
- **Guardrail metric & boundary what must not break, and how far it can move before you investigate:** Partner merchant share of card volume (baseline 63.1%). Investigate if the variant falls more than 3 points below control. I picked 3 points because the monthly figure already swings between 56.8% and 63.1%, so a smaller drop could just be noise.
- **Minimum Detectable Effect (MDE) the smallest improvement worth shipping, your floor:** +5 percentage points, from 66.3% to 71.3%. Anything smaller isn’t worth the engineering time.
- **Sample size per arm use the calculator in the builder, baseline + MDE:** About 1,350 users per arm, about 2,700 in total. That’s my calculation at 95% confidence and 80% power. Check it against the builder’s calculator, which may round slightly differently.
- **Traffic split & test duration 50/50 standard · cover ≥ 2 weekly cycles:** _(not filled in)_
- **Significance threshold p < 0.05 is standard, explain any deviation:** _(not filled in)_

## Define your control and variant
- **Control (A) the current experience, reference your M2 moment of misery and M3 funnel/workflow data:** Today’s app. The card balance and regular pay-later orders are on two separate screens, and Lena has to open both and add the totals herself. This is her moment of misery: she can’t tell which total is the real one (N-07, T-103), and she gets two reminders in the same week for different amounts (T-104). In the data, activity drops after the first bill, from 77.6% to 66.3% to 51.0% for the month 1 group (cohort_activity.csv).
- **Variant (B) your single change, copy the relevant screens & functional requirements from your M4 PRD:** B3: One balance view, as defined in the M4 PRD.

Screens

Home: the total owed (card plus pay-later orders), a “Next payment” banner with amount and date, and a “See everything” button.
Core: every unpaid item with shop, amount, due date and a “Card” or “Pay later” label, sorted by earliest due date first.
Confirmation: after a payment, “Paid €X to [shop],” the new total and the new next due date.

Functional requirements

The total equals the sum of all unpaid items, to the cent.
Overdue items show first, with a red “Overdue” label.
The total and next due date update within 1 second of a payment.
If the total doesn’t match the items, the app shows an error, not a number.
When nothing is owed, the app shows “All clear.”

Not in the variant (frozen out): “Due soon” labels, same-day grouping, “last updated” time, and
- **Isolation check, what has NOT changed? list everything identical between arms (app version, eligibility rules, notifications, onboarding). If something changed inadvertently, your test is compromised.:** Same app version and release, apart from the new screen
Same entry point: the variant sits where the old balance screens were
Same eligibility: new heavy users only, randomly assigned 50/50 at activation
Same onboarding, ID check and approval rules
Same payment terms, due dates, statement date and pricing
Same reminders and notifications: timing, content and channel
Same card, phone wallet setup and checkout flow
Same merchant offers and partner list
Same support scripts and help articles

## Formalize your hypothesis & shipping criteria
- **Your hypothesis (filled in):** I believe that B3, one balance view for card and pay-later orders, for heavy pay-later users like Lena, will keep them using the card after their first bill arrives. I’ll measure this as a +5 percentage point increase in the share of heavy users who make at least one purchase in the month after their first bill (baseline 66.3%), within 12 weeks, with a 50/50 split at p < 0.05. We will protect partner merchant share of card volume (no more than 3 points below control) and on-time repayment (no more than 2 points below control).
- **Your shipping criteria (filled in):** We read results once, at the end of week 12. We will SHIP if the primary metric is higher in B than A with p < 0.05, an observed lift of at least +3 points, and no guardrail breached. We will ITERATE if the lift is positive but not significant or below +3 points, with no guardrail breached. We will KILL if the lift is zero or negative, or if any guardrail is breached, whatever the primary result. The only early check is in week 1, to confirm the split is close to 50/50 and tracking works.
- **Hardest parameter to define, and did it change your hypothesis? quick debrief:** The sample size. Once I ran the numbers, I needed about 2,700 new heavy users, but the whole pilot only had 431 activated cards, so this test can’t run in the friends-and-family group.
