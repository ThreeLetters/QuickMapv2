# QuickMapv2
Quickmap, but much better

## The Plan
Use a key-value array with a Doubly-LinkedList
### Insertion: 
1. Add the node to the linked list (var linkedlistnode = linkedlist.insert(node))
2. Add the linkedlist node into the array as the key (arr[key] = linkedlistnode)

### Deletion:
1. Get linkedlistnode from array.
2. do linkedlistnode.destroy();

### Loop
1. Loop through linkedlist

## Why?

Item deletion is expensive. But removing the pointer isnt. Also, why not use a key-value pair?

## Notes

1. Do not insert with a key used before unless you delete it with `delete()` - It wont check duplicates for efficiency
2. Do not delete a key that has not been inserted. - It wont check if it exsists for efficiency
3. Do not get from a key that has not been inserted yet - It wont check for efficiency.
