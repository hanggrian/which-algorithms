# Searching

!!! quote
    &ldquo;Computers are useless. They can only give you answers.&rdquo;
    &mdash; *Pablo Picasso*

<div class="grid cards" markdown>
-   **Linear search** [:material-information-variant:][linear-search]

    ---

    [:material-dots-horizontal:{ .xxxl }](linear-search.md)

    Sequentially checks each element of the list until a match is found

    [:material-arrow-right: Use cases](linear-search.md#use-cases)

-   **Binary search** [:material-information-variant:][binary-search]

    ---

    [:material-set-split:{ .xxxl }](binary-search.md)

    Compares the target value to the middle element of the array, eliminating half of the search range each iteration.

    [:material-arrow-right: Use cases](binary-search.md#use-cases)

-   **Depth-first search** [:material-information-variant:][depth-first-search]

    ---

    [:material-arrow-expand-vertical:{ .xxxl }](depth-first-search.md)

    Explores as far as possible along each branch before backtracking.

    :material-arrow-right: Use cases

-   **Breadth-first search** [:material-information-variant:][breadth-first-search]

    ---

    [:material-arrow-expand-horizontal:{ .xxxl }](breadth-first-search.md)

    Explores all nodes at the present depth prior to moving on to the nodes at
    the next depth level.

    :material-arrow-right: Use cases
</div>

### Performance overview

Search | Time complexity | Space complexity
--- | :---: | :---:
Linear search | $\color{white} \fcolorbox{limegreen}{forestgreen} {Ω(1)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {Θ(n)}$ &rarr; $\color{black} \fcolorbox{gold}{yellow} {O(n)}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$
Binary search | $\color{white} \fcolorbox{limegreen}{forestgreen} {Ω(1)}$ &rarr; $\color{black} \fcolorbox{yellowgreen}{greenyellow} {Θ(log(n))}$ &rarr; $\color{black} \fcolorbox{yellowgreen}{greenyellow} {O(log(n))}$ | $\color{white} \fcolorbox{limegreen}{forestgreen} {O(1)}$
Breadth-first search | $\color{black} \fcolorbox{gold}{yellow} {Θ(│E│ + │V│)}$ | $\color{black} \fcolorbox{gold}{yellow} {Θ(│V│)}$
Depth-first search | $\color{black} \fcolorbox{gold}{yellow} {Θ(│E│ + │V│)}$ | $\color{black} \fcolorbox{gold}{yellow} {Θ(│V│)}$

[linear-search]: https://en.wikipedia.org/wiki/Linear_search "Wikipedia: Linear search"
[binary-search]: https://en.wikipedia.org/wiki/Binary_search "Wikipedia: Binary search"
[breadth-first-search]: https://en.wikipedia.org/wiki/Breadth-first_search "Wikipedia: Breadth-first search"
[depth-first-search]: https://en.wikipedia.org/wiki/Depth-first_search "Wikipedia: Depth-first search"
