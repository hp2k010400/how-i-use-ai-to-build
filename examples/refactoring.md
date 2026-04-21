# Refactoring with AI

## Context

When working on projects, code can become repetitive or harder to maintain as features are added.

I use AI to help quickly clean up and improve existing code without changing functionality.

---

## Before

```js
function getPrices(items) {
  let result = [];
  for (let i = 0; i < items.length; i++) {
    if (items[i].price) {
      result.push(items[i].price);
    }
  }
  return result;
}

Prompt I Used

"Can you refactor this function to be cleaner and more modern JavaScript while keeping the same functionality?"

function getPrices(items) {
  return items
    .filter(item => item.price)
    .map(item => item.price);
}

Result
Reduced lines of code
Improved readability
Easier to maintain and extend
Key Takeaway

AI is very effective for improving code quality and readability.

However, I always review the output to ensure:

the logic remains correct
the changes fit the wider codebase

This allows me to move faster while still maintaining control over the code.
