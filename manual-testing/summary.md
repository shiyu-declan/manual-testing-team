# Team Summary

## Guided Testing Coverage

### Login Testing

Required coverage:
- Valid credentials.
- Incorrect password.
- Missing password.
- Missing username.
- Recovery after an invalid attempt.

Results:
Add links to the relevant member records.

### Equivalence Partitioning

Required coverage:
- Age below the accepted range.
- Age within the accepted range.
- Age above the accepted range.

Results:
Add links to the relevant member records.

### Input-Format Observations

Required observations:
- Blank age.
- Non-numeric age input.

Results:
Add links to the relevant member records.

### 2-Point Boundary Testing

Required values:
17, 18, 80, 81.

Results:
Add links to the relevant member records.

### 3-Point Boundary Testing

Required values:
16, 17, 18, 19, 79, 80, 81, 82.

Results:
Add links to new executions and identify reused evidence.

## Member Contributions

### Member A

- Guided results: [View results](results/member-a.md)
- Self-designed tests: [View tests](exploratory/member-a.md)
- Reflection: [View reflection](reflections/member-a.md)
- Chosen investigation:
- Main observation:
- Pull request: Add the actual pull-request link.

### Member B

- Guided results: [View results](results/member-b.md)
- Self-designed tests: [View tests](exploratory/member-b.md)
- Reflection: [View reflection](reflections/member-b.md)
- Chosen investigation:
- Main observation:
- Pull request: Add the actual pull-request link.

### Wei Ye

- Guided results: [View results](results/member-c.md)
- Self-designed tests: [View tests](exploratory/member-c.md)
- Reflection: [View reflection](reflections/member-c.md)
- Chosen investigation: Lastname input below 11 characters
- Main observation: Query rejected
- Pull request: Already merged

### Member D

- Guided results: [View results](results/member-a.md)
- Self-designed tests: [View tests](exploratory/member-a.md)
- Reflection: [View reflection](reflections/member-a.md)
- Chosen investigation:
- Main observation:
- Pull request: Add the actual pull-request link.

### Member E

- Guided results: [View results](results/member-e.md)
- Self-designed tests: [View tests](exploratory/member-e.md)
- Reflection: [View reflection](reflections/member-e.md)
- Chosen investigation: Error handing in Shopping cart.
- Main observation: The shopping cart handles a few errors. Have not taken account on certain scenarios like handling an empty cart. Though, it handles common errors such as input validations in the quantity section.
- Pull request: Already merged.