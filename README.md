# thread-and-multithread-python

Multiprocessing vs Threading Python

#The threading module uses threads, the multiprocessing module uses processes. 
The difference is that threads run in the same memory space, while processes have separate memory. 
This makes it a bit harder to share objects between processes with multiprocessing. 
Since threads use the same memory, precautions have to be taken or two threads will write to the same memory at the same time. 
This is what the global interpreter lock is for.


#MULTIPROCESSING

Multiprocessing adds CPUs to increase computing power.
Multiple processes are executed concurrently.
Creation of a process is time-consuming and resource intensive.
Multiprocessing can be symmetric or asymmetric.

"The multiprocessing library in Python uses separate memory space, multiple CPU cores, bypasses GIL limitations in CPython, child processes are killable (ex. function calls in program) and is much easier to use.
Some caveats of the module are a larger memory footprint and IPC’s a little more complicated with more overhead".

#
MULTIPROCESSING

Multiprocessing adds CPUs to increase computing power.
Multiple processes are executed concurrently.
Creation of a process is time-consuming and resource intensive.
Multiprocessing can be symmetric or asymmetric.
The multiprocessing library in Python uses separate memory space, multiple CPU cores, bypasses GIL limitations in CPython, child processes are killable (ex. function calls in program) and is much easier to use.
Some caveats of the module are a larger memory footprint and IPC’s a little more complicated with more overhead.
MULTITHREADING

Multithreading creates multiple threads of a single process to increase computing power.
Multiple threads of a single process are executed concurrently.
Creation of a thread is economical in both sense time and resource.

"The multithreading library is lightweight, shares memory, responsible for responsive UI and is used well for I/O bound applications.
The module isn’t killable and is subject to the GIL.
Multiple threads live in the same process in the same space, each thread will do a specific task, have its own code, own stack memory, instruction pointer, and share heap memory."

resource

https://stackoverflow.com/questions/3044580/multiprocessing-vs-threading-python
