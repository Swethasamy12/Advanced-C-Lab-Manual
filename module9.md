EXP NO:11 C PROGRAM TO DISPLAY STACK ELEMENTS USING AN ARRAY.

Aim:
To write a C program to display stack elements using an array.
Algorithm:
1.	Include Necessary Header Files
2.	Declare Global Variables
3.	Define the Display Function
4.	Main Function (or Other Relevant Code)
5.	Initialize the stack and top as needed.
6.	Perform stack operations (push, pop, etc.).
7.	Use the display function to visualize the stack's contents
 
Program:
```
int stack[100],top,i;
void display()
{
    if(top==-1)
    {
        printf("Stack is empty");
    }
    else
    {
        for(i=top;i>=0;i--)
        {
            printf("%d\n",stack[i]);
        }
    }
}
```

Output:

<img width="1140" height="536" alt="503307944-3f00cea1-70ec-4485-b440-4914697b3fdb" src="https://github.com/user-attachments/assets/f6ee970c-ff95-4b2b-9226-cb947c268224" />




Result:
Thus, the program to display stack elements using an array is verified successfully.
 

EXP NO:12  PROGRAM TO PUSH THE GIVEN ELEMENT IN TO A STACK USING ARRAY.

Aim:
To create a C program to push the given element in to a stack using array.
Algorithm:
1.	Declare global variables for the stack size, top index, and the stack itself.
2.	Define the push function to add a floating-point number to the stack.
3.	Initialize the stack size, top index, and the stack itself.
4.	Call the push function as needed.
 
Program:
```
float stack[100];
int size=3,top=-1;
void push (float data)
{
    if (top == size-1 )
    {
    printf("stack is full\n");
    }
    else
    {
        top = top+1;
        stack[top] = data;
    }
}
```
Output:


<img width="1422" height="662" alt="503308527-aa150f0f-24f8-4da9-abd8-d5a7c05f0baf" src="https://github.com/user-attachments/assets/0b697ee9-994c-462f-b66a-4c12a38b5664" />


Result:
Thus, the program to push the given element in to a stack using array is verified successfully


 
EXP NO:13 C PROGRAM TO DISPLAY QUEUE ELEMENTS USING ARRAY.
Aim:
To write a C program to display queue elements using array

Algorithm:
1.	Declare global variables for the queue, rear, front, and iteration.
2.	Define the display function to print the elements of the queue.
3.	Initialize the queue, rear, and front as needed.
4.	Call the display function and perform other queue operations as needed.
 
Program:
```
int queue[50], rear=-1, front=-1;
void display()
{
    if(front==-1 || front>rear)
    {
        printf("No elements to display");
    }
    else
    {
        for(int i=front;i<=rear;i++)
        {
            printf("%d\n",queue[i]);
        }
    }
}
```

Output:

<img width="1376" height="641" alt="503308960-0577635e-c31a-420e-9662-b45b3357621d" src="https://github.com/user-attachments/assets/63941cb8-beb3-4092-af03-471b79b2644d" />



Result:
Thus, the program to display queue elements using array is verified successfully.


 
EXP NO:14 C PROGRAM TO INSERT ELEMENTS IN QUEUE USING ARRAY.
Aim:
To write a C program to insert elements in queue using array.

Algorithm:
1.	Declare global variables for the size, rear, front, and the queue itself.
2.	Define the enqueue function to add a float to the queue.
3.	Initialize the rear, front, and size of the queue as needed.
4.	Call the enqueue function as needed.

Program:
```
float queue[50];
int front=-1,rear=-1,size=10;
void enqueue(float data)
{
    if(rear==size-1)
    {
        printf("Queue Overflow");
    }
    else
    {
        if(front==-1)
        {
            front=0;
        }
        rear++;
        queue[rear]=data;
    }
}
```

Output:

<img width="1136" height="456" alt="503309379-a57107f3-dcaf-42b4-bef4-528f3afe4d71" src="https://github.com/user-attachments/assets/36a35af8-4620-4b03-8336-ce9570450783" />

 

Result:
Thus, the program to insert elements in queue using array is verified successfully.



 
EXP NO:15 C FUNCTION TO DELETE ELEMENTS IN QUEUE USING ARRAY



Aim:

To create a function in C that deletes an element from a queue implemented using an array.

Algorithm:

1.	Check if the Queue is Empty
o	If the front pointer is -1, it means the queue is empty, and there are no elements to delete. Print a message indicating that the queue is empty.
2.	Delete the Front Element
o	If the queue is not empty, the element at the front index is deleted.
o	Increment the front pointer by 1 to remove the element and point to the next element in the queue.
3.	Check if the Queue Becomes Empty After Deletion:
o	After deletion, check if the front pointer has passed the rear pointer (front > rear). If this is true, reset both front and rear to -1, indicating that the queue is now empty.
4.	End the Function.



Program:
```
int front, rear;
void dequeue()
{
    if(front == -1 || front>rear)
    {
        printf("Queue is empty\n");
    }
    else
    {
        front++;
    }
}
```


Output:


<img width="1212" height="695" alt="503310371-f47b5bf1-4abe-4ca1-a0bb-7d257f49392c" src="https://github.com/user-attachments/assets/1d1ae588-f319-417a-9ea1-66d48e0d5ddc" />


Result:
Thus, the function that deletes an element from a queue implemented using an array is verified successfully.
