# Amazon Household Cart — Interactive Prototype

A clickable mobile prototype for **Household Cart**, a Prime-exclusive shared cart feature for Amazon that lets household members collaboratively build and review a cart before checkout.

Built as part of a Senior Growth PM take-home exercise for Samsara.

**Live prototype → [household-cart-prototype.vercel.app/prototype.html](https://household-cart-prototype.vercel.app/prototype.html)**

---

## The concept

Most Prime memberships are shared by households. But Amazon's cart experience is built for one person — leaving household coordination to happen outside the app, over text, or in person.

**Household Cart** closes that gap. One member initiates a shared cart, the other gets a push notification, both can add items, and they check out together — in one order, one delivery.

### Jobs to be done

> *When* I'm ready to place an Amazon order, *I want to* loop in my partner before I checkout, *so we can* make the purchase decision together, get everything we need in one order, and avoid the waste of multiple deliveries for things we could have combined.

Three motivations in one feature:
- **Purchase confidence** — joint decision-making enables commitment (the Costco effect)
- **Coordination efficiency** — fewer fragmented orders, fewer missed items
- **Environmental impact** — fewer deliveries, less waste

---

## Two entry-point flows

### Path A — Cart → Invite
The user has already been shopping and realizes before checkout they should loop in their partner. A contextual banner surfaces in the cart.

`My Cart` → `"Loop in Jeff" banner` → `Invite sheet` → `Shared cart live` → `Checkout`

### Path B — Product Page → Start Shared Cart
The earlier, higher-intent signal. The coordination thought forms at the product level — before the solo cart is even built.

`Product page` → `"Start Shared Cart" CTA` → `Invite sheet` → `Confirmation + push notification` → `Shared cart`

---

## Prototype details

Built on real Amazon mobile app screenshots with new UI elements composited on top.

**Key UX moments demonstrated:**
- Live collaborator pulse dot showing the invited member is active
- Visually distinct item ownership (Jeff's items clearly labeled and bordered)
- Duplicate item conflict detection before checkout
- Deal timer visible to both users
- Push notification preview the invited member receives

**Scoped to Prime Household members only** — this is a deliberate strategic choice. Making collaborative checkout Prime-exclusive protects Amazon's individual membership moat and turns the feature into a reason to *maintain* Prime rather than consolidate to one account.

---

## Files

| File | Description |
|---|---|
| `prototype.html` | Self-contained interactive prototype (all images embedded as base64) |
| `index.html` | Redirect to prototype.html for clean root URL routing |

---

## Running locally

No build step or dependencies needed. Just open `prototype.html` in any browser.

For the best experience, view in mobile form factor:
- **On your phone** — open the Vercel URL in Safari or Chrome
- **On a laptop** — open Chrome DevTools → toggle device toolbar → select iPhone 14

---

*Prototype by Gayle Doud · June 2026*
