# Elixir List Modification During Enum.each Iteration

This example demonstrates a common pitfall in Elixir when attempting to modify a list while iterating over it using `Enum.each`.  `Enum.each` is designed for side effects, not for modifying the collection it's iterating over.  Attempting to do so leads to unexpected results.

The provided `bug.exs` file shows this issue. The solution, `bugSolution.exs`, demonstrates a correct approach using `Enum.reduce` or `Enum.filter`.