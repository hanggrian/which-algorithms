## Java

Operation | ArrayList [:material-information-outline:][array] | LinkedList [:material-information-outline:][linked_list] | CopyOnWriteArrayList [:material-information-outline:][array]
--- | :---: | :---: | :---:
Add | $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$
Remove | $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$
Get | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{black} \fcolorbox{gold}{yellow} {O(n)}$
Contains | $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{black} \fcolorbox{gold}{yellow} {O(n)}$
Next | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$

## Python

Operation | list [:material-information-outline:][array]
--- | :---:
Copy | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$
Append | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$
Pop last | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$
Pop intermediate | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$
Insert | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$
Get item | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$
Set item | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$
Delete item | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$
Iteration | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$
Get slice | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {Θ(k)}$ &rarr; $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(k)}$
Del slice | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$
Set slice | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {Θ(k + n)}$ &rarr; $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(k + n)}$
Extend | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {Θ(k)}$ &rarr; $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(k)}$
Sort | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {Θ(log(n))}$ &rarr; $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(log(n))}$
Multiply | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {Θ(n . k)}$ &rarr; $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(n . k)}$
`x in s` | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$
`mins(s)`, `max(s)` | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$
Get length | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$

[array]: https://en.wikipedia.org/wiki/Array_(data_structure) "Array"
[linked_list]: https://en.wikipedia.org/wiki/Linked_list "Linked list"
