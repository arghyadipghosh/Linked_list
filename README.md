# Linked_list
They are the datastructures which are user-defined using classes.
synatx:

class node{
int data;
node *next;
};


STATICALLY DECLARAATION OF LINKED LIST:

#include<iostream>
using namespace std;
class node{
	public:
	int data;
	node *next;
	
		node(int data){
			this->data=data;
			next=NULL;
		}
};
#include<iostream>
using namespace std;
#include"node.cpp"
void print(node *head){
	while(head!=NULL){
	
	cout<<head->data<<" ";
	head=head->next;
}
}
int main()
{
	node n1(1);
	node *head=&n1;
	node n2(2);
	node n3(3);
	node n4(4);
	node n5(5);
	n1.next=&n2;
	n2.next=&n3;
	n3.next=&n4;
	n4.next=&n5;
	
	print(head);
	//cout<<n1.data<<" "<<n2.data;
	
}







