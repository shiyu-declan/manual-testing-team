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
### Requirement Question: First Name Minimum Length

- The handout baseline first name `Alex` (4 characters) was rejected with the message "Firstname too short".
- The instructions page does not list a minimum length for first name.
- `Alexander` (9 characters) was accepted with the other baseline values (TestingStudent, 30, Singapore, Manual testing classroom exercise).
- The exact minimum is unknown, so this is recorded as an observation only, not a confirmed defect.
- The team baseline now uses `Alexander` as the first name.

---

### Test ID: AGE-EP-10-B

| Item | Details |
|---|---|
| Test type | Negative |
| Tester | member-b |
| Website | Test Pages validation form |
| Technique | Equivalence partitioning |
| Status | Pass |

#### Purpose

Check that an age below the accepted range (below 18) is rejected.

#### Preconditions

The validation form is open and freshly loaded. All other fields use the agreed valid baseline.

#### Test Data

| Field | Value |
|---|---|
| First name | `Alexander` |
| Surname | `TestingStudent` |
| Age | `10` |
| Country | `Singapore` |
| Notes | `Manual testing classroom exercise` |

#### Steps

1. Open https://testpages.eviltester.com/apps/client-server-form-validation/ and reload so the form is empty.
2. Enter the baseline: first name `Alexander`, surname `TestingStudent`, country `Singapore`, notes `Manual testing classroom exercise`.
3. Enter `10` in the age field.
4. Select submit.
5. Observe the response.

#### Expected Result

Age 10 is rejected because it is below the minimum age of 18.

#### Actual Result

With the baseline values and only age changed to `10`, a validation message appeared on the age field: "Value must be greater than or equals to 18." The form could not be submitted and no Validation Report page was shown. The rejection came from the browser's input validation before submission, not from a server response. This matches the expected result.

#### Evidence

No screenshot captured. Result recorded in writing above.

---

   ## 2-Point Boundary Tests
### Test ID: AGE-2P-18-B

| Item | Details |
|---|---|
| Test type | Positive |
| Tester | member-b |
| Website | Test Pages validation form |
| Technique | 2-point boundary testing |
| Status | Pass |

#### Purpose

Check that the minimum valid age (18) is accepted.

#### Preconditions

The validation form is open and freshly loaded. All other fields use the agreed valid baseline.

#### Test Data

| Field | Value |
|---|---|
| First name | `Alexander` |
| Surname | `TestingStudent` |
| Age | `18` |
| Country | `Singapore` |
| Notes | `Manual testing classroom exercise` |

#### Steps

1. Open https://testpages.eviltester.com/apps/client-server-form-validation/ and reload so the form is empty.
2. Enter the baseline: first name `Alexander`, surname `TestingStudent`, country `Singapore`, notes `Manual testing classroom exercise`.
3. Enter `18` in the age field.
4. Select submit.
5. Observe the response and check the age shown in the report.

#### Expected Result

Age 18 is accepted, the Validation Report shows "Your Input passed validation", and the submitted age is shown as 18.

#### Evidence

No screenshot captured. Result recorded in writing above.

---

   ## 3-Point Boundary Tests
   ### Test ID: AGE-3P-19-B

| Item | Details |
|---|---|
| Test type | Positive |
| Tester | member-b |
| Website | Test Pages validation form |
| Technique | 3-point boundary testing (8-value convention: 16, 17, 18, 19, 79, 80, 81, 82) |
| Status | Pass |

#### Purpose

Check that an age one above the minimum boundary (19) is accepted.

#### Preconditions

The validation form is open and freshly loaded. All other fields use the agreed valid baseline.

#### Test Data

| Field | Value |
|---|---|
| First name | `Alexander` |
| Surname | `TestingStudent` |
| Age | `19` |
| Country | `Singapore` |
| Notes | `Manual testing classroom exercise` |

#### Steps

1. Open https://testpages.eviltester.com/apps/client-server-form-validation/ and reload so the form is empty.
2. Enter the baseline: first name `Alexander`, surname `TestingStudent`, country `Singapore`, notes `Manual testing classroom exercise`.
3. Enter `19` in the age field.
4. Select submit.
5. Observe the response and check the age shown in the report.

#### Expected Result

Age 19 is accepted, the Validation Report shows "Your Input passed validation", and the submitted age is shown as 19.

#### Actual Result

With the baseline values and only age changed to `19`, the form submitted and a Validation Report page appeared showing "Valid Input: Your Input passed validation". The "You submitted" section listed Age as 19, with the other fields matching the baseline. No validation errors appeared. This matches the expected result.

#### Evidence

No screenshot captured. Result recorded in writing above.

---