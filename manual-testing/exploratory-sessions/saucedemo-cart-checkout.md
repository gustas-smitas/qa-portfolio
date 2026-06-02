# Saucedemo — Cart & Checkout Exploration

**Date:** 2026-06-02
**Tester:** Gustas
**Browser / OS:** Chrome 148.0.7778.181 / macOS Tahoe 26.5

**URL:** https://www.saucedemo.com
**User:** standard_user / secret_sauce

---

## Goal

Explore the cart and checkout flow. Note anything that feels off — visual glitches, confusing UX, missing validations, unexpected behaviour. No formal bug format yet, just honest observations.

---

## Areas Explored

- [ ] Adding items to cart from inventory page
- [ ] Removing items from inventory page
- [ ] Cart badge (does count update correctly?)
- [ ] Cart page — item details, remove button, continue shopping
- [ ] Checkout step 1 — first name, last name, postal code fields
- [ ] Checkout step 2 — order summary, item total, tax, total
- [ ] Checkout complete page
- [ ] Back navigation during checkout (browser back button, "Cancel" buttons)

---

## Observations

### 1. Cart mouseover icon does not change to 'click here' icon

What happened: When hovering over cart icon, mouse cursor icon stayed the default one

What you expected: When hovering over cart icon, mouse hover icon changes to 'click here' icon

---

### 2. Can't change the amount to buy at checkout or in products page

What happened: Can't change the number of items to buy at checkout or in products page

What you expected: Expected to chose how many items I could buy at checkout or in products page

---

### 3. [Swag Labs page page heading does not link anywhere]

What happened: page heading is inactive text only

What you expected: for page heading to link to homepage

---

### 4. [clicking 'enter' after filling checkout credentials redirects to cart]

What happened: clicking enter after filling checkout credentials redirects back to cart page

What you expected: clicking enter after filling checkout credentials redirects to checkout conformation page

---

### 5. [postal code field at checkout works with letters only]

What happened: can press continue with invalid post code

What you expected: invalid post code is denied

---

## Questions / Things to Investigate Later

- input lengths
- error handling

## Time Spent

Start: ~17:00
End: ~17:30
Total:
