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
| Status | Run |

#### Purpose

To test whether the user can re-enter their credentials after a failed attempt.

#### Preconditions

User has an account registered in the website.

#### Test Data

| Field | Value |
|---|---|
| Input name | standard_user |

#### Steps

1.Enter standard_user and wrong_password.
2.Select Login.
3.Confirm rejection.
4.Replace the password with secret_sauce.
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
| Status | Run |

#### Purpose

Observe whether the input can be entered or is rejected, prevented or cleared.

#### Preconditions

None.

#### Test Data

| Field | Value |
|---|---|
| Input name | standard_user |

#### Steps

1.Enter Alex in First Name.
2.Enter TestingStudent in Surname.
3.Enter abc in age.
4.Select Singapore from dropdown.
5.Enter Manual testing classroom exercise in notes.
2.Select Submit.

#### Expected Result

The invalid attempted is rejected.

#### Actual Result

Input is prevented when entering the age.

#### Evidence

[View screenshot](../evidence/member-e/age-ep-abc-e.png)

---

## 2-Point Boundary Tests

## 3-Point Boundary Tests

