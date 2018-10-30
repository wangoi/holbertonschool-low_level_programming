# C - More singly linked lists
In this project, I continued to practice building and using singly linked lists in C.

## Helper File
* `lists.h`: Header file containing definitions and prototypes for all types and functions written for the project.

| Type/File             | Definition/Prototype                                                             |
| --------------------- | -------------------------------------------------------------------------------- |
| `struct listint_s`    | <ul><li>`int n`</li><li>`struct listint_s *next`</li></ul>                       |
| `typedef listint_t`   | `struct listint_s`                                                               |
| `0-print_listint.c`   | `size_t print_listint(const listint_t *h);`                                      |
| `1-listint_len.c`     | `size_t listint_len(const listint_t *h);`                                        |
| `2-add_nodeint.c`     | `listint_t *add_nodeint(listint_t **head, const int n);`                         |
| `3-add_nodeint_end.c` | `listint_t *add_nodeint_end(listint_t **head, const int n);`                     |
| `4-free_listint.c`    | `void free_listint(listint_t *head);`                                            |
| `5-free_listint2.c`   | `void free_listint2(listint_t **head);`                                          |
| `6-pop_listint.c`     | `int pop_listint(listint_t **head);`                                             |
| `7-get_nodeint.c`     | `listint_t *get_nodeint_at_index(listint_t *head, unsigned int index);`          |
| `8-sum_listint.c`     | `int sum_listint(listint_t *head);`                                              |
| `9-insert_nodeint.c`  | `listint_t *insert_nodeint_at_index(listint_t **head, unsigned int idx, int n);` |
| `10-delete_nodeint.c` | `int delete_nodeint_at_index(listint_t **head, unsigned int index);`             |

## Task
* **Print list**
  * `0-print_listint.c`: C function that prints all the elements of a `listint_t` linked list.
    * Returns the number of nodes in the `listint_t` list.

* **List length**
  * `1-listint_len.c`: C function that returns the number of elements in a `listint_t` linked list.

* **Add node**
  * `2-add_nodeint.c`: C function that adds a new node at the beginning of a `listint_t` linked list.
    * If the function fails - returns `NULL`.
    * Otherwise - returns the address of the new element.

* **Add node at the end**
  * `3-add_nodeint_end.c`: C function that adds a new node at the end of a `listint_t` linked list.
    * If the function fails - returns `NULL`.
    * Otherwise - returns the address of the new element.

* **Free list**
  * `4-free_listint.c`: C function that frees a `listint_t` linked list.

* **Free**
  * `5-free_listint2.c`: C function that frees a `listint_t` linked list.
    * Sets the `head` to `NULL`.

* **Pop**
  * `6-pop_listint.c`: C function that deletes the head node of a `listint_t` linked list.
    * If the linked list is empty - returns `0`.
    * Otherwise - returns the head node's data (`n`).

* **Get node at index**
  * `7-get_nodeint.c`: C function that locates a given node of a `listint_t` linked list.
    * If the node does not exist - returns `NULL`.
    * Otherwise - returns the located node.

* **Sum list**
  * `8-sum_listint.c`: C function that returns the sum of all the data (`n`) of a `listint_t` linked list.
    * If the linked list is empty - returns `0`.
    * Otherwise - returns the sum of all the data (`n`).

* **Insert**
  * `9-insert_nodeint.c`: C function that inserts a new node to a `listint_t` linked list at a given position.
    * If it is not possible to add the new node at index `idx`, or the function fails - returns `NULL`.
    * Otherwise - returns the address of the new node.

* **Delete at index**
  * `10-delete_nodeint.c`: C function that deletes the node at a given index of a `listint_t` linked list.
    * If the function succeeds - returns `1`.
    * If the function fails - returns `-1`.