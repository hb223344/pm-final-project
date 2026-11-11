# Hypothesis & Success Metrics (Module 3)

## Pre-work · Hypothesis check
- **Role , who you are solving for (from M2):** Lena, 32, a heavy pay-later user who shops mostly on her phone, has two or three pay-later apps installed, and lives on a middling salary with little cushion
- **Goal , what this user is ultimately trying to achieve:** She wants to always know exactly what she owes and when it’s due, all in one place, so payday never brings surprises.
- **Friction / moment of misery , the specific pain blocking their goal:** Her card balance and her normal pay-later orders showed up on two different screens, so she couldn’t tell which total was the real one. Her card statement date and pay-later due dates didn’t match, so she got two reminders in the same week for different amounts. The card became one more thing to check before payday. (N-02, N-07, T-103, T-104)
- **Current workaround , the external tool or manual process they rely on (M2):** Before payday, she opens each pay-later app (Klarna, PayPal, Riverty) one by one. In the Riverty app she flips between the card screen and the pay-later screen and adds up the totals in her head. She matches reminders by hand, and asks support when the numbers don’t add up. (N-02, N-07, T-103, T-104)
- **Problem Hook , your one-sentence framing of the business crisis (M1):** We must stop Riverty from being just one more swappable option at checkout, by fixing consumers’ stress of tracking scattered pay-later bills and not being able to pay later in store.
- **Value Proposition , the outcome your initiative promised to deliver (M1):** Pay later anywhere, your way. Give each purchase its own due date, or bundle it into one monthly bill. You always see what you owe.

## Read the evidence in your case
- **Where does your case say people stall or leave? Does that match the friction you wrote in Module 2?:** Invited → applied: the biggest drop. Only 716 of 1,200 invited people applied (59.7%), so about 4 in 10 never even started. 
Approved → card activated: the second biggest. 586 people were approved, but only 431 activated (73.5%). 
First purchase → 3+ purchases. 350 people made a first purchase, but only 253 made three or more in their first month (72.3%). 

Does it match my Module 2 friction?

Only partly.
- **What got better or worse in the case, and does that support the workaround your persona uses?:** Better: Total spending grew from about €15k to €61k a month, and spend per active card rose from €200 to €233. Partner shops’ share also went up, from 57% to 63%.

Worse: Declines rose in month 4, with in-store declines back up to 8.7%. People also fade after their first month: in every group, activity drops 15 to 20 points, and in-store use stayed flat at around 17% of purchases. The month 4 dip in active cards is mostly fewer new sign-ups, not people leaving.

Does it support Lena’s workaround? Partly. People drop off right when the first bills and reminders arrive, which is when Lena starts juggling screens. But the data shows when people leave, not why.
- **Which user in the case is carrying the pain, and is that the person your Module 2 persona describes?:** Who carries the pain: heavy pay-later users. They buy the most (5.8 times a month), spend the most (€321) and use instalments the most (25%). That means the most due dates to track.

Is that Lena? Yes. She’s a heavy user, and her age group (25–34) spends the most.

Nuances:

It’s a keeping problem, not a starting one. Heavy users activate the most (83%), so the pain doesn’t stop them signing up. It risks them drifting away later.
The in-store pain belongs to someone else. Heavy users shop in store the least (12%), so that half of the hook fits light users better.

## Step 2 · Craft your hypothesis
- **Qualitative evidence (from M2) , quote the specific friction / moment of misery for your persona:** “I could not see in one place what I owe on the card and what I owe on my normal pay later orders.” (N-07)

It’s backed by two tickets. Participants ask which total is the real one (T-103), and two reminders arrive in the same week for different amounts (T-104).
- **Quantitative evidence (from M3) , name the metric or data point that confirms the pain; cite the number:** Activity drops right when the first bills and reminders arrive. In the month 1 group, 77.6% were active in their first month, 66.3% a month later, and 51.0% the month after that (cohort_activity.csv).

Heavy users like Lena carry the most due dates to track: 25.4% of their purchases are instalments, compared with 6.0% for light users (segments.csv).
- **Persona , role, goal, and the friction you confirmed in the reconciliation steps:** Role: Lena, 32, a heavy pay-later user who shops mostly on her phone, has two or three pay-later apps, and lives on a middling salary with little cushion.
Goal: She wants to always know exactly what she owes and when it’s due, all in one place, so payday never brings surprises.
Confirmed friction: She can’t see her card balance and her pay-later orders in one place, and gets mismatched reminders (N-07, T-103, T-104). Heavy users like her carry the most due dates to track (25.4% of purchases are instalments), and activity drops after the first month, right when the first bills arrive (77.6% → 66.3% → 51.0%). The reconciliation also showed that this is a problem of keeping users, not winning them. Heavy users activate well (82.6%), and the in-store pain fits light users more than Lena.
- **Problem you are solving , one sentence describing the specific friction this initiative removes:** Problem you are solving

Heavy pay-later users like Lena can’t see what they owe on the card and their pay-later orders in one place, and get mismatched reminders, so they drift away once the first bills arrive
- **Strategic outcome , what behaviour change do you expect, and how does it map to retention / revenue / churn?:** Strategic outcome

The behaviour change: heavy users like Lena keep using the card after their first bills arrive, and they move more of their pay-later spending onto Riverty instead of spreading it across apps.

Retention: more users still active two months in. The baseline is 51.0% for the month 1 group, and the goal is to lift that.
Revenue: heavy users spend the most (€321 a month), and 68.1% of their volume goes to partner shops. Keeping them means more card volume and more value for merchants.
Churn: fewer people fade out at the first-bill moment, and fewer “which total is real?” support contacts.
- **Primary success metric (initiative signal) , the leading indicator that tells you the gap is closing:** Primary success metric

The share of heavy users who are still making purchases in the month after their first bill. That’s the moment Lena currently drifts away.

Baseline: about 64–69% are still active one month after activation, across the three groups (cohort_activity.csv). The data pack doesn’t split this by heavy users, so you’d need to set that baseline yourself.
Why it’s leading: it moves before revenue and long-term churn do, so it tells you early whether the one-screen view is working.
- **Guardrail metric (product signal) , the metric that must NOT drop; it protects your existing base:** Guardrail metric

Partner merchant share of card volume must not drop. The baseline is 63.1% in month 4 (metric_baselines.csv).

Why this one: Riverty’s existing base is its merchants. If the one-screen view and monthly bill pull Lena’s spending away from partner shops toward big marketplaces, the card starts competing with the checkout business, which is exactly the fear in N-08 and N-09.
- **Decision window , how much time or data before you scale, pivot, or kill? minimum threshold to proceed?:** About 12 weeks, so that at least two groups of new users go through two full billing cycles each. The primary metric only shows up after the first bill, so anything shorter is too early.

Minimum data

At least 300 activated heavy users across those groups. The pilot only had 138, which is too few to trust a few points of change. Also include real customers, not just colleagues, because of the test-group bias in N-10.

Thresholds (my assumptions, so set your own)

Scale: the month-after-first-bill activity rises by at least 5 points, and partner share stays at or above 63%.
Pivot: activity rises less than 5 points, or the guardrail slips slightly. Fix the design and test again.
Kill: activity is flat or worse, or partner share falls clearly below 63%.
- **Draft your full hypothesis sentence , one to three sentences; quote the metric, name the persona, name the outcome:** Hypothesis statement

Based on Lena’s frustration that she “could not see in one place what I owe” (N-07), and on activity dropping from 77.6% to 51.0% in the two months after users’ first bills, I believe that giving heavy pay-later users like Lena one screen with one total and one clear reminder will keep them using the card after their first bill arrives. I’ll measure this as a 5-point increase in the share of heavy users still buying the month after their first bill (baseline about 64–69%). I will protect partner merchant share of volume (at or above 63.1%) and make a go/no-go decision after 12 weeks and at least 300 activated heavy users.
