# JavaScript Testing Fundamentals

## Why is testing important?
1. Confidence (уверенность) of your code
2. Documentation for developers
3. Refactoring gets easy
4. Become a better developer
5. Working in a team

## What to test?
We're going to learn how to evaluate our code and identify what we should test. We walk through a User class and evaluate each method.

## Types of Testing
In this lesson about testing, we're learning about the different types of tests we can create.

```
    /1\      -  SLOW
  /  2  \
/____3____\  -  FAST
```

1. Acceptance Tests (often called end-to-end tests)
2. Integration Tests
3. Unit Tests - тестирование маленьких кусочков кода

Lets make first Unit test for class `User`.

## What are mocks and mocking?
Mocks are a common tool when writing tests for your software. In this lesson, we're learning what mocks are and why and when they are useful.

If we talk of a Mock, we mean an alternate implementation of a Dependency, when we are testing our code.

Here is mock example `mocks.js`.

## What are stubs?
We're learning what stubs are when it comes to JavaScript testing.

Stubs are similar to mocks, but they only replace small parts of your code compared to Mocks who replace the entire dependency.

To make our example easier we'll just evoke function itself, so, we can see the outcome
on the command line, as we did before.
```
(function have5Pokemons() {
    stubAmout(5)
    howsMyCollection()
})()
```
So, we changed the results to what we needed when we needed.

The originalAmount method is also available, if we would need it at any point. In this particular case we also save time, by creating a stub, instead of mocking the entire class.

For example we didn't change anything to say method. And now we can leverage it, and see that our test works as intended.

Here is stub example `stubs.js`.

How to debug JS:
- https://code.visualstudio.com/docs/nodejs/nodejs-debugging
- https://medium.com/the-node-js-collection/debugging-node-js-with-google-chrome-4965b5f910f4

## What are spies?
Spies are very handy and often has a lighter footprint than mocks.
