   # Manual Testing Results — Member B

   ## Environment

   | Item | Details |
   |---|---|
   | Tester identifier | member-b |
   | Date and time | 2026-11-05, (time) |
   | Browser and version | (e.g. Chrome 1xx, from Help > About) |
   | Operating system | (e.g. Windows 11) |

   ## Login Tests
   ### Test ID: LOGIN-N01

| Item | Details |
|---|---|
| Test type | Negative |
| Tester | member-b |
| Website | SauceDemo |
| Status | Not run |

#### Purpose

Check that login is rejected when a valid username is entered with an incorrect password.

#### Preconditions

The SauceDemo login page is open, the user is logged out, and both input fields are empty.

#### Test Data

| Field | Value |
|---|---|
| Username | `standard_user` |
| Password | `wrong_password` |

#### Steps

1. Open https://www.saucedemo.com/ and confirm both fields are empty.
2. Enter `standard_user` in the username field.
3. Enter `wrong_password` in the password field.
4. Select `Login`.
5. Observe the page and any feedback shown.

#### Expected Result

Login is rejected, error feedback appears, and the inventory page is not reached.

#### Actual Result

After entering `standard_user` and `wrong_password` and selecting `Login`, login was rejected. The error message "Epic sadface: Username and password do not match any user in this service" appeared. The page stayed on the login screen and the inventory page was not reached. This matches the expected result.

#### Evidence

No screenshot captured. Result recorded in writing above.

---

   ## Equivalence Partitioning
### Test ID: AGE-EP-10-B

| Item | Details |
|---|---|
| Test type | Positive / Negative / Recovery |
| Tester | Your member identifier |
| Website | Website name |
| Status | Not run |

#### Purpose

What does this test check?

#### Preconditions

What must be true before the test starts?

#### Test Data

| Field | Value |
|---|---|
| Input name | Input value |

#### Steps

1.
2.
3.

#### Expected Result

Write this before executing the test.

#### Actual Result

Not recorded — test has not been executed.

#### Evidence

Not captured.

---
   ## 2-Point Boundary Tests
### Test ID: AGE-2P-18-B

| Item | Details |
|---|---|
| Test type | Positive / Negative / Recovery |
| Tester | Your member identifier |
| Website | Website name |
| Status | Not run |

#### Purpose

What does this test check?

#### Preconditions

What must be true before the test starts?

#### Test Data

| Field | Value |
|---|---|
| Input name | Input value |

#### Steps

1.
2.
3.

#### Expected Result

Write this before executing the test.

#### Actual Result

Not recorded — test has not been executed.

#### Evidence

Not captured.

---
   ## 3-Point Boundary Tests
   ### Test ID: AGE-3P-19-B

| Item | Details |
|---|---|
| Test type | Positive / Negative / Recovery |
| Tester | Your member identifier |
| Website | Website name |
| Status | Not run |

#### Purpose

What does this test check?

#### Preconditions

What must be true before the test starts?

#### Test Data

| Field | Value |
|---|---|
| Input name | Input value |

#### Steps

1.
2.
3.

#### Expected Result

Write this before executing the test.

#### Actual Result

Not recorded — test has not been executed.

#### Evidence

Not captured.

---