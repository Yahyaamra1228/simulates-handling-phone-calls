# simulates-handling-phone-calls
C# console application simulates handling phone calls in a call center using a queue and a timer.

Call Class:

Defines a Call class with properties for the caller's identity, name, and the duration of the call.
Global Variables:

Declares global variables for a timer (timer) and a queue of Call objects (callQueue).
Main Method:

Initializes a Queue<Call> (callQueue) and adds sample Call objects to it.
Displays the initial contents of the call queue.
Creates a Timer (timer) to simulate call handling and sets it to run the HandleCall method.
HandleCall Method:

Dequeues a call from the front of the queue (if the queue is not empty).
Simulates handling the call by sleeping the thread for the duration of the call.
Displays information about the handled call.
Enqueues the next call (if there are more calls in the queue) and restarts the timer for the next call.
DisplayCallQueue Method:

Displays the contents of the call queue, excluding the currently handled call.
Prints the caller's identity, name, and call duration for each call in the queue.
This code is a simple simulation of a call center where calls are queued, and a timer is used to handle each call sequentially. The timer is set to trigger the HandleCall method, which dequeues a call, simulates call handling, and enqueues the next call if available. The console output displays the status of the call queue before and after handling each call.
