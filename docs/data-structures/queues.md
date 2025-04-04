## Java

Operation | PriorityQueue [:material-information-outline:][priority_queue] | LinkedList [:material-information-outline:][linked_list] | ArrayDequeue [:material-information-outline:][array] | ConcurrentLinkedQueue [:material-information-outline:][linked_list] | ArrayBlockingQueue [:material-information-outline:][array] | PriorityBlockingQueue [:material-information-outline:][priority_queue] | SynchronousQueue | DelayQueue [:material-information-outline:][priority_queue] | LinkedBlockingQueue [:material-information-outline:][linked_list]
--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---:
Offer | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(log(n))}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(log(n))}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(log(n))}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$
Peek | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$
Poll | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(log(n))}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(log(n))}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(log(n))}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$
Remove | $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{black} \fcolorbox{gold}{yellow} {O(n)}$
Size | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$

## Python

Operation | collections.deque [:material-information-outline:][linked_list]
--- | :---:
Copy | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$
Append | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$
Append left |$\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$
Pop | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$
Pop left | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$
Extend | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {Θ(k)}$ &rarr; $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(k)}$
Extend left | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {Θ(k)}$ &rarr; $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(k)}$
Rotate | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {Θ(k)}$ &rarr; $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(k)}$
Remove | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$
Get length | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$

[array]: https://en.wikipedia.org/wiki/Array_(data_structure) "Array"
[linked_list]: https://en.wikipedia.org/wiki/Linked_list "Linked list"
[priority_queue]: https://en.wikipedia.org/wiki/Priority_queue "Priority queue"
