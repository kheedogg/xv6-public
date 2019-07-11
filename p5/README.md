# xv6 Page fault handler


## What is implemeted

- Initial size of stack: Prepare 1 page initially. Can be grow up to 4 pages

- Growth of stack: tf->esp can move up to 32bytes. New page should be allocated to this process if current stack is full

- When stack pointer reaches guard page or a process accesses invalid address, kill that process

- Print out “Invalid access” when approaching abnormal address

- Print out “Allocate page” if page-fault handler is executed normally

## Change log
### Changed files
- `proc.h`
- `exec.c`
- `proc.c`
- `vm.c`
- `trap.c`


### proc.h

### exec.c

### proc.c

### vm.c

### trap.c
