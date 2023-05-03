# stack & queue 

A stack is a data structure consisting of nodes with no reference to their previous node, only to the next node. It is a last-in-first-out (LIFO) structure,
where the first item added to the stack will be the last item to be removed from the stack.
The push operation adds a node to the top of the stack and is an O(1) operation,
and the pop operation removes the top node from the stack and is also an O(1) operation.
The peek operation retrieves the value of the top node without removing it, and the isEmpty operation returns true when the stack is empty.
A queue is another data structure, but it is a first-in-first-out (FIFO) structure where the first item added to the queue will be the first item removed.
The enqueue operation adds a node to the rear of the queue, and the dequeue operation removes a node from the front of the queue. The front of the queue is the first node,
and the rear is the last node. If the dequeue operation is called when the queue is empty, an exception will be raised.
