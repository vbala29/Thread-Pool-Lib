# C++ Thread Pool Implementation

**Thread Pool API**
See thread_pool.hpp. 

```
typedef void (*workerFunction)(T, void* args);
ThreadPool(uint16_t num_workers, workerFunction wf);
void add_job(T job);
```

*Compile: clang++ -std=c++14 main.cpp thread_pool.cpp thread_pool_test.cpp -o thread_pool
