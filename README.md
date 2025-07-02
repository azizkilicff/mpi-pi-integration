# MPI π Integration

This project approximates the value of π using the midpoint rule and parallel computing with MPI.

## How it works

It integrates the function `f(x) = 4 / (1 + x^2)` from 0 to 1 using:

- The midpoint numerical integration rule
- MPI parallel processing with any number of processes

## Compile and Run

```bash
mpicc project5_2.c -o project5_2 -lm
mpirun -np 4 ./project5_2 1000000
