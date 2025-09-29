# nextvertex
is a streaming BFS frontier expander for unweighted graphs. Given the current frontier $$F_t$$ and a global `visited` bitset, it reads neighbors, atomically test-and-sets `visited[v]`, and emits a vertex precisely once. The core is a fixed-II=1 pipeline that sustains one neighbor per cycle after fill, with deterministic latency and no duplicates.

### Suggested reading
1. [Dr. BFS: Data Centric Breadth-First Search on FPGAs](https://asherliu.github.io/docs/dac19.pdf)
2. [SMT Based Verification: Symbolic Haskell theorem prover using SMT solving.](https://hackage.haskell.org/package/sbv)
3. [Refinement Types for Haskell](https://ranjitjhala.github.io/static/refinement_types_for_haskell.pdf)
4. [FPGP: Graph Processing Framework on FPGA](https://dai.sjtu.edu.cn/my_file/pdf/c04da8ca-cca4-4e1d-90cb-5c55f490736e.pdf)
5. [Boosting the Performance of FPGA-based Graph Processor using Hybrid Memory Cube: A Case for Breadth First Search](https://www.isfpga.org/past/fpga2017/slides/D3_S2_01.pdf)
6. [Under the hood of Formal Verification](https://tomverbeure.github.io/rtl/2019/01/04/Under-the-Hood-of-Formal-Verification.html)
7. [ThunderGP: HLS-based Graph Processing Framework on FPGAs](https://www.comp.nus.edu.sg/~wongwf/papers/FPGA2021.pdf)
8. [Graph Processing on FPGAs: Taxonomy, Survey, Challenges](https://arxiv.org/pdf/1903.06697)
