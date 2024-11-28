# Push_swap

Push_swap is a 42 school project that challenges students to implement a sorting algorithm using a constrained set of stack operations. The goal is to sort a list of integers in ascending order using two stacks (`a` and `b`) while minimizing the number of operations.

## Project Overview

The project requires writing a program, `push_swap`, which:
- Reads a list of integers as input.
- Uses two stacks (`a` and `b`) and a set of predefined operations to sort the integers in ascending order in stack `a`.
- Outputs the sequence of operations needed to achieve the sorted order.

### Allowed Operations

The following operations are permitted in this project:

- **Swap**:
  - `sa`: Swap the top two elements of stack `a`.
  - `sb`: Swap the top two elements of stack `b`.
  - `ss`: Perform `sa` and `sb` simultaneously.

- **Push**:
  - `pa`: Push the top element of stack `b` onto stack `a`.
  - `pb`: Push the top element of stack `a` onto stack `b`.

- **Rotate**:
  - `ra`: Rotate stack `a` upwards (top element becomes bottom).
  - `rb`: Rotate stack `b` upwards.
  - `rr`: Perform `ra` and `rb` simultaneously.

- **Reverse Rotate**:
  - `rra`: Rotate stack `a` downwards (bottom element becomes top).
  - `rrb`: Rotate stack `b` downwards.
  - `rrr`: Perform `rra` and `rrb` simultaneously.

### Goals

- The sorted integers must end up in stack `a`.
- Minimize the total number of operations.

## What I Learned

1. **Stack Operations**:
   - Implementing and managing data structures like stacks.
   - Visualizing how operations affect the state of the stacks.

2. **Sorting Algorithms**:
   - Adapting sorting algorithms (like quick sort) to work within the constraints of stack-based operations.
   - Designing efficient solutions for small and large data sets.

3. **Optimization**:
   - Minimizing the number of operations while ensuring correctness.
   - Balancing time complexity and the project constraints.

4. **Debugging and Testing**:
   - Building comprehensive test cases to validate edge cases.
   - Handling invalid input gracefully.

5. **Algorithm Design**:
   - Breaking down problems into smaller, manageable steps.
   - Translating high-level algorithms into stack operations.

## How to Use

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/push_swap.git
   cd push_swap
   ```

2. **Compile the Program**:
   Use the provided Makefile:
   ```bash
   make
   ```

3. **Run the Program**:
   Provide a list of integers as arguments:
   ```bash
   ./push_swap 4 2 3 1 5
   ```
   The program outputs the sequence of operations to sort the integers.

4. **Check Your Solution** (if applicable):
   Use the optional `checker` program to verify the correctness of the operations (if implemented).

## Challenges Faced

- Designing a scalable solution for larger inputs while adhering to project constraints.
- Debugging and testing edge cases, such as duplicate numbers or invalid inputs.
- Striking a balance between performance and simplicity in algorithm implementation.
