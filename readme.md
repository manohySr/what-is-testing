## 🚀 Testing

- Your project will scale 🚀, and you will add more code to it.
- As code grows, debugging becomes more challenging. Everything is somehow interconnected, and adding some code (even with good intentions to improve performance) may break the whole thing. 🐞🔧
- Enter **Testing**: Testing helps us to add code without the fear of breaking something. 🛡️

## 🔍 Types of Tests

### 🧩 Unit Tests

- How a piece of code is expected to work.
- Focus on one function at a time.
- Don’t worry about other functions.

### 🔗 Integration Tests

- How different pieces of code are expected to work together.
- Liaison between some functions.
- Cross communication validation.

### 🤖 Automation Tests

- UI tests.
- Test in real-life scenarios (human test or robot test).

## 🛠️ Testing Libraries

- **[Jest](https://jestjs.io/)**
- **[Cypress](https://www.cypress.io/)**
- **[Jasmine](https://jasmine.github.io/)**
- **[Mocha](https://mochajs.org/)**

## 🧪 What We Expect in Tests

### 🔍 Test Assertion

Test assertions are the conditions or boolean expressions used within a test case to verify that the code behaves as expected. Assertions compare the actual output of the code with the expected output. If the comparison fails, the test fails.

**Example:**

```javascript
const sum = (a, b) => a + b;
const result = sum(2, 3);
assert.equal(result, 5); // This is an assertion
```

### 🏃 Test Runner

A test runner is a tool that runs tests and reports the results. It organizes test execution, handles setup and teardown, and provides feedback on which tests passed or failed. Popular test runners include Jest, Mocha, and Jasmine.

**Example:**

```javascript
jest // Command to run tests using Jest
```

### 📊 Code Coverage

Code coverage measures how much of your code is executed while running tests. It helps identify which parts of your codebase are not tested and ensures that your tests cover all possible execution paths.

**Example:**

```javascript
jest --coverage // Command to run tests with code coverage reporting in Jest
```

### 🔍 Spy

A spy allows you to track the calls to a function and its arguments without replacing the function. It's useful for verifying that certain functions are called with the expected arguments.

**Example with Sinon:**

```javascript
const spy = sinon.spy(myObject, 'myMethod');
myObject.myMethod('test');
assert(spy.calledWith('test'));
```
