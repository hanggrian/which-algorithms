<div class="grid cards" markdown>
-   **Lists**

    ---

    :material-format-list-bulleted:{ .xxxl }

    Array, list or any indexed collection of elements.

    [:material-arrow-right: Java](lists#java)&emsp;[:material-arrow-right: Python](lists#python)

-   **Queues**

    ---

    :material-tray-full:{ .xxxl }

    Queue, stack or any FIFO or LIFO collection of elements.

    [:material-arrow-right: Java](queues#java)&emsp;[:material-arrow-right: Python](queues#python)

-   **Sets**

    ---

    :material-table-row:{ .xxxl }

    Set or any collection of unique elements.

    [:material-arrow-right: Java](sets#java)&emsp;[:material-arrow-right: Python](sets#python)

-   **Maps**

    ---

    :material-table-large:{ .xxxl }

    Map, dictionary or any collection of key-value pairs.

    [:material-arrow-right: Java](maps#java)&emsp;[:material-arrow-right: Python](maps#python)
</div>

### Performance overview

Data structure | Access | Search | Insert | Delete
--- | :---: | :---: | :---: | :---:
Lists | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$
Queues | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$
Sets | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$
Maps | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {Θ(1)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$
