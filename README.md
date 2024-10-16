# Exp-17

## Aim:
To implement basic operations on a singly linked list in C++ including node creation and inserting nodes at the head of the list.

## Software Used:
- Dev c++
  
## Theory:
A linked list is a dynamic data structure consisting of nodes, where each node contains data and a pointer to the next node in the sequence. Unlike arrays, linked lists are not stored in contiguous memory locations, making them more efficient for operations like insertion and deletion. The first code demonstrates how to create a single node, while the second code builds on this by inserting nodes at the head of the list and displaying the list.

## Program 1: Node Creation.
<strong> Code: </strong>
<br>
```cpp
// Premish Ninawe
// 23070123092
// ENTC B1
#include<iostream>
using namespace std;
class Link{
    public:
    int data ;
    Link* next;
    Link(int num){
        data = num;
        next = NULL;
    }
};
int main(){
    Link* l1 = new Link(6);
    cout << l1->data<<"   "<<l1->next;
}
```
<strong> Output: </strong>
<br>

## Program 2: Adding Nodes and Displaying the List.
<strong> Code: </strong>
<br>
```cpp
// Premish Ninawe
// 23070123092
// ENTC B1
#include<iostream>
using namespace std;
class Link{
    public:
    int data ;
    Link* next;
    Link(int num){
        data = num;
        next = NULL;
    }
};
void insert_head(Link* &head, int data){
    Link* new_node = new Link(data);
    new_node -> next= head;
    head = new_node;
}
void disp(Link*head){
    Link*temp = head;
    while (temp!= NULL){
        cout<<temp->data<<"->";
        temp = temp->next;

    }
    cout<<"NULL"<<endl;
}

int main(){
    Link*head = NULL;
    insert_head(head, 30);
    disp(head);
    insert_head(head, 32);
    disp(head);
    insert_head(head,35);
    disp(head);
}

```
<strong> Output: </strong>
<br>


## Conclusion:
Through these programs, we learned how to create and manipulate a singly linked list in C++. The first code illustrates node creation, while the second code demonstrates how to insert nodes at the head and display the list. Linked lists provide an efficient way to manage data dynamically.
