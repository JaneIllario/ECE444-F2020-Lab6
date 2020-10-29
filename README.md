# ECE444-F2020-Lab6

## Pros and Cons of TDD

### Pros
1. TDD encourages adding feautures and related tests incrementally, an approach that makes identifying the source of error easier because the most recently added feature is likely the code or integrated functionality causing issues.

2. Individual unit testing for each function encourages higher granularity tests as the developer spends more time working with a single function, analyzing corner cases, and forecast user-interaction with the funcitonality. This, in contrast to writing a testing suite for the whole code once all is done gives the developer more intimate knowledge of all functional components and likely exposes them to thinking about more edge cases.

3. High test converage as there is individual testing for each feature/function in the form of unit tests. This goes to reduce efforts required in later phase debugging, once the system is larger and more complex, given that the isolated features of the code work as expected.

### Cons
1. In a complex system, features often become more interdependent and unit testing may necessitate rigorous mocking in order to execute thoroughly. Setting up mocking infrastructure is often a significant time investment on behalf of the developers, and religious following of the TDD doctorine will likely extend development time.

2. The effectiveness of TDD relies on the quality of the tests written. For unit tests, there is an assumption that the developer has asserted for the correct values and written the functions with a correct input and output schemes. For more sophisticates tests, such as integration/regression tests, the developer has to properly understand the many interactions taking place in the system and their expected funcitoning. Incorrect tests, incomplete tests, and redundant tests may falsely imply the correctness of the code while the test suite iteself is heavily flawed.

3. Test require upkeep based on code changes, and wiht the extensive testing produced through TDD, this would mean greater developer/tester time required for asserting that tests that fail are doing so for good reason as opposed to being outdated. While this is a good way to control how quickly big updates to the code take place, it is a factor to be consdiered under developer time expenditure.
