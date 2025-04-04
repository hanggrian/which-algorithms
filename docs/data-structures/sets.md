## Java

Operation | HashSet [:material-information-outline:][hash_table] | LinkedHashSet [:material-information-outline:][hash_table] | EnumSet [:material-information-outline:][bit_array] | TreeSet [:material-information-outline:][red_black_tree] | CopyOnWriteArraySet [:material-information-outline:][array] | ConcurrentSkipListSet [:material-information-outline:][skip_list]
--- | :---: | :---: | :---: | :---: | :---: | :---:
Add | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(log(n))}$ | $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(log(n))}$
Remove | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(log(n))}$ | $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(log(n))}$
Contains | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(log(n))}$ | $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(log(n))}$
Next | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(h / n)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(log(n))}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$
Size | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{black} \fcolorbox{gold}{yellow} {O(n)}$

## Python

Operation | set [:material-information-outline:][hash_table]
--- | :---:
`x in s` | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$
Union `s|t` | $\color{black} \fcolorbox{gold}{yellow} {Θ(len(s) + len(t))}$
Intersection `s&t` | $\color{black} \fcolorbox{gold}{yellow} {Θ(min(len(s), len(t)))}$ &rarr; $\color{black} \fcolorbox{darkorange}{sandybrown} {O(len(s) . len(t))}$
Multiple intersection `s1&s2&...&sn` | $\color{black} \fcolorbox{darkorange}{sandybrown} {(n - 1) . O(l)}$<br>$\small{\textsf{where} l = \mathtt{max}(\mathtt{len}(s1), \ldots, \mathtt{len}(sn))}$
Difference `s-t` | $\color{black} \fcolorbox{gold}{yellow} {Θ(len(s))}$
`s.difference_update(t)` | $\color{black} \fcolorbox{gold}{yellow} {Θ(len(t))}$
Symmetric Difference `s^t` | $\color{black} \fcolorbox{gold}{yellow} {Θ(len(s))}$ &rarr; $\color{black} \fcolorbox{darkorange}{sandybrown} {O(len(s) . len(t))}$
`s.symmetric_difference_update(t)` | $\color{black} \fcolorbox{gold}{yellow} {Θ(len(t))}$ &rarr; $\color{black} \fcolorbox{darkorange}{sandybrown} {O(len(s) . len(t))}$

[array]: https://en.wikipedia.org/wiki/Array_(data_structure) "Array"
[bit_array]: https://en.wikipedia.org/wiki/Bit_array "Bit array"
[hash_table]: https://en.wikipedia.org/wiki/Hash_table "Hash table"
[red_black_tree]: https://en.wikipedia.org/wiki/Red-black_tree "Red-black tree"
[skip_list]: https://en.wikipedia.org/wiki/Skip_list "Skip list"
