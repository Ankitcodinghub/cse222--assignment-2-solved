# cse222--assignment-2-solved
**TO GET THIS SOLUTION VISIT:** [CSE222 -Assignment #2 Solved](https://www.ankitcodinghub.com/product/cse222-assignment-2-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;95932&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSE222 -Assignment #2  Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
In this assignment, you’re going to implement a linked list using dynamic memory.

MAIN NODE STRUCTURE

Your linked list will be constructed from nodes, similar to what you used in PA1:

struct node{

int data;

struct node *next;

}; where

data is the integer actually stored in the list; and

next is the memory location of the next element, or NULL for the end of the list.

Declare a sentinel node pointer in your main program as follows: struct node *list;

NECESSARY FUNCTIONS

You should implement the following functions:

struct node *init()

(this is the one function whose prototype changes from PA1)

This should return a pointer to an empty list. An empty list has a sentinel node pointing to NULL (indicating there are no other nodes in the list besides the sentinel).

int add(struct node*list,int number)

This should add a node the list, to store number in the list. The list should always be sorted, smallest to largest. The function returns 1 if successful, 0 if not successful (i.e. there is no memory left for creating a new node).

void print(struct node*list)

This routine will print the nodes in the linked list “list.” Since the nodes are stored in sorted order, the printed list should automatically appear in sorted order too.

int delete(struct node*list, int number)

This routine deletes the node containing “number” from the list “list.” This function returns 1 if the node as deleted, 0 if not (i.e. the node was not found in the list).

int search(struct node*list, int number)

This searches the linked list for a node containing the given number. It returns 1 if the node is found, 0 if it is not found.

The above routines represent the interface between a main program and the linked list as an abstract data type (ADT). They must behave exactly as described above, in the way described below.

</div>
</div>
<div class="layoutArea">
<div class="column">
Each element in the linked list (collection of struct nodes) contains 2 fields:

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
<ul>
<li>a data field, which is the stored number; and</li>
<li>a next field, which has the address of the next node, or the value NULL.
To add a number to the list, create a new node, search the list for the proper point to insert the new node, adjust the prior node’s “next” field to point to the new node, and adjust the new node’s “next” field accordingly.

Similar actions are taken for printing, searching and deleting, as discussed in class.

You should use malloc(sizeof(struct node)) to get the address of a new node; and free(ptr) to release a node from memory (after deleting it, or at the end of the program).

MAIN PROGRAM

You should use the above functions to implement a main program which lets the user manipulate a linked list. It is important that the main program never manipulate the data structure directly. All manipulation should be done via the above routines (this is the idea of encapsulation/information hiding/ADTs).

The first thing your program should do is initialize an empty linked list.

Next, the program should prompt the user for input using the prompt

&gt;

and then wait for the user to enter a command followed by the ENTER key. The program then processes the command, as follows:

i number (where number is any legal integer).

This will insert the number into the list, in order (smallest to largest), provided the node is not already in the list. It should then print

the message “SUCCESS”; “NODE ALREADY IN LIST”; or “OUT OF MEMORY.”

p

This will print the list in order, on one line, with the numbers separated by spaces

s number

This searches for the given number, and prints either “FOUND” or “NOT FOUND”

d number

This deletes the node containing the given number, and prints either “SUCCESS” or “NODE NOT FOUND”

x

This should cause the program to exit after freeing all allocated memory (use valgrind to confirm this)

(anything else)

should print a synopsis of legal commands.

The program should return to showing a prompt, and wait for another command.
</li>
</ul>
</div>
</div>
</div>
