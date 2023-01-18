#include <iostream>
using namespace std;

// Node class for linked list
class Node {
public:
    int data;
    Node* next;
};

// Stack class
class Stack {
private:
    Node* top;

public:
    Stack() { top = NULL; }

    // Function to push an element to the stack
    void push(int value) {
        Node* newNode = new Node();
        newNode->data = value;
        newNode->next = top;
        top = newNode;
    }

    // Function to pop the topmost element from the stack
    int pop() {
        if (top == NULL) {
            cout << "underflow" << endl;
            return -1;
        }
        Node* temp = top;
        top = top->next;
        int value = temp->data;
        delete temp;
        return value;
    }

    // Function to display the contents of the stack
    void display() {
        if (top == NULL) {
            cout << "empty stack" << endl;
            return;
        }
        Node* temp = top;
        while (temp != NULL) {
            cout << temp->data << " ";
            temp = temp->next;
        }
        cout << endl;
    }
};

int main() {
    Stack stack;
    int choice, value;
    while (true) {
        cin >> choice;
        if (choice == 0) break;
        switch (choice) {
            case 1:
                cin >> value;
                stack.push(value);
                break;
            case 2:
                value = stack.pop();
                break;
            case 3:
                stack.display();
                break;
            default:
                cout << "Invalid choice" << endl;
        }
    }
    return 0;
}
