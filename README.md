# Cell-Life-Stimulation
Consider a rectangular grid of dimensions MxN. The initial configuration of cell life will be provided as an input file. Cell life should be simulated for the next 100 generations.

A generation of cell life passes to the next generation by adhering to the following rules:

1. A cell having four or more neighbors will die due to overpopulation.

2. A cell having exactly two or three neighbors will survive the next step.

3. A cell having one or zero neighbors will die due to under population.

4. A dead cell with exactly three neighbors will get a life.

##Input Format
The first line of the input specifies two integers separated by a space - M, N. The next M rows contain N characters each. ‘-’ (ASCII 45) indicates a dead cell, whereas ‘*’ (ASCII 42) indicates a live cell. The dimensions will not exceed 1000x1000 size.

Input:

35

\ --*--

\ --*--

\ --*--

##Output
At step=1: // Cell at (1,3), (3,3) die (Rule 3.). Cell at (2,3) lives (Rule 2.). New cells come up at (2,2), (2,4)

\ -----

\ -***-

\ -----

At step=2: // The configuration is reverted back to the initial configuration.

\ --*--

\ --*--

\ --*--

.... // For the next 98 steps, the configuration keeps alternating.
