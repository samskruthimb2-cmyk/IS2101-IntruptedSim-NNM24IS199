# IS2101-IntruptedSim-NNM24IS199


# Descripton
This program simulates interrupt handling for multiple I/O devices using threads and mutex locks in C.
It demonstrates how interrupts from devices like Keyboard, Mouse, and Printer are received and serviced based on masking and prioritization.

# Features
	•	Simulates three I/O devices:
	•	Keyboard – High Priority
	•	Mouse – Medium Priority
	•	Printer – Low Priority
	•	Uses multithreading (pthreads) to represent concurrent interrupts.
	•	Demonstrates masking (enabling/disabling certain interrupts).
	•	Uses mutex locks to prevent race conditions while handling interrupts.
	•	Randomly triggers interrupts for simulation realism.

# Input
This program does not require user input — it automatically simulates interrupts from devices randomly.

# Run and Compile
gcc interrupt_sim.c -o interrupt_sim -lpthread
interrupt_sim

# Sample Output 
=== INTERRUPT HANDLER SIMULATION ===
Priority: Keyboard > Mouse > Printer

Keyboard Interrupt Received -> Processing ISR -> Done
Interrupt Ignored (Masked Device)
Printer Interrupt Received -> Processing ISR -> Done
Keyboard Interrupt Received -> Processing ISR -> Done

All interrupts handled successfully. Execution complete.

# Output:

![WhatsApp Image 2025-10-29 at 21 10 15_48aa8255](https://github.com/user-attachments/assets/70beeebc-17e9-4a27-87e7-9ab8bec34b12)


# Conclusion
This program demonstrates how interrupts from different I/O devices are handled using threads and mutex locks.
It shows the concept of priority, masking, and synchronization in interrupt handling.
Overall, it gives a clear idea of how an Interrupt Service Routine (ISR) works in real systems.




