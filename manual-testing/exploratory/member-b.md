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
| Status | Not run |

#### Purpose

Check how a 1-character first name is handled.

#### Preconditions

Validation form open and freshly loaded.

#### Test Data

| Field | Value |
|---|---|
| First name | `A` (1 character) |
| Other fields | Baseline (TestingStudent, 30, Singapore, notes) |

#### Steps

1. Reload the validation form.
2. Enter the baseline values with first name `A`.
3. Select submit.
4. Observe the response.

#### Expected Result

No documented minimum, so there is no confirmed expected result. Question being investigated: is a 1-character first name accepted or rejected?

#### Actual Result

Not recorded — test has not been executed.

#### Evidence

Not captured.

---

### Test ID: OWN-B-02

| Item | Details |
|---|---|
| Test type | Exploratory |
| Tester | member-b |
| Status | Not run |

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

No documented minimum. Question being