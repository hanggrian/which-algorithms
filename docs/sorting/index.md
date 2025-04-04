<div class="grid cards" markdown>
-   **Selection sort** [:material-information-outline:][selection_sort]

    ---

    :material-land-rows-horizontal:{ .xxxl }

    Easy to implement but performs the worst of them all.

-   **Bubble sort** [:material-information-outline:][bubble_sort]

    ---

    :material-swap-horizontal:{ .xxxl }

    Bubble sort or sinking sort, is better than selection sort but more complex
    than insertion sort.

-   **Insertion sort** [:material-information-outline:][insertion_sort]

    ---

    :material-cards-outline:{ .xxxl }

    Simple to implement and sufficient for smaller data sets.

-   **Merge sort** [:material-information-outline:][merge_sort]

    ---

    :material-source-merge:{ .xxxl }

    Efficiently sorts large data sets with divide and conquer.

-   **Quicksort** [:material-information-outline:][quicksort]

    ---

    :material-graph-outline:{ .xxxl }

    Expands on merge sort with a pivot to reduce the number of comparisons.

-    **Heapsort** [:material-information-outline:][heapsort]

    ---

    :material-family-tree:{ .xxxl }

    Reorganizes the data into a heap structure to sort it.
</div>

### Performance overview

Sort | Time complexity | Space complexity
--- | :---: | :---:
Selection sort | $\color{white} \fcolorbox{crimson}{firebrick} {Ω(n^2)}$ &rarr; $\color{white} \fcolorbox{crimson}{firebrick} {Θ(n^2)}$ &rarr; $\color{white} \fcolorbox{crimson}{firebrick} {O(n^2)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$
Bubble sort | $\color{black} \fcolorbox{gold}{yellow} {Ω(n)}$ &rarr; $\color{white} \fcolorbox{crimson}{firebrick} {Θ(n^2)}$ &rarr; $\color{white} \fcolorbox{crimson}{firebrick} {O(n^2)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$
Insertion sort | $\color{black} \fcolorbox{gold}{yellow} {Ω(n)}$ &rarr; $\color{white} \fcolorbox{crimson}{firebrick} {Θ(n^2)}$ &rarr; $\color{white} \fcolorbox{crimson}{firebrick} {O(n^2)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$
Merge sort | $\color{black} \fcolorbox{darkorange}{sandybrown} {Ω(n . log(n))}$ &rarr; $\color{black} \fcolorbox{darkorange}{sandybrown} {Θ(n . log(n))}$ &rarr; $\color{black} \fcolorbox{darkorange}{sandybrown} {O(n . log(n))}$ | $\color{black} \fcolorbox{gold}{yellow} {O(n)}$
Quicksort | $\color{black} \fcolorbox{darkorange}{sandybrown} {Ω(n . log(n))}$ &rarr; $\color{black} \fcolorbox{darkorange}{sandybrown} {Θ(n . log(n))}$ &rarr; $\color{white} \fcolorbox{crimson}{firebrick} {O(n^2)}$ | $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(log(n))}$
Heapsort | $\color{black} \fcolorbox{darkorange}{sandybrown} {Ω(n . log(n))}$ &rarr; $\color{black} \fcolorbox{darkorange}{sandybrown} {Θ(n . log(n))}$ &rarr; $\color{black} \fcolorbox{darkorange}{sandybrown} {O(n . log(n))}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$

[bubble_sort]: https://en.wikipedia.org/wiki/Bubble_sort "Bubble sort"
[heapsort]: https://en.wikipedia.org/wiki/Heapsort "Heapsort"
[insertion_sort]: https://en.wikipedia.org/wiki/Insertion_sort "Insertion sort"
[merge_sort]: https://en.wikipedia.org/wiki/Merge_sort "Merge sort"
[selection_sort]: https://en.wikipedia.org/wiki/Selection_sort "Selection sort"
[quicksort]: https://en.wikipedia.org/wiki/Quicksort "Quicksort"
