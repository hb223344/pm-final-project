# AI Synthesis, Product Health & Insights Summary (Module 2)

## Responses
- **Assumption to validate #1:** In-store use. Customers will actually use the card in shops, not just online. Her habit of tapping her bank card can change.
- **Assumption to validate #2:** One view. Seeing evaerything she owes in one place is a strong enough reason to add yet another card.
- **Assumption to validate #3:** Sign-up is easy enough. Most people who apply will get through the ID check without giving up.
- **Moment of misery / red flag #1 (e.g., “user gave up after 3 tries”):** The card got declined at a bakery and the app didn’t say why. The participant went back to their debit card the same week (N-06).
- **Moment of misery / red flag #2:** “Which total is the real one?”
Participants couldn’t see in one place what they owe on the card and on their normal pay-later orders (N-07, T-103).
- **Moment of misery / red flag #3:** paid twice because the alert was late
In some shops the purchase notification arrives minutes late. People think the payment failed and pay again with another card (T-108). Paying twice for one coffee is the kind of thing people don’t forget, and it kills trust fast.
- **Product Health & Insights Summary (Claude's output):** Executive summary

The test shows a clear need for the card: heavy pay-later users want the same control in store that they already get online. That makes the card relevant beyond Riverty’s checkout. In practice, the experience breaks at the moments that decide whether people come back: in-store declines with no reason given, late payment confirmations, and a split view of what users owe. Each of these pushes users back to their debit cards. The core product idea holds up, but trust in the card is weaker than the need for it, and the test group’s makeup means the real-world gap is likely larger than observed.

Thematic synthesis
1. Technical stability

Stability issues cluster at the point of sale rather than across the product. In-store purchases are the newest and least familiar way people use Riverty, and a failure there carries outsized cost. A single unexplained decline or an unclear payment status leads users to switch payment methods, and these issues hit hardest at exactly that point.

Critical: In-store declines show no reason or next step in the app. 48 declines appear in the test log, and at least one participant went back to their debit card within a week (T-101, N-06).
High: Purchase notifications arrive minutes late at some shops. Users read the payment as failed and pay again with another card, creating duplicate charges (T-108).
High: Phone wallet setup fails or is abandoned after activation, with 143 activated cards never reaching the wallet. That leaves a large share of users unable to tap to pay in store (T-102).
2. Onboarding and adoption

Losses happen both before and after approval. During application, a repeat-upload loop at the ID check causes some people to give up. After activation, the bigger barrier is habit: in-store payment with a bank card is automatic, and a new card has to be remembered to be used. Users with several pay-later apps already treat another card as extra mental load rather than relief.

High: The identity check asks for a new document photo after a failed upload, and some applicants quit at this step (T-106).
High: Users default to their bank card in store and would have to actively remember the Riverty card (N-03).
High: For users who already hold several pay-later products, the card adds one more balance to check before payday rather than replacing anything (N-02).
3. Trust and clarity

This is the largest theme. The card’s main promise is control over what you owe, yet the test experience fragments that picture. Two balances on separate screens and two reminder schedules with different amounts weaken confidence in the numbers themselves. Uncertainty about credit scores and instalments adds to this, especially for users who are wary of credit.

High: The card balance and regular pay-later orders appear on different screens, and users ask which total is correct (T-103, N-07).
High: The card statement date and pay-later due dates don’t line up, so users get several reminders in the same week for different amounts (T-104).
Medium: Credit-wary users react negatively to instalment and interest framing, which limits how much of the market the card appeals to (N-05).
Medium: Users are unsure whether card use affects their credit score, and no help content addresses the question (T-107).
4. Value proposition and retention

The underlying need is real and specific: users want to decide on a purchase before the money leaves their account, and they want that for everyday spending like grocery runs. Evidence on lasting use is weak, though. Incentives are seen as a reason to try the card, not to keep using it, so retention would have to come from the core experience rather than from rewards.

High: Retention isn’t yet proven. Cashback is described as a trial driver with no effect on continued use (N-12).
Medium: Demand for everyday in-store use, such as splitting the weekly supermarket shop, is strong but depends on reliable acceptance (N-04, N-01).
5. Merchant and strategic alignment

Merchant feedback shows a strategic risk to Riverty’s merchant-first model. Large online merchants see a card usable everywhere as a reason for customers to stop choosing Riverty at their checkout. Smaller merchants are open to the card only if it sends traffic to them rather than to large marketplaces. The value case for merchants is not yet clear.

High: Enterprise merchants question what they gain if the card works everywhere, a direct risk to the checkout relationship (N-08).
Medium: SME merchants are conditionally positive: interested if the card sends customers to them, opposed if it favours marketplaces (N-09).
6. Evidence quality and operating constraints

Two internal constraints affect how far these findings can be trusted and acted on. The test group is mostly employees, so approval and repayment results likely look better than they would with real customers. Separately, every change to the product’s pricing, credit policy or terms needs regulatory approval, which takes months. This limits how quickly the issues above can be addressed once scope is set.

High: Results are likely skewed by an employee-heavy test group, especially approval and repayment metrics (N-10).
High: Regulatory approval takes months for every product change, which limits how much can be adjusted between test and launch (N-11).
7. Support load

No ticket volume data is available, so this theme is inferred from the nature of the issues. Several problems above are likely to generate repeat contacts: questions about which balance is correct, duplicate-charge disputes from late notifications, decline queries with no in-app explanation, and credit score questions with no self-service answer. The support burden would likely grow with the user base rather than level off.

Medium (inferred): Repeat contacts are likely from balance confusion, duplicate charges, unexplained declines and credit score questions (T-103, T-108, T-101, T-107).

Minor Technical Debt: The post-purchase instalment option shows up only for some purchase categories, with no visible logic, so users read it as random (T-105).
- **Did the AI catch the specific moment of misery / pain point you found in Step 1?:** Yes, fully.
- **Did it smooth over a critical frustration into a generic bullet point?:** Partially
- **Did the AI try to suggest features or a roadmap despite the constraints?:** No.
- **Logic leak / hallucination #1 (e.g., “AI suggested a new search bar feature, roadmap leak”):** The AI turned single quotes into group findings. One enterprise merchant (N-08) became “large online merchants see the card as a reason...”, and one small shop owner (N-09) became “smaller merchants are open to it.”
- **Logic leak / hallucination #2:** _(not filled in)_
