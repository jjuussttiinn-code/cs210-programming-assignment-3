### Entry 1
**Date:** 2026-04-21
**Entry Type:** Engineering Decision
**Task worked on:** Defined the DFS function signature and required parameters
**Issue or decision:** Needed a clear structure for the recursive maze search implementation
**Error message / symptom (if applicable):** None
**What I tried:** Added the full `dfs(...)` function signature with all required arguments
**Fix / resolution (or final decision):** Created the DFS scaffold to allow later recursive logic to be added
**Commit(s):** Add DFS function signature with parameters

### Entry 2
**Date:** 2026-04-23
**Entry Type:** Bug Fix
**Task worked on:** Implemented DFS validation checks
**Issue or decision:** DFS must ignore invalid positions and prevent revisiting cells
**Error message / symptom (if applicable):** None
**What I tried:** Added out-of-bounds, wall, and visited checks in the DFS body
**Fix / resolution (or final decision):** Ensured DFS only explores valid, unvisited open cells
**Commit(s):** Add DFS base case checks for bounds, walls, and visited cells

### Entry 3
**Date:** 2026-04-29
**Entry Type:** Bug Fix
**Task worked on:** Added visited marking and exit detection
**Issue or decision:** DFS needed to track visited cells and stop when it reached the exit
**Error message / symptom (if applicable):** None
**What I tried:** Marked each cell as visited and returned true when the current cell was the exit
**Fix / resolution (or final decision):** Prevented cycles and allowed successful exit detection
**Commit(s):** Mark visited cells and add exit check in DFS

### Entry 4
**Date:** 2026-04-30
**Entry Type:** Engineering Decision
**Task worked on:** Added recursive neighbor exploration and parent tracking
**Issue or decision:** Needed correct traversal order plus path reconstruction support
**Error message / symptom (if applicable):** None
**What I tried:** Loop over direction vectors, assign parent coordinates, and recurse into neighbors
**Fix / resolution (or final decision):** Completed recursive DFS logic and prepared parent arrays for path printing
**Commit(s):** Add recursive DFS calls and parent coordinates before recursion

### Entry 5
**Date:** 2026-05-05
**Entry Type:** Engineering Decision
**Task worked on:** Integrated DFS invocation into main program flow
**Issue or decision:** The search routine needed to be executed on the generated maze
**Error message / symptom (if applicable):** None
**What I tried:** Uncommented and enabled the `dfs(...)` call in `main()`
**Fix / resolution (or final decision):** Program now actually performs DFS from the entrance cell
**Commit(s):** Enable DFS call in main

### Entry 6
**Date:** 2026-05-05
**Entry Type:** Edge Case
**Task worked on:** Enabled path printing and no-path fallback output
**Issue or decision:** Needed correct final user output based on whether DFS succeeded
**Error message / symptom (if applicable):** None
**What I tried:** Uncommented the `printPath(...)` block and the `No path exists.` fallback
**Fix / resolution (or final decision):** Program prints the reconstructed path when found or a failure message otherwise
**Commit(s):** Enable path printing and no-path fallback in main