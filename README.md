# Queue
## Implementation of queue using array
![Screenshot (288)](https://user-images.githubusercontent.com/125993593/234153372-ecfca104-683f-4c7c-85fe-c0239bab5c49.png)
This C program implements a queue using an array. 
The program presents a menu to the user, allowing them to insert an element into the queue, delete an element from the queue, or display the elements in the queue.
The insert() function inserts an element at the end of the queue. 
If the queue is full (rear = MAX - 1), the function displays an error message.
If the queue is empty (front = -1), the function sets the front index to 0. 
The delete() function removes the element at the front of the queue.
If the queue is empty (front = -1) or if front is greater than rear, the function displays an error message. 
The delete() function removes the element at the front of the queue. 
If the queue is empty (front = -1) or if front is greater than rear, the function displays an error message. 
### Algorithm
1. Declare a constant MAX with a value of 50.
2. Declare an integer array named queue_array of size MAX.
3. Initialize rear and front to -1.
4. Define the insert() function:
    a. Declare an integer variable named add_item.
    b. Check if the queue is full (i.e., rear == MAX - 1). If it is, print "Queue Overflow" and return.
    c. If the queue is not full, check if the queue is initially empty (i.e., front == -1).
        i. If it is, set front to 0.
    d. Prompt the user to enter the element to be added to the queue.
    e. Read the value of add_item from the user.
    f. Increment rear by 1 and add add_item to queue_array at the position specified by rear.
5. Define the delete() function:
    a. Check if the queue is empty (i.e., front == -1 or front > rear). If it is, print "Queue Underflow" and return.
    b. If the queue is not empty, print the element at the front of the queue (i.e., queue_array[front]).
    c. Increment front by 1 to remove the element from the queue.
6. Define the display() function:
    a. Declare an integer variable named i and initialize it to front.
    b. Check if the queue is empty (i.e., front == -1). If it is, print "Queue is empty" and return.
    c. If the queue is not empty, print "Queue is:".
    d. Loop through the elements of the queue_array from i to rear, printing each element separated by a space.
    e. Print a newline character to end the output.
7. Define the main() function:
    a. Declare an integer variable named choice.
    b. Enter a loop that runs forever (i.e., while(1)).
        i. Print a menu with the following options:
            1. Insert element to queue
            2. Delete element from queue
            3. Display all elements of queue
            4. Quit
        ii. Prompt the user to enter a choice and read the value of choice from the user.
        iii. Use a switch statement to execute the appropriate function based on the user's choice (i.e., 1 calls insert(), 2 calls delete(), 3 calls display(), and 4 exits the program).

