# Data structures

<img
  width="640"
  src="../images/data_structures.jpg"
  alt="By now your name and particulars have been fed into every laptop, desktop, mainframe and supermarket scanner that collectively make up the global information conspiracy, otherwise known as &quot;The Beast.&quot;">

<div class="grid cards" markdown>
-   **Lists**

    ---

    [:material-format-list-bulleted:{ .xxxl }](lists.md)

    Array, list or any indexed collection of elements.

    [:material-arrow-right: Which one to use?](lists.md#which-one-to-use)

-   **Queues**

    ---

    [:material-tray-full:{ .xxxl }](queues.md)

    Queue, stack or any FIFO or LIFO collection of elements.

    [:material-arrow-right: Which one to use?](queues.md#which-one-to-use)

-   **Sets**

    ---

    [:material-table-row:{ .xxxl }](sets.md)

    Set or any collection of unique elements.

    [:material-arrow-right: Which one to use?](sets.md#which-one-to-use)

-   **Maps**

    ---

    [:material-table-large:{ .xxxl }](maps.md)

    Map, dictionary or any collection of key-value pairs.

    [:material-arrow-right: Which one to use?](maps.md#which-one-to-use)
</div>

### Performance overview

Data structure | Access | Search | Insert | Delete
--- | :---: | :---: | :---: | :---:
Lists | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$
Queues | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$
Sets | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$
Maps | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$
