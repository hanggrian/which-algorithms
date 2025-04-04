## Java

Operation | HashMap [:material-information-outline:][hash_table] | LinkedHashMap [:material-information-outline:][hash_table] | IdentityHashMap [:material-information-outline:][array] | WeakHashMap [:material-information-outline:][hash_table] | EnumMap [:material-information-outline:][array] | TreeMap [:material-information-outline:][red_black_tree] | ConcurrentHashMap [:material-information-outline:][hash_table] | ConcurrentSkipListMap [:material-information-outline:][skip_list]
--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---:
Get | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(log(n))}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(log(n))}$
Contains | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(log(n))}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(log(n))}$
Next | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(h / n)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(h / n)}$ | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(h / n)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(log(n))}$ | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(h / n)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$

## Python

Operation | dict [:material-information-outline:][hash_table]
--- | :---:
`k in d` | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$
Copy | $\color{black} \fcolorbox{gold}{yellow} {O(n)}$
Get item | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$
Set item | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$
Delete item | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$
Iteration | $\color{black} \fcolorbox{gold}{yellow} {O(n)}$

[array]: https://en.wikipedia.org/wiki/Array_(data_structure) "Array"
[hash_table]: https://en.wikipedia.org/wiki/Hash_table "Hash table"
[red_black_tree]: https://en.wikipedia.org/wiki/Red-black_tree "Red-black tree"
[skip_list]: https://en.wikipedia.org/wiki/Skip_list "Skip list"
