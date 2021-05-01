# LinuxNamespace
Test IPC's in linux SysV and POSIX on native and namespace environments

# How to run

## GUI

run ```sudo pyhton3 Linux_IPC_GUI.py```

## C program

First you must build using

```sudo ./build.script```
Then you can run the exe with the following options:
  - IPC Type 
  - Posix Vs SysV
  - Namespace vs Native
  - Iteration count
  - Loop count
 
Here are the numbers cooresponding to the correct build

To run all :          0

Posix semaphores:     5

Posix Message Queues: 6

Posix Shared Memory:  7

SysV semaphores:      9

SysV Message Queues:  10

SysV Shared Memory:   11


Namespace = 1

Native = 2

Here is an example run of posix semaphores in a namespace iterating 100 times with 50 samples:

```sudo ./build/LNDriver/LNDriver 5 1 100 50```


### OR

run

```sudo ./run_all.script``` 
to run the executable for all IPCS


## For specific IPCS

run 
```sudo ./run_ipcname_enivironment_library```

so for example, if you want to run semaphores in a namespace using posix you write

```sudo ./run_sem_namespace_posix```
