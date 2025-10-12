
## Computer Hardware Core Components
- CPU
- Memory
- IO Controller

## Computer Structure
- Early computer connect all components in one Bus, IO devices are much slower than cpu and memory, to coordinate IO and Bus speed, every IO device shall has a IO controller.
- Due to CPU frequency improvement, memory speed is slower than cpu, so there's a system bus appears with same memory frequency. CPU communicate system bus with multi-frequency. Since system bus adopts PCI structure, so we call system bus with PCI bus. The south bridge chip is also called PCI bridge.
- GPU improve a lot later, and IO bus can't meet the speed of CPU, memory, GPU, so the north brigde chip came out. It handle the high speed communication.
- The south bridge chip to handle slow speed IO devices, like hardware disk, usb, keyboard. these devices connect the bus called ISA bus. The south bridge chip is also called ISA bridge.

## Operation System
- System call interface implemented by Sofeware Interrupt
- Multi-tasking system, application run with Process, process has separate address space, CPU distribute resource based on process priority, it's called Preemptive
- Send IO commend to hardware through I/O Port Register, I/O Port Register is a chip on motherboard, different IO hardware is assigned with different port address. Two instructions `in`, `out`
- Virtual Address maps process address to physical address. Segmentation and Paging.
- Thread, Lightweight Process. Using multi-core CPU ability. Priority Schedule, Round Robin.
- 