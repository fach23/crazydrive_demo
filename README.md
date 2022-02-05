# crazydrive_demo
This repository contains demo of the crazdrive trajectory planner. The source code might be published in the future. 

- The trajectory planner uses a nonlinear kinematic vehicle model represented in curvilinear coordinates.
- The trajectory planner is implemented in C++ and makes use of acados. More specifically the RTI scheme, the gauss newton hessian approximation and the QP Solver HPIPM with partial condensing is used.
- The mean runtime of one planning cycle is 4ms (min: 2ms, max: 10ms) on a laptop with Intel® Core™ i7-4600U CPU @ 2.10GHz × 4.


https://user-images.githubusercontent.com/51156083/152644705-dc174ba1-cde2-4e14-ba11-e8b66ea330fb.mp4

