# Self-Designed Testing — Member B

## Testing Idea

Find out how the first-name field handles short names, and where "Firstname too short" stops appearing.

## Reason

While setting up the baseline, `Alex` (4 characters) was rejected with "Firstname too short", but the instructions page lists no minimum length. I want to find out where the cutoff actually is.

## Test Basis

The instructions page says first name is required and fewer than 90 characters. It gives no minimum length, so there is no documented expected result for short names. Each case is an exploratory observation, and I will not label any result as a defect.

## Approach

Keep surname (`TestingStudent`), age (`30`), country (`Singapore`) and notes (`Manual testing classroom exercise`) at the baseline. Change only the first name, using lengths 1 to 6 in order. Reload the form before each case.

## Test Cases

### Test ID: OWN-B-01

| Item | Details |
|---|---|
| Test type | Exploratory |
| Tester | member-b |
| Status | Observation only |

#### Purpose

Check how a 1-character first name is handled.

#### Preconditions

Validation form open and freshly loaded.

#### Test Data

| Field | Value |
|---|---|
| First name | `A` (1 character) |
| Other fields | Baseline (TestingStudent, 30, Singapore, Manual testing classroom exercise) |

#### Steps

1. Reload the validation form.
2. Enter the baseline values with first name `A`.
3. Select submit.
4. Observe the response.

#### Expected Result

No documented minimum, so no confirmed expected result. Question being investigated: is a 1-character first name accepted or rejected?

#### Actual Result

The form was rejected with a "Firstname too short" error.

#### Evidence

No screenshot captured. Result recorded in writing above.

---

### Test ID: OWN-B-02

| Item | Details |
|---|---|
| Test type | Exploratory |
| Tester | member-b |
| Status | Observation only |

#### Purpose

Check how a 2-character first name is handled.

#### Preconditions

Validation form open and freshly loaded.

#### Test Data

| Field | Value |
|---|---|
| First name | `Al` (2 characters) |
| Other fields | Baseline |

#### Steps

1. Reload the validation form.
2. Enter the baseline values with first name `Al`.
3. Select submit.
4. Observe the response.

#### Expected Result

No documented minimum. Question being investigated: is a 2-character first name accepted or rejected?

#### Actual Result

The form was rejected with a "Firstname too short" error.

#### Evidence

No screenshot captured. Result recorded in writing above.

---

### Test ID: OWN-B-03

| Item | Details |
|---|---|
| Test type | Exploratory |
| Tester | member-b |
| Status | Observation only |

#### Purpose

Check how a 3-character first name is handled.

#### Preconditions

Validation form open and freshly loaded.

#### Test Data

| Field | Value |
|---|---|
| First name | `Ale` (3 characters) |
| Other fields | Baseline |

#### Steps

1. Reload the validation form.
2. Enter the baseline values with first name `Ale`.
3. Select submit.
4. Observe the response.

#### Expected Result

No documented minimum. Question being investigated: is a 3-character first name accepted or rejected?

#### Actual Result

The form was rejected with a "Firstname too short" error.

#### Evidence

No screenshot captured. Result recorded in writing above.

---

### Test ID: OWN-B-04

| Item | Details |
|---|---|
| Test type | Exploratory |
| Tester | member-b |
| Status | Observation only |

#### Purpose

Formally repeat the 4-character case that was rejected during baseline setup.

#### Preconditions

Validation form open and freshly loaded.

#### Test Data

| Field | Value |
|---|---|
| First name | `Alex` (4 characters) |
| Other fields | Baseline |

#### Steps

1. Reload the validation form.
2. Enter the baseline values with first name `Alex`.
3. Select submit.
4. Observe the response.

#### Expected Result

No documented minimum. Earlier baseline setup showed "Firstname too short"; this checks whether that is repeatable.

#### Actual Result

The form was rejected with a "Firstname too short" error again, so the baseline-setup result was repeatable.

#### Evidence

No screenshot captured. Result recorded in writing above.

---

### Test ID: OWN-B-05

| Item | Details |
|---|---|
| Test type | Exploratory |
| Tester | member-b |
| Status | Observation only |

#### Purpose

Check how a 5-character first name is handled.

#### Preconditions

Validation form open and freshly loaded.

#### Test Data

| Field | Value |
|---|---|
| First name | `Alexa` (5 characters) |
| Other fields | Baseline |

#### Steps

1. Reload the validation form.
2. Enter the baseline values with first name `Alexa`.
3. Select submit.
4. Observe the response.

#### Expected Result

No documented minimum. Question being investigated: is a 5-character first name accepted or rejected?

#### Actual Result

The form submitted and the Validation Report showed "Your Input passed validation". The first name was listed as Alexa, with the other fields matching the baseline.

#### Evidence

No screenshot captured. Result recorded in writing above.

---

### Test ID: OWN-B-06

| Item | Details |
|---|---|
| Test type | Exploratory |
| Tester | member-b |
| Status | Observation only |

#### Purpose

Check how a 6-character first name is handled.

#### Preconditions

Validation form open and freshly loaded.

#### Test Data

| Field | Value |
|---|---|
| First name | `Alexan` (6 characters) |
| Other fields | Baseline |

#### Steps

1. Reload the validation form.
2. Enter the baseline values with first name `Alexan`.
3. Select submit.
4. Observe the response.

#### Expected Result

No documented minimum. Question being investigated: is a 6-character first name accepted or rejected?

#### Actual Result

The form submitted and the Validation Report showed "Your Input passed validation". The first name was listed as Alexan, with the other fields matching the baseline.

#### Evidence

No screenshot captured. Result recorded in writing above.

---

## Overall Observations

First names of 1 to 4 characters were rejected with "Firstname too short". First names of 5 and 6 characters were accepted. This suggests the form enforces a minimum first-name length of 5 characters, but the instructions page does not document this, so it is recorded as an observation only. Only lengths 1 to 6 were tested, and each length was tried once, so this is not proof of the exact rule.

## Next Question

Is the minimum counted in characters regardless of type (for example, would a name made of spaces or symbols count)? Also, is there a maximum, and does it match the documented limit of fewer than 90 characters?