# ClockTree-6500-Dataset

This repository contains 6,500 synthetic clock-tree test cases generated
for the study of useful-skew timing optimization and buffer insertion.

The test cases were generated according to the problem formulation and
input format of Problem D, *Timing Fixing by Useful Skew*, in the
2026 CAD Contest at ICCAD. The dataset was constructed for the
development and evaluation of graph neural network (GNN)-based
clock-tree optimization methods.

## Dataset Description

The dataset consists of 6,500 independently generated clock-tree test
cases, indexed from `case_0000` to `case_6499`.

Each test case contains a clock-tree structure and timing information
under two process corners:

- `clk_tree.structure`: clock-tree structure and buffer information.
- `SS_delay.rpt`: timing information under the SS process corner.
- `FF_delay.rpt`: timing information under the FF process corner.

The directory structure is organized as follows:

```text
dataset/
├── case_0000/
│   ├── clk_tree.structure
│   ├── SS_delay.rpt
│   └── FF_delay.rpt
├── case_0001/
│   ├── clk_tree.structure
│   ├── SS_delay.rpt
│   └── FF_delay.rpt
├── ...
└── case_6499/
    ├── clk_tree.structure
    ├── SS_delay.rpt
    └── FF_delay.rpt
```

## Buffer Library

The official `buf.lib` file is not included in this repository.

The buffer library used in our experiments is the official buffer
library provided for Problem D, *Timing Fixing by Useful Skew*,
of the 2026 CAD Contest at ICCAD.

Users should obtain the official buffer library separately from the
CAD Contest at ICCAD website.

2026 CAD Contest at ICCAD:  
https://www.iccad-contest.org/tw/