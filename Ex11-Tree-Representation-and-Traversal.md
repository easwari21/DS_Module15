# Ex11 Tree Representation and Traversal

## AIM:
To write a C function to perform post order traversal of a binary tree.

## Algorithm
1. Start and define display_postorder(root_node).
2. If root_node is not null, recursively call left and right children.
3. After both calls, print the current node’s value.
4. End
  
## Program:
```
Program to perform post order traversal of a binary tree.
Developed by: Easwari M
RegisterNumber: 212223240033 

struct node
{
int value;
struct node*left_child, *right_child;
};*/
void display_postorder(struct node*root_node){
if(root_node)
{
display_postorder(root_node->left_child);
display_postorder(root_node->right_child);
printf("%d\n",root_node->value);
}
}

```

## Output:
![image](https://github.com/user-attachments/assets/719d2585-96cf-4dde-bc22-57e5099e6d2b)


## Result:
Thus, the function to perform post order traversal of a binary tree is implemented successfully
