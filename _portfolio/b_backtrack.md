---
title: "Backtrack"
excerpt: "A biophysics tool for tracking cell motion and division.
Backtrack uses Deep learning-based segmentation and motion tracking (MOT) algorithms.
Integrated SSN (Spatiotemporal Sequence Networks) for improved cell tracking and segmentation of E. coli microscope data, optimizing tracking accuracy and performance. Optimized deep learning model performance for biological datasets using PyTorch, NumPy, OpenCV, scikit-image.

Bactrack is inspired by ultrack. Bactrack uses segmentation hierarchy to allow various segmentation scenarios, and hierarchy is built on Omnipose dynamic/pixel clustering logic, and using MIP solver to assign cell from frame to frame by maximize weights.

For assignment algorithm, Bactrack includes following MIP solvers: HiGHS, CBC, Gurobi for tracking assignment task. All of these MIP solver will return the same optimized global maximum result but with different run-time speed. For performance comparsion between MIP solvers check this benchmark. In short, the speed of Gurobi is the fastest (Gurobi > HiGHS > CBC).
[Github repository](https://github.com/yyang35/bactrack)
<br/><img src='/images/gui.png'>"
collection: "https://github.com/yyang35/bactrack"

---

[https://github.com/yyang35/bactrack](https://github.com/yyang35/bactrack)

A biophysics tool for tracking cell motion and division.
Backtrack uses Deep learning-based segmentation and motion tracking (MOT) algorithms.
Integrated SSN (Spatiotemporal Sequence Networks) for improved cell tracking and segmentation of E. coli microscope data, optimizing tracking accuracy and performance. Optimized deep learning model performance for biological datasets using PyTorch, NumPy, OpenCV, scikit-image.


Bactrack is inspired by ultrack(paper). Bactrack uses segmentation hierarchy to allow various segmentation scenarios, and hierarchy is built on Omnipose dynamic/pixel clustering logic, and using MIP solver to assign cell from frame to frame by maximize weights.

For assignment algorithm, Bactrack includes following MIP solvers: HiGHS, CBC, Gurobi for tracking assignment task. All of these MIP solver will return the same optimized global maximum result but with different run-time speed. For performance comparsion between MIP solvers check this benchmark. In short, the speed of Gurobi is the fastest (Gurobi > HiGHS > CBC).

( Those tools are not directly be used, but through Python interface libraries: specifically: Scipy.milp for HiGHS, and python_mip for CBC and Gurobi. So if you look at solvers name: MipSolver,ScipySolver, it's interface name rather than solver name)


