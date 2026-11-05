# Self-Designed Testing — Member E

## Testing Idea

Find out how the shopping cart handles invalid values or inputs.

## Reason

When I logged into the website, I saw the inventory and shopping cart. I want to test whether there is any errors I can produce.

## Test Basis

See if it updates the quantity of different items and how it handles an empty shopping cart.

## Approach

I will log in with the same username (`standard_user`) and password (`secret_sauce`) as a baseline. While only changing the items and their quantity in the shopping cart.

## Test Cases

### Test ID: OWN-E-01

| Item | Details |
|---|---|
| Test type | Negative |
| Tester | member-e |
| Status | Pass |

#### Purpose

Check how it handles non-numeric input in quantity.

#### Preconditions

User is already logged in.

#### Test Data

| Field | Value |
|---|---|
| Cart | Sauce Labs Backpack |
| Qty | abc |

#### Steps

1. Add `Sauce Labs Backpack` to cart.
2. Click cart icon.
3. Input `abc` in Qty.

#### Expected Result

Qty field would prevent any non-numeric input.

#### Actual Result

Qty field is empty after inputting the non-numeric value.

#### Evidence

[View screenshot](../evidence/member-e/own-e-01.png)

---

## Test Cases

### Test ID: OWN-E-02

| Item | Details |
|---|---|
| Test type | Negative |
| Tester | member-e |
| Status | Fail |

#### Purpose

Check how it handles an empty cart.

#### Preconditions

User is already logged in.

#### Test Data

| Field | Value |
|---|---|
| First Name | Alex |
| Last Name | TestingStudent |
| Postal Code | 654321 |
| Cart | NULL |

#### Steps

1. Click Cart icon.
2. Click Checkout.
3. Enter First Name, Last Name, Postal Code.
4. Click Continue.
5. Click Finish.

#### Expected Result

Error message to appear when clicking checkout.

#### Actual Result

Able to complete the checkout with an empty cart.

#### Evidence

[View screenshot](../evidence/member-e/own-e-02.png)

---

## Overall Observations

The shopping cart handles a few errors. Have not taken account on certain scenarios like handling an empty cart. Though, it handles common errors such as input validations in the quantity section.

## Next Question

How does it handle errors for their inventory page?