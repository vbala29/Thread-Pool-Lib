# C++ Thread Pool Implementation

**Thread Pool API**

For more see thread_pool.hpp. 

```
typedef void (*workerFunction)(T, void* args);
ThreadPool(uint16_t num_workers, workerFunction wf);
void add_job(T job);
```
*Configure:* In *thread_pool_test.cpp* you can change number of jobs created (edit for loop bounds) and also the number of threads in the pool (edit ThreadPool ctor arg).

*Compile:* 
```
clang++ -std=c++14 main.cpp thread_pool.cpp thread_pool_test.cpp -o thread_pool
```

*Run:* 
```
./thread_pool
```
