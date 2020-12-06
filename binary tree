#include <iostream> 
#include <bits/stdc++.h> 
using namespace std; 

typedef struct Node 
{ 
    int data; 
    struct Node* left, *right; 
    Node(int data) 
    { 
        this->data = data; 
        left = right = NULL; 
    } 
}; 

void printPostorder(Node* node) 
{ 
    if (node == NULL) 
        return; 

    printPostorder(node->left); 
    printPostorder(node->right); 
    cout << node->data << " "; 
} 
  
void printInorder(Node* node) 
{ 
    if (node == NULL) 
        return; 
    printInorder(node->left); 
    cout << node->data << " "; 
    printInorder(node->right); 
} 
  
void printPreorder(Node* node) 
{ 
    if (node == NULL) 
        return; 
    cout << node->data << " "; 
    printPreorder(node->left);  
    printPreorder(node->right); 
}  
  
void printPostorder_using_one_stack(Node *root)
{
    
}

int main() 
{ 
    Node *root        = new Node(1); 
    root->left        = new Node(2); 
    root->right       = new Node(3); 
    root->left->left  = new Node(4); 
    root->left->right = new Node(5);  
  
    cout << "\nPreorder traversal of binary tree is \n"; 
    printPreorder(root); 
    cout << "\nInorder traversal of binary tree is \n"; 
    printInorder(root);  
    cout << "\nPostorder traversal of binary tree is \n"; 
    printPostorder(root); 
    cout << "\nPostorder traversal of binary tree using one stack is \n"; 
    printPostorder_using_one_stack(root);
    
    return 0; 
} 
