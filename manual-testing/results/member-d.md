# Manual Testing Results — Member D

## Environment

| Item | Details |
|---|---|
| Tester identifier | member-d |
| Date and time | |
| Browser and version | |
| Operating system | |

## Login Tests

## Equivalence Partitioning

## 2-Point Boundary Tests

## 3-Point Boundary Tests

### Test ID: LOGIN-N03

| Item | Details |
|---|---|
| Test type | Positive |
| Tester | D |
| Website | [Website name](https://www.saucedemo.com/) |
| Status | Pass |

#### Purpose

Checks if user can login successfully if they dont enter their username

#### Preconditions

User must have an existing account

#### Test Data

| Field | Value |
|---|---|
| Username | Empty |
| Password | secret_sauce |

#### Steps

1.Follow the shared starting procedure.
2.Leave the username empty.
3.Enter the password.
4.Select Login.
5.Observe the feedback.

#### Expected Result

The attempt is rejected with validation feedback. The inventory is not reached.

#### Actual Result

User cannot login to their account and receives an error message

#### Evidence

[View screenshot](../evidence/member-d/image.png)

---