# OpenMP_benchmark

## Compiling Commands:

### stencil/ 2d convolution
gcc -fopenmp -DPOLYBENCH_TIME -O2 -I../utilities convolution-2d.c ../utilities/polybench.c -o convolution-2d_acc

### Correlation / covariance (complicated)
gcc -fopenmp -DPOLYBENCH_TIME -O2 -I../../utilities correlation.c ../../utilities/polybench.c -o correlation_acc -lm
gcc -fopenmp -DPOLYBENCH_TIME -O2 -I../../utilities covariance.c ../../utilities/polybench.c -o covariance_acc -lm

### atax (mainly for SIMD)
gcc -fopenmp -DPOLYBENCH_TIME -O2 -I../utilities atax.c ../utilities/polybench.c -o atax_acc

### 3mm (matrix multiplication)
gcc -fopenmp -DPOLYBENCH_TIME -O2 -I../utilities 3mm.c ../utilities/polybench.c -o 3mm_acc

### openacc / gradient
<Yet To setup>

## Execution Commands:
./<executable_file>




