Brand new pintos for Operating Systems and Lab (CS330), KAIST, by Youngjin Kwon.

The manual is available at https://casys-kaist.github.io/pintos-kaist/.

### busy wait
```
// result: make check

pass tests/threads/alarm-single
pass tests/threads/alarm-multiple
pass tests/threads/alarm-simultaneous
FAIL tests/threads/alarm-priority
pass tests/threads/alarm-zero
pass tests/threads/alarm-negative
FAIL tests/threads/priority-change
FAIL tests/threads/priority-donate-one
FAIL tests/threads/priority-donate-multiple
FAIL tests/threads/priority-donate-multiple2
FAIL tests/threads/priority-donate-nest
FAIL tests/threads/priority-donate-sema
FAIL tests/threads/priority-donate-lower
FAIL tests/threads/priority-fifo
FAIL tests/threads/priority-preempt
FAIL tests/threads/priority-sema
FAIL tests/threads/priority-condvar
FAIL tests/threads/priority-donate-chain
FAIL tests/threads/mlfqs/mlfqs-load-1
FAIL tests/threads/mlfqs/mlfqs-load-60
FAIL tests/threads/mlfqs/mlfqs-load-avg
FAIL tests/threads/mlfqs/mlfqs-recent-1
FAIL tests/threads/mlfqs/mlfqs-fair-2
FAIL tests/threads/mlfqs/mlfqs-fair-20
FAIL tests/threads/mlfqs/mlfqs-nice-2
FAIL tests/threads/mlfqs/mlfqs-nice-10
FAIL tests/threads/mlfqs/mlfqs-block
22 of 27 tests failed.
```
```
// result: run alarm-single

Executing 'alarm-single':
...
Execution of 'alarm-single' complete.
Timer: 285 ticks
Thread: 0 idle ticks, 286 kernel ticks, 0 user ticks
```
```
// result: run alarm-multiple

Executing 'alarm-multiple':
...
Execution of 'alarm-multiple' complete.
Timer: 620 ticks
Thread: 0 idle ticks, 621 kernel ticks, 0 user ticks
```
### # 1 sleep wakeup 
```
// result: make check

pass tests/threads/alarm-single
pass tests/threads/alarm-multiple
pass tests/threads/alarm-simultaneous
FAIL tests/threads/alarm-priority
pass tests/threads/alarm-zero
pass tests/threads/alarm-negative
FAIL tests/threads/priority-change
FAIL tests/threads/priority-donate-one
FAIL tests/threads/priority-donate-multiple
FAIL tests/threads/priority-donate-multiple2
FAIL tests/threads/priority-donate-nest
FAIL tests/threads/priority-donate-sema
FAIL tests/threads/priority-donate-lower
FAIL tests/threads/priority-fifo
FAIL tests/threads/priority-preempt
FAIL tests/threads/priority-sema
FAIL tests/threads/priority-condvar
FAIL tests/threads/priority-donate-chain
FAIL tests/threads/mlfqs/mlfqs-load-1
FAIL tests/threads/mlfqs/mlfqs-load-60
FAIL tests/threads/mlfqs/mlfqs-load-avg
FAIL tests/threads/mlfqs/mlfqs-recent-1
FAIL tests/threads/mlfqs/mlfqs-fair-2
FAIL tests/threads/mlfqs/mlfqs-fair-20
FAIL tests/threads/mlfqs/mlfqs-nice-2
FAIL tests/threads/mlfqs/mlfqs-nice-10
FAIL tests/threads/mlfqs/mlfqs-block
22 of 27 tests failed.
```
```
// result: run alarm-single

Executing 'alarm-single':
...
Execution of 'alarm-single' complete.
Timer: 289 ticks
Thread: 250 idle ticks, 40 kernel ticks, 0 user ticks
```
```
// result: run alarm-multiple

Executing 'alarm-multiple':
...
Execution of 'alarm-multiple' complete.
Timer: 628 ticks
Thread: 550 idle ticks, 79 kernel ticks, 0 user ticks
```