# Linked-List-.cpp

# include<iostream>

using namespace std;
class node {
    public:
    int data;
    node *next;
};
int main()
{
    int n,i;
    node *ptr = new node();
    node *head = new node();
    ptr = head;
    ptr->data = 10;
    ptr->next = NULL;
    cout<<"Enter the nodes to make\n";
    cin>>n;
    for(i=0;i<n-1;i++)
    {
        ptr->next = new node();
        ptr = ptr->next;
        cout<<"Enter the data\n";
        cin>> ptr->data;
    }
    ptr->next = NULL;
    cout<<"Our data is\n";
     ptr = head;
    while(ptr != NULL)
    {
        cout<<ptr->data<<"\n";
        ptr = ptr->next;
    }
    return 0;

}
