# LinkedList Implementation in Python

This Python script defines a simple linked list and provides various operations for manipulating it. Below is a Markdown-formatted README explaining the classes and methods in the script.

## `Node` Class

### `__init__(self, data=None, next=None)`
- **Parameters:**
  - `data`: The data to be stored in the node.
  - `next`: Reference to the next node in the linked list.
- **Description:** Initializes a node with the given data and reference to the next node.

## `LinkedList` Class

### `__init__(self)`
- **Description:** Initializes an empty linked list with a `head` attribute set to `None`.

### `print(self)`
- **Description:** Prints the elements of the linked list in the format `data1 --> data2 --> ...`.

### `get_length(self)`
- **Returns:** The length (number of nodes) of the linked list.
- **Description:** Counts and returns the number of nodes in the linked list.

### `insert_at_beginning(self, data)`
- **Parameters:**
  - `data`: The data to be inserted at the beginning of the linked list.
- **Description:** Inserts a new node with the given data at the beginning of the linked list.

### `insert_at_end(self, data)`
- **Parameters:**
  - `data`: The data to be inserted at the end of the linked list.
- **Description:** Inserts a new node with the given data at the end of the linked list.

### `insert_at(self, index, data)`
- **Parameters:**
  - `index`: The position at which the data is to be inserted.
  - `data`: The data to be inserted.
- **Description:** Inserts a new node with the given data at the specified index in the linked list.

### `remove_at(self, index)`
- **Parameters:**
  - `index`: The position of the node to be removed.
- **Description:** Removes the node at the specified index from the linked list.

### `insert_values(self, data_list)`
- **Parameters:**
  - `data_list`: A list of data elements to be inserted into the linked list.
- **Description:** Clears the existing linked list and inserts the elements from the provided list.

### `insert_after_value(self, data_after, data_to_insert)`
- **Parameters:**
  - `data_after`: The data value after which a new node is to be inserted.
  - `data_to_insert`: The data to be inserted.
- **Description:** Inserts a new node with the given data after the first occurrence of the specified value in the linked list.

### `remove_by_value(self, data)`
- **Parameters:**
  - `data`: The data value to be removed from the linked list.
- **Description:** Removes the first occurrence of the specified value from the linked list.

## Example Usage

```python
if __name__ == '__main__':
    ll = LinkedList()
    ll.insert_values(["banana","mango","grapes","orange"])
    ll.print()
    
    ll.insert_after_value("mango","apple")
    ll.print()
    
    ll.remove_by_value("orange")
    ll.print()
    
    ll.remove_by_value("figs")
    ll.print()
    
    ll.remove_by_value("banana")
    ll.remove_by_value("mango")
    ll.remove_by_value("apple")
    ll.remove_by_value("grapes")
    ll.print()
