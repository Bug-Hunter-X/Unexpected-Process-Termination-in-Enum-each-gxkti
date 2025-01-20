# Elixir Enum.each and Process.exit() Bug

This repository demonstrates a subtle bug that can occur when using `Process.exit()` within an `Enum.each` loop in Elixir.  The code may terminate prematurely, leading to incomplete processing of the list. The solution demonstrates safer alternatives for handling such scenarios.

## Bug Description
The `bug.ex` file contains code that iterates through a list. If a specific condition is met, `Process.exit()` is called to terminate the process. This can cause the loop to stop before all elements are processed, resulting in unexpected behavior.

## Solution
The `bugSolution.ex` file provides alternative approaches that avoid premature termination, ensuring all elements are handled appropriately.