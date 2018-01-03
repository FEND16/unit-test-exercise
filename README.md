# unit-test-exercise

Write unit tests for this todo-application. The code is located inside of `src` and you are going to write all your tests in `__tests__/todo.js`. Feel free to implement more functionality and test that functionality.

## Installation

```bash
git clone https://
cd unit-test-exercise
yarn
```
```bash
git clone https://
cd unit-test-exercise
npm install
```

## Run tests

Single run
```bash
yarn test
```
```bash
npm run test
```

Watch mode
```bash
yarn test:watch
```
```bash
npm run test:watch
```

## Jest syntax

I have written a first test for you to start with:
```js
/* So the functionalty is tested in isolation. This means
 * that each new test doesn't know anything about the previous
 * when mutating the state  (the list of todos) it is important
 * that we reset the state after each test */
beforeEach(() => {
  jest.resetModules();
});

test('returns all todos', () => {
  /* require the list for each test to guarantee isolated tests */
  const todoList = require('../src/todoList');
  expect(todoList.getAllTodos()).toHaveLength(4);
});
```

## Solution

Some example solutions is located under the branch [`solution`]()