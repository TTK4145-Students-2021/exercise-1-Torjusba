Exercise 1 - Theory questions
-----------------------------
 
 ### What is the difference between concurrency and parallelism?
 Concurrency means that multiple tasks can start and complete in overlapping time. 
 Parallelism means that the tasks are running at the exact same time, for example on multiple cores.
 
 ### Why have machines become increasingly multicore in the past decade?
 Because we recently developed the technology required to create machines with more cores. Also, we've realized their potential in parallel processing.
 
 ### Why do we divide software (programs) into concurrently executing parts (like threads or processes)?
 Concurrency is used for increasing efficiency of systems that are not utilizing all of their resources at all times. By starting multiple processes in parallel, the machine can perform other tasks in time that would otherwise be used for waiting. 
 One good example is performing background tasks while waiting for external input.
 
 ### Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
 Both. It enables more elegant solutions to problems which require multiple focus areas, for example waiting for external input.
 Still, concurrency can make the life harder if not done properly, as concurrent programs require more effort to develop and debug.
 
 ### What is the conceptual difference between threads and processes?
 A process is assigned resources and memory. The process then contains one or multiple threads which executes instructions. The threads in a process share the process' assigned resources and memory. 

 ### Some languages support "fibers" (sometimes called "green threads") or "coroutines"? What are they?
 Fibers are special cases of threads, which use *cooperative multitasking* instead of *preemptive multitasking*. 
 That means that the processes communicate when to change context, instead of being controlled by the kernel's scheduling.
 
 ### What is the Go-language's "goroutine"? A C/POSIX "pthread"?
 A goroutine is an abstraction over OS threads that simplifies concurrency. They are managed by the Go Runtime Scheduler.
 A C/POSIX pthread is a raw OS thread.
 
 ### In Go, what does `func GOMAXPROCS(n int) int` change? 
It sets the maximum amount of CPUs that can execute simultaneously.



 
 
 
 
