# Ada Shallow Copy Pitfall

This example highlights a common issue in Ada: the behavior of array assignments.  Unlike some languages that automatically create deep copies, Ada's assignment for arrays creates a *shallow copy*.  This means that both variables point to the same underlying data structure. Any changes made to one array will also be reflected in the other.

The code in `bug.ada` demonstrates this behavior.  The solution in `bugSolution.ada` illustrates a way to avoid this problem using an explicit loop to create a deep copy.
