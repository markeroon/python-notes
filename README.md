Python Data Structures Notes
============================

Lists
-----

`lst = []`

`lst.append(x)` append x to end of list

`lst.extend(x)` append items in x to end of list

`lst.insert(i,x)` insert item at given position, will be followed by item that previously occupied that position

`lst.index(x)` position of item x in lst

`lst.remove(x)` remove first found instance of x in lst

`lst.pop([i])` default arg is -1, which will pop the last element and return it

##Using a list to model a stack##
```
stack = []
```

`push` ->
```
lst.append('x')
stack = ['x']

lst.append('y')
stack = ['x','y']

```

`pop` ->
```
lst.pop()
(stack == ['x'])
```
`peek` ->
```
stack[len(stack)-1]
```

Queues
------
Pop left is inefficient in a regular queue

```
import deque
```
queue = deque([])
queue.append('x')
queue.append('y')
queue.popleft()
```
```(queue ==  ['y'])```
