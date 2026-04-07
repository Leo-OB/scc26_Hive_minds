# Hive_minds Task 5:

## Benchmarks results with screenshots:
Step 1 Job allocation:
```bash
salloc --partition=club --time=59:00 -N 2 --ntask-per-node=8 --job-name=hpl_test --nodelist=com6,com7
```
![code uses to create a job allocation](job1.png)

Step 2 Running mpirun:
```bash
#since we allowed 16 task we used 8 cores on each of the two comes
mpirun -np 16 --host com6:8,com7:18 ./xhpl
```
![code used to run the benchmark](mpirun1.png)
