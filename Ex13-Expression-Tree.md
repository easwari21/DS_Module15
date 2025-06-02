# Ex13 Expression Tree

## AIM:
To write a C function to construct an Expression Tree for the given Postfix Expression and display the output in the format of In-order ,Pre-order and Post-order traversal.

## Algorithm
1. Print node data in preorder then traverse left then right
2. Traverse left in inorder then print node data then traverse right
3. Traverse left in postorder then traverse right then print node data
4. Recursive approach is used for all three traversal methods
5. Functions handle each tree node using tree->d, tree->l, tree->r
   

## Program:
```
Program to construct an Expression Tree for the given Postfix Expression and display the output in the format of In-order ,Pre-order and Post-order traversal.
Developed by: Easwari M
RegisterNumber: 212223240033 

void preOrder(struct n*tree)
{
if(tree)
{
printf("%c",tree->d);
preOrder(tree->l);
preOrder(tree->r);
}
}
void inOrder(struct n*tree)
{
if(tree)
{
inOrder(tree->l);
printf("%c",tree->d);
inOrder(tree->r);
}
}
void postOrder(struct n*tree)
{
if(tree)
{
postOrder(tree->l);
postOrder(tree->r);
printf("%c",tree->d);
}
}

```

## Output:
![image](https://github.com/user-attachments/assets/ea67a6f2-1860-4c7d-900d-f0f2c16ce010)


## Result:
Thus, the C program to display the Expression Tree in the format of In-order ,Pre-order and Post-order traversal.
