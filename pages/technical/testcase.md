A test case is composed of 2 tests:

- a test in the IDE for players to test their code against a specific scenario
- a test, called _validator_ to validate the same kind of scenario

IDE tests are visible to the players whereas validators are hidden.

## Guidelines for writing test cases <a name="guidelines"/>

- Test cases should cover all specifications

_The more tests, the better._

- Each validator must* differ from the corresponding test

_It's only to ensure that the players don't hardcode the solution._
_* Sometimes, to cover edge cases, there is no other way than having the same test as validator_

- Each validator should check the same case as the corresponding test

_They work by pairs._

- The first test case must be a simple one

_It's included in the statement as the example._

## Best Practices

- It is useful to give explicit names to test cases to help players quickly understand their purpose

