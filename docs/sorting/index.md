# Sorting

<img
  width="640"
  src="../images/sorting.webp"
  alt="Can you like, shut up?">

<div class="grid cards" markdown>
-   **Selection sort** [:material-information-variant:][selection-sort]

    ---

    [:material-view-sequential-outline:{ .xxxl }](selection-sort.md)

    Selection sort is an in-place comparison sorting algorithm.

    [:material-arrow-right: Use cases](selection-sort.md#use-cases)

-   **Bubble sort** [:material-information-variant:][selection-sort]

    ---

    [:material-swap-horizontal-bold:{ .xxxl }](bubble-sort.md)

    Repeatedly steps through the input list element by element, comparing the
    current element with the one after it, swapping their values if needed.

    :material-arrow-right: Use cases

-   **Insertion sort** [:material-information-variant:][insertion-sort]

    ---

    [:material-cards-outline:{ .xxxl }](insertion-sort.md)

    Builds the final sorted array (or list) one item at a time by comparisons.

    :material-arrow-right: Use cases

-   **Merge sort** [:material-information-variant:][merge-sort]

    ---

    [:material-source-merge:{ .xxxl }](merge-sort.md)

    Efficient, general-purpose, and comparison-based sorting algorithm.

    :material-arrow-right: Use cases

-   **Quicksort** [:material-information-variant:][quicksort]

    ---

    [:material-graph-outline:{ .xxxl }](quicksort.md)

    Slightly faster than merge sort and heapsort for randomized data,
    particularly on larger distributions.

    :material-arrow-right: Use cases

-    **Heapsort** [:material-information-variant:][heapsort]

    ---

    [:material-family-tree:{ .xxxl }](heapsort.md)

    Reorganizes an input array into a heap (a data structure where each node
    is greater than its children) and then repeatedly removes the largest
    node from that heap, placing it at the end of the array.

    :material-arrow-right: Use cases
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

[bubble-sort]: https://en.wikipedia.org/wiki/bit-array "Wikipedia: Bubble sort"
[heapsort]: https://en.wikipedia.org/wiki/Heapsort "Wikipedia: Heapsort"
[insertion-sort]: https://en.wikipedia.org/wiki/Insertion_sort "Wikipedia: Insertion sort"
[merge-sort]: https://en.wikipedia.org/wiki/Merge_sort "Wikipedia: Merge sort"
[selection-sort]: https://en.wikipedia.org/wiki/Selection_sort "Wikipedia: Selection sort"
[quicksort]: https://en.wikipedia.org/wiki/Quicksort "Wikipedia: Quicksort"
