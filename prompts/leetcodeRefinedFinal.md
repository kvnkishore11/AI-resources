# Optimized LeetCode Problem-Solving Template

## Problem Analysis (2-3 minutes)

**Problem Restatement:**
```
I need to [describe the core task] where the input is [input description] and the expected output is [output description].
```

**Constraints & Edge Cases:**
- What are the input size limits? (n ≤ ?)
- Are there special cases to handle? (empty inputs, negative values, duplicates)
- What should I return for invalid inputs?
- Time/space complexity requirements?

**Visual Problem Representation:**
```
Draw or describe a visual representation of the problem:
- For arrays/strings: Show example elements with indices
- For trees/graphs: Sketch the structure with nodes and connections
- For matrices: Draw a small example grid
```

## Pattern Recognition (3-5 minutes)

**Problem Classification:**
- Does this problem involve searching, sorting, or transformation?
- Is this a classic pattern? (sliding window, two pointers, BFS/DFS, dynamic programming, etc.)
- What data structures might be helpful? (hash map, stack, queue, heap, etc.)

**Pattern Visualization:**
```
If this matches a known pattern, visualize how the pattern applies:
- For sliding window: Show window movement through array
- For two pointers: Show pointer positions and movements
- For tree traversal: Show traversal order with numbered steps
```

## Solution Development (5-8 minutes)

**Approach Brainstorming:**
1. **Brute Force Approach:**
   - Simple solution without optimization
   - Time & space complexity analysis
   
2. **Optimized Approach(s):**
   - How can I improve the brute force solution?
   - Can I use a specific data structure to optimize?
   - Time & space complexity analysis
   
3. **Selected Approach:**
   - Why I'm choosing this approach (clarity, efficiency, etc.)
   - Key insight that makes this approach work

**Step-by-Step Algorithm Visualization:**
```
1. Create a visual flowchart or state diagram showing:
   - Initial state
   - Key transformation steps
   - Decision points
   - Final state

2. Walk through a simple example visually:
   - Show the state of variables at each step
   - Use arrows, colors, or annotations to highlight changes
   - Demonstrate how edge cases are handled
```

## Implementation (10-20 minutes)

**Pseudocode:**
```
Write high-level pseudocode that outlines:
- Function signature
- Variable initialization
- Main logic blocks
- Return statement
```

**Code Implementation:**
```python
def solution(input_params):
    # Step 1: Initialize variables
    
    # Step 2: Core algorithm implementation
    
    # Step 3: Handle edge cases
    
    # Step 4: Return result
    return result
```

**Visual Trace-Through:**
```
For input example [example_input]:
1. Initial state: variables = {...}
2. After step 1: variables = {...}
3. After step 2: variables = {...}
...
Final output: [example_output]

Draw the execution flow with variable states at each step.
```

## Verification & Optimization (3-5 minutes)

**Test Cases:**
1. Normal case: [example]
2. Edge case 1 (e.g., empty input): [example]
3. Edge case 2 (e.g., single element): [example]
4. Complex case: [example]

**Complexity Analysis:**
- Time Complexity: O(?) - Explain why
- Space Complexity: O(?) - Explain why
- Can this be further optimized? If yes, how?

**Code Refinement:**
- Any redundant operations?
- Can we simplify the logic?
- Are there cleaner ways to express the solution?

## Interview Communication Tips

**Narrating Your Thought Process:**
- "I notice this problem is similar to [related problem]..."
- "My first instinct is to try [approach], but let me think if there's a more efficient way..."
- "A key insight here is that [observation]..."
- "I'm choosing this approach because [reasoning]..."

**Time Management Checkpoints:**
- 2-3 minutes: Problem understanding complete
- 5-8 minutes: Approach selected and explained
- 15-25 minutes: Implementation complete
- 25-30 minutes: Testing and optimization complete

**Visual Communication Techniques:**
- "Let me draw this to make it clearer..."
- "Visually, the algorithm works like this..."
- "If we trace through with this example, we can see..."
- "This diagram shows how the state changes at each step..."

## Pattern Library Reference

**Common Patterns & Their Visual Signatures:**

1. **Sliding Window:**
   - Visual: |[  ]| → |  [ ]| → |   [ ]|
   - When to use: Contiguous subarrays/substrings with constraints

2. **Two Pointers:**
   - Visual: [L→ ... ←R] or [→ →]
   - When to use: Sorted arrays, pair finding, palindromes

3. **Fast & Slow Pointers:**
   - Visual: [S→ ... F→→]
   - When to use: Cycle detection, middle elements

4. **Binary Search:**
   - Visual: [L ... M ... R] → [L ... M] or [M ... R]
   - When to use: Sorted arrays, search space reduction

5. **Tree Traversal:**
   - Visual: Root → Left → Right (pre-order)
   - When to use: Tree exploration, path finding

6. **Graph Traversal:**
   - Visual: BFS (level by level) or DFS (deep paths first)
   - When to use: Connected components, shortest paths

7. **Dynamic Programming:**
   - Visual: Build table from base cases
   - When to use: Optimization problems with overlapping subproblems

8. **Backtracking:**
   - Visual: Decision tree with branches
   - When to use: Combinatorial problems, permutations

Remember to adapt this template based on the specific problem type and your personal strengths!
