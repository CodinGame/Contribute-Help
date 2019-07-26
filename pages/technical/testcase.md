A test case is composed of 2 tests:

- a test for the IDE
- a test for validating a solution, often called _validator_.

IDE tests are visible to the players whereas validators are hidden.

# Guidelines <a name="guidelines"/>

- Test cases should cover all specifications

_The more tests, the better._

- Test cases must have explicit names

_It helps players to understand the purpose of the test._

- Each validator should check the same case as the corresponding test

_They work by pairs._

- Each validator must differ from the corresponding test

_It's only to ensure that the players don't harcode the solution._

- The first test case must be a simple one

_It's included in the statement._

