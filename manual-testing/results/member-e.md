# Manual Testing Results — Member E

## Environment

| Item | Details |
|---|---|
| Tester identifier | Member-E |
| Date and time | 5/11/2026 1030 hrs |
| Browser and version | Google Chrome 157 |
| Operating system | Windows 11 |

## Login Tests

### Test ID: LOGIN-R01

| Item | Details |
|---|---|
| Test type | Recovery |
| Tester | Member-E |
| Website | https://www.saucedemo.com/ |
| Status | Pass |

#### Purpose

To test whether the user can re-enter their credentials after a failed attempt.

#### Preconditions

User has an account registered in the website.

#### Test Data

| Field | Value |
|---|---|
| Username | standard_user |
| Password | wrong_password |
| Corrected Password | secret_sauce |

#### Steps

1.Enter `standard_user` and `wrong_password`.
2.Select Login.
3.Confirm rejection.
4.Replace the password with `secret_sauce`.
5.Keep the username unchanged.
6.Select Login again.
7.Check whether the inventory appears.

#### Expected Result

The invalid attempt is rejected. After correcting the password, login succeeds.

#### Actual Result

For the first attempt, entering with a wrong password prompted a rejected message. 
On the second attempt, able to login after correcting the password and able to view all the inventory.

#### Evidence

[View screenshot](../evidence/member-e/login-r01-1st.png)
[View screenshot](../evidence/member-e/login-r01-2nd.png)

---
## Equivalence Partitioning
### Test ID: AGE-EP-ABC-E

| Item | Details |
|---|---|
| Test type | Negative |
| Tester | Member-E |
| Website | https://testpages.eviltester.com/apps/client-server-form-validation/ |
| Status | Pass |

#### Purpose

Observe whether the input can be entered or is rejected, prevented or cleared.

#### Preconditions

None.

#### Test Data

| Field | Value |
|---|---|
| First name | Alex |
| Surname | TestingStudent |
| Age | abc |
| Country | Singapore |
| Notes | Manual testing classroom exercise |

#### Steps

1. Restore the validation form.
2. Enter the baseline.
3. Enter `abc` in age field.
4. Submit.
5. Observe the response.

#### Expected Result

The invalid attempted is rejected.

#### Actual Result

Input is prevented when entering the age.

#### Evidence

[View screenshot](../evidence/member-e/age-ep-abc-e.png)

---

## 2-Point Boundary Tests

### Test ID: AGE-2P-18-81-E

| Item | Details |
|---|---|
| Test type | Negative |
| Tester | member-e |
| Website | Test Pages validation form |
| Technique | 2-point boundary testing |
| Status | Pass |

#### Purpose

Check whether the age that are either above or below the boundary values is rejected.

#### Preconditions

The validation form is open.
All other fields will use the agreed valid baseline.

#### Test Data

| Field | Value |
|---|---|
| First name | Alex |
| Surname | TestingStudent |
| Age | `18` & `81` |
| Country | Singapore |
| Notes | Manual testing classroom exercise |

#### Steps

1. Restore the validation form.
2. Enter the baseline.
3. Replace age with `18`.
4. Submit.
5. Observe the response.
6. Restore the validation form.
7. Enter the baseline.
8. Replace age with `81`.
9. Submit.
10. Observe the response again.

#### Expected Result

Age 81 is rejected because it is above the maximum age of 80 whereas Age 18 is accepted.

#### Actual Result

Age 18 is accepted whereas for Age 81, an invalid prompt appears. 

#### Evidence

[View screenshot](../evidence/member-e/age-2p-18-e.png)
[View screenshot](../evidence/member-e/age-2p-81-e.png)
---

## 3-Point Boundary Tests

### Test ID: AGE-3P-18-81-E

| Item | Details |
|---|---|
| Test type | Negative |
| Tester | member-e |
| Website | Test Pages validation form |
| Technique | 3-point boundary testing |
| Status | Not Run |

#### Purpose

Check whether the age that are either above or below the boundary values is rejected.

#### Preconditions

The validation form is open.
All other fields will use the agreed valid baseline.

#### Test Data

| Field | Value |
|---|---|
| First name | Alex |
| Surname | TestingStudent |
| Age | `16` & `79` |
| Country | Singapore |
| Notes | Manual testing classroom exercise |

#### Steps

1. Restore the validation form.
2. Enter the baseline.
3. Replace age with `16`.
4. Submit.
5. Observe the response.
6. Restore the validation form.
7. Enter the baseline.
8. Replace age with `79`.
9. Submit.
10. Observe the response again.

#### Expected Result

Age 16 is rejected because it is below the minimum age of 80 whereas Age 79 is accepted.

#### Actual Result

Age 79 is accepted whereas for Age 16, an invalid prompt appears. 

#### Evidence

[View screenshot](../evidence/member-e/age-3p-16-e.png)
[View screenshot](../evidence/member-e/age-3p-79-e.png)
---
