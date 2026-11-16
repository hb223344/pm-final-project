# PRD & Prototype Sprint (Module 4)

## Pick & scope with MoSCoW
- **The “Now” feature I’m scoping (name + one-line core description):** B3: One balance view. It shows everything Lena owes on the card and her pay-later orders as one total, on one screen.
- **My finalized Must-Haves (after overriding the AI):** One total owed, combining the card balance and all Riverty pay-later orders
A list of every unpaid item with shop, amount, due date and a “Card” or “Pay later” label
The next due date and amount shown at the top
The total and next due date update right away when an item is paid
- **What I demoted from Must → Should/Won’t, and why:** Pay from the list → Should. Lena can see what she owes without it, and paying is a separate flow.
“Last updated” time → Should. Good for trust, but the total works without it.
Klarna and PayPal orders → Won’t. We have no access to their data, and it would need partner deals.
Unified reminders → Won’t. That’s B8, and it needs terms approval that takes months (N-11).

## Generate your Simplified PRD
- **One thing my PRD makes explicit that a vague brief would have missed:** The total has to match the item list to the cent, and if it doesn’t, the app shows an error instead of a wrong number. “Show the balance” would never have said that, but a wrong total is exactly Lena’s moment of misery.

## Prompt-to-prototype sprint
- **Where did the prototype reveal a gap in my PRD logic? (what I had to update):** The PRD never said how card purchases get paid. In the prototype, you could pay each card purchase one by one, but a real card is paid as one statement. I had to add a rule: card items are paid together as one statement, and pay-later orders are paid one by one.
- **My prototype: save Claude's HTML as prototype.html in 04-roadmap/, open it in your browser, and add a screenshot:** _(not filled in)_
