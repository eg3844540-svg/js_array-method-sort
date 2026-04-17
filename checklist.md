1. Implement only `Array.prototype.sort2` - do NOT override `Array.prototype.sort`.
2. `sort2` must return the original array (the same reference, not a new one), so the caller can chain calls on it.
3. `sort2` must sort the array in place (mutate the original array).
4. When `compareFunction` is not provided, sort elements as strings (convert to string, then compare by character codes). Numbers like `[3, 12, 2, 11]` must become `[11, 12, 2, 3]`.
5. When `compareFunction` is provided, use it to determine order: negative result → first before second, positive → first after second, zero → keep order.
6. Do NOT call the built-in `Array.prototype.sort` inside your implementation - write your own sorting algorithm (e.g. bubble sort, insertion sort).
7. Define `sort2` via `[].__proto__.sort2 = function(compareFunction) { ... }` inside `applyCustomSort` - keep the given structure in `src/arrayMethodSort.js`.
8. Use descriptive variable names (e.g. `compareFunction`, `currentElement`), avoid one-letter names except for loop indices.
9. Prefer `const` over `let` where the value doesn't change.
