# Activities

## Task 1:

- Refer to the following link. Discuss how Stacks based on linked lists works:
  https://www.cs.usfca.edu/~galles/visualization/StackLL.html
# A: Discussed

## Task 2:

The following snippet is from `./src/stack.cpp` lines 25-31.

```cpp
void push(StackNode **root, int new_data)
{
    StackNode *stackNode = newNode(new_data);
    stackNode->next = *root;
    *root = stackNode;
    cout << new_data << endl;
}
```

- Discuss in groups how the code works?
# A: Discussed
- Why do we need to use double pointers?
# A: Double pointers, or pointers to pointers, are used in some programming situations where we need to modify a pointer itself or when we want to create and modify a dynamic array of pointers.

## Task 3: Individual (At home)

Practice: Asymptotic Analysis and Upper Bounds. Refer to the following link:
https://opendsa-server.cs.vt.edu/OpenDSA/Exercises/AlgAnal/UpperBoundsSumm.html

# A: Practiced. Quite silly that this practice keeps repeating the same questions over and over again in a loop...