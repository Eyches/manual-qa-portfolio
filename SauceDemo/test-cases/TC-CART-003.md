# TC-CART-003: Remove an item from the shopping cart

## Test Information
- **Application:** SauceDemo
- **Module:** Shopping Cart
- **Test Type:** Functional Testing
- **Test Level:** System Testing
- **Execution Date:** 2026-10-13
- **Status:** PASSED

## Preconditions
- The user is logged in as `standard_user`.
- The Products page is open.
- The shopping cart is empty.

## Test Data
- Product 1: Sauce Labs Backpack
- Product 2: Sauce Labs Bike Light

## Test Steps
1. Add Sauce Labs Backpack to the cart.
2. Add Sauce Labs Bike Light to the cart.
3. Open the shopping cart.
4. Verify that both products are displayed.
5. Remove Sauce Labs Backpack from the cart.
6. Verify that Sauce Labs Bike Light remains in the cart.
7. Verify that the cart badge displays `1`.

## Expected Result
- Both products are successfully added to the shopping cart.
- The cart badge displays `2` after adding both products.
- Sauce Labs Backpack is removed from the cart.
- Sauce Labs Bike Light remains in the cart.
- The cart badge updates to `1`.

## Actual Result
Both Sauce Labs Backpack and Sauce Labs Bike Light were
successfully added to the shopping cart.

The cart badge displayed `2`.

After removing Sauce Labs Backpack, only Sauce Labs Bike Light
remained in the cart.

The cart badge displayed `1`.

## Status
**PASSED**

## Notes
This test case was designed and executed manually
on the public SauceDemo demonstration application.
