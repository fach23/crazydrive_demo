# crazydrive_demo
This repository contains demo of the crazdrive trajectory planner. The source code might be published in the future. 

- The trajectory planner uses a nonlinear kinematic vehicle model represented in curvilinear coordinates. The four state variables are chosen to be station, velocity, acceleration and curvature. The control variables are chosen to be longitudinal jerk and curvature rate.
- The objective can be adapted to different use cases (comfort --> public road vs. time-optimal --> racing).
- Time dependent constraints w.r.t. station, velocity, acceleration, jerk, curvature, curvature rate, lateral acceleration, total acceleration can be specified.
- The trajectory planner is implemented in C++ and makes use of acados. More specifically the RTI scheme, the gauss newton hessian approximation and the QP Solver HPIPM with partial condensing is used.
- The mean runtime of one planning cycle is 4ms (min: 2ms, max: 10ms) on a laptop with Intel® Core™ i7-4600U CPU @ 2.10GHz × 4.


https://user-images.githubusercontent.com/51156083/152644705-dc174ba1-cde2-4e14-ba11-e8b66ea330fb.mp4

