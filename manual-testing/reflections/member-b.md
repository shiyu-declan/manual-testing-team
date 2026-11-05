## 1. What makes a test positive or negative?

A test is positive or negative depending on whether the input is valid. Positive tests use valid input and expect the app to accept it, while negative tests use invalid input and expect the app to reject it.

## 2. Why can a negative test pass?

A negative test passes when the app handles the invalid input correctly. In LOGIN-N01, the wrong password produced the error "Epic sadface: Username and password do not match any user in this service" and no login, which was the expected result, so it passed.

## 3. How did equivalence partitioning help you select data?

It let me test one representative value from each age group instead of many similar ones. I used age 10 to represent everything below 18, which was enough to show that the below-range group is rejected, without testing every age under 18.

## 4. What did boundary testing help you investigate?

It helped me check the edge of the valid range, where mistakes like using > instead of >= are most likely. I tested 18 (the lowest valid age) and 19 (one above it), and both were accepted as expected.

## 5. What did you choose to test during the open-ended activity, and why?

I tested first-name length. The handout baseline name `Alex` was rejected with "Firstname too short" even though the instructions page lists no minimum, so I wanted to find where the cutoff is.

## 6. Did your observations lead to follow-up tests?

Yes. The rejected baseline led me to test first names of 1 to 6 characters. Lengths 1 to 4 were rejected and 5 and 6 were accepted, which suggests a minimum of 5 that isn't documented. That raised new questions, such as whether spaces or symbols count toward the length.

## 7. How does your Git history show your contribution?

My work is on my own branch, testing/member-b, with separate commits for each stage: login testing, the age tests, the self-designed test plan, and the self-designed results. The history shows the plan being committed before the results, and my files hold my own test records.