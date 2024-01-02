[home](../README.md)
# [Development Practices](README.md) - Testability


Having a suite of reliable tests can enable the team to make change with the confidence that they aren't breaking the existing functionality.

Whilst creating and maintaining an effective test suite can be seen as a distraction from developing change, investing time and effort at this stage can save significant time and effort later.


## When to write test?

>The best time to plant a tree was 20 years ago. The second best time is today.

The same is true for writing tests.

**The best time to write tests**, is right before the functionality is created. Adopting a test-first approach is a recomended method called Test Driven Development. The developer first writes a failing test (or tests) and then makes the required changes to enable the test to pass.

**The second best time to write tests**, is now.

In cases where an established application has little or no tests, to get to the industry standard of 80% test coverage can seem an insurmountable task. However, an achievable aim would be that - *all future changes must have at least 80% code coverage*.

See [quality gate enforcement](../continuous-delivery/quality-gate-enforcement.md).


## When to "fix" a failing test?

The team should have a mindset that - when a test fails, it is investigated straightaway. This ensures that it is "fixed" whilst the change is still fresh in the minds of those who wrote it.

Fixing a failing test can mean:
* Altering the functionality of the change so that the test passes - i.e. the test was correct
* Updating the test to accommodate the new functionality - i.e. the code was correct
* A combination of the above

It should **never** mean - disabling the test in order to meet a deadline.

However, in some circumstances - it could mean
* The test is no longer fit-for-purpose and should be deleted
> [!WARNING]  
> This should be a team decision to prevent accusations of poor practice - i.e. "deleting rather than fixing"

---
**Further reading**:
* [Testing Maturity](../test-automation/testing-maturity.md)
* [You Should Throw Your Unit Tests Away](https://medium.com/ngconf/you-should-throw-away-your-unit-tests-717c6884a77b)
