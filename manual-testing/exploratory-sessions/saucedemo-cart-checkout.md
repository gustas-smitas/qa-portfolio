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

- [x] Adding items to cart from inventory page
- [x] Removing items from inventory page
- [x] Cart badge (does count update correctly?)
- [x] Cart page — item details, remove button, continue shopping
- [x] Checkout step 1 — first name, last name, postal code fields
- [x] Checkout step 2 — order summary, item total, tax, total
- [x] Checkout complete page
- [x] Back navigation during checkout (browser back button, "Cancel" buttons)

---

## Observations

### 1. Cart mouseover icon does not change to 'click here' icon

What happened: When hovering over cart icon, mouse cursor icon stayed the default one

What you expected: When hovering over cart icon, mouse hover icon changes to 'click here' icon

---

### 2. Can't change the amount to buy at checkout or in products page

What happened: Can't change the number of items to buy at checkout or in products page

What you expected: Expected to choose how many items I could buy at checkout or in products page

---

### 3. Swag Labs page heading does not link anywhere

What happened: page heading is inactive text only

What you expected: for page heading to link to homepage

---

### 4. clicking 'enter' after filling checkout credentials redirects to cart

What happened: clicking enter after filling checkout credentials redirects back to cart page

What you expected: clicking enter after filling checkout credentials redirects to checkout confirmation page

---

### 5. checkout form page accepts all symbols

What happened: name, last name and postal code input fields accept all symbols and any length

What you expected: checkout form page denies further checkout process with invalid form inputs (input length over 255, invalid characters used)

---

## Questions / Things to Investigate Later

- Check if checkout form gracefully handles empty input fields (shows an error message)
- Check if checkout is possible with empty shopping cart

## Time Spent

Start: ~17:00
End: ~17:30
Total: ~30 minutes
