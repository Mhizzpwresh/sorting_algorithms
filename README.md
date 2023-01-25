C - Sorting algorithms & Big O

In this project, I implemented twelve different sorting algorithms.



Tests heavy_check_mark

tests: Folder of test files. Provided by Holberton School.

Helper Files raised_hands

print_array.c: C function that prints an array of integers. Provided by Holberton School.

print_list.c: C function that prints a listint_t doubly-linked list. Provided by Holberton School.

Header Files file_folder

sort.h: Header file containing definitions and prototypes for all types and functions written for the project.

Data Structure:



typedef struct listint_s

{

.git/const int n;

.git/struct listint_s *prev;

.git/struct listint_s *next;

} listint_t;

Function Prototypes:



FilePrototype

print_array.cvoid print_array(const int *array, size_t size)

print_list.cvoid print_list(const listint_t *list)

0-bubble_sort.cvoid bubble_sort(int *array, size_t size);

1-insertion_sort_list.cvoid insertion_sort_list(listint_t **list);

2-selection-sort.cvoid selection_sort(int *array, size_t size);

3-quick_sort.cvoid quick_sort(int *array, size_t size);

100-shell_sort.cvoid shell_sort(int *array, size_t size);

101-cocktail_sort_list.cvoid cocktail_sort_list(listint_t **list);

102-counting_sort.cvoid counting_sort(int *array, size_t size);

103-merge_sort.cvoid merge_sort(int *array, size_t size);

104-heap_sort.cvoid heap_sort(int *array, size_t size);

105-radix_sort.cvoid radix_sort(int *array, size_t size);

106-bitonic_sort.cvoid bitonic_sort(int *array, size_t size);

107-quick_sort_hoare.cvoid quick_sort_hoare(int *array, size_t size);

deck.h: Header file containing definitions and prototypes for all types and functions written for the task 1000-sort_deck.c.

Data Structures:



typedef enum kind_e

{

.git/SPADE = 0,

.git/HEART,

.git/CLUB,

.git/DIAMOND

} kind_t;



typedef struct card_s

{

.git/const char *value;

.git/const kind_t kind;

} card_t;



typedef struct deck_node_s

{

.git/const card_t *card;

.git/struct deck_node_s *prev;

.git/struct deck_node_s *next;

} deck_node_t;

Function Prototype:



FilePrototype

1000-deck_node.cvoid sort_deck(deck_node_t **deck);

Tasks page_with_curl

0. Bubble sort



0-bubble_sort.c: C function that sorts an array of integers in ascending order using the Bubble Sort algorithm.

Prints the array after each swap.

0-O: Text file containing the best, average, and worst case time complexities of the Bubble Sort algorithm, one per line.

1. Insertion sort



1-insertion_sort_list.c: C function that sorts a listint_t doubly-linked list of integers in ascending order using the Insertion Sort algorithm.

Prints the list after each swap.

1-O: Text file containing the best, average, and worst case time complexities of the Insertion Sort algorithm, one per line.

2. Selection sort



2-selection_sort.c: C function that sorts an array of integers in ascending order using the Selection Sort algorithm.

Prints the array after each swap.

2-O: Text file containing the best, average, and worst case time complexities of the Selection Sort algorithm, one per line.

3. Quick sort



3-quick_sort.c: C function that sorts an array of integers in ascending order using the Quick Sort algorithm.

Implements the Lomuto partition scheme.

Always uses the last element of the partition being sorted as the pivot.

Prints the array after each swap.

3-O: Text file containing the best, average, and worst case time complexities of the Quick Sort Lomuto Partition scheme algorithm, one per line.

4. Shell sort - Knuth Sequence



100-shell_sort.c: C function that sorts an array of integers in ascending order using the Shell sort algorithm.

Implements the Knuth interval sequence.

Prints the array each time the interval is decreased.

5. Cocktail shaker sort



101-cocktail_sort_list.c: C function that sorts a listint_t doubly-linked list of integers in ascending order using the Cocktail Shaker Sort algorithm.

Prints the list after each swap.

101-O: Text file containing the best, average, and worst case time complexities of the Cocktail Shaker Sort algorithm, one per line.

6. Counting sort



102-counting_sort.c: C function that sorts an array of integers in ascending order using the Counting Sort algorithm.

Assumes that the array will only contain numbers >= 0.

Prints the counting array after it has been initialized.

102-O: Text file containing the best, average, and worst case time complexities of the Counting Sort algorithm, one per line.

7. Merge sort



103-merge_sort.c: C function that sorts an array of integers in ascending order using the Merge Sort algorithm.

Implements the top-down Merge Sort algorithm.

When an array is divided, the size of the left subarray is always less than or equal to the size of the right subarray.

Always sorts the left subarray before the right one.

Prints subarrays each time they are merged.

103-O: Text file containing the best, average, and worst case time complexities of the Merge Sort algorithm, one per line.

8. Heap sort



104-heap_sort.c: C function that sorts an array of integers in ascending order using the Heap Sort algorithm.

Implements the sift-down Heap Sort algorithm.

Prints the array after each swap.

104-O: Text file containing the best, average, and worst case time complexiites of the Heap Sort algorithm, one per line.

9. Radix sort



105-radix_sort.c: C function that sorts an array of integers in ascending order using the Radix Sort algorithm.

Implements the Least-Significant-Digit (LSD) Radix Sort algorithm.

Assumes that the array will only contain numbers >= 0.

Prints the array for each significant digit increase.

105-O: Text file containing the best, average, and worst case time complexities of the Radix Sort algorithm, one per line.

10. Bitonic sort



106-bitonic_sort.c: C function that sorts an array of integers in ascending order using the Bitonic Sort algorithm.

Assumes that size is a power of 2 (ie. size can be expressed as 2^k where k >= 0).

Prints subarrays each time they are merged.

106-O: Text file containing the best, average, and worst case time complexities of the Bitonic Sort algorithm, one per line.

11. Quick Sort - Hoare Partition scheme



107-quick_sort_hoare.c: C function that sorts an array of integers in ascending order using the Quick Sort algorithm.

Implements the Hoare partition scheme.

Always uses the last elemement of the partition being sorted as the pivot.

Prints the array after each swap.

107-O: Text file containing the best, average, and worst case time complexities of the Quick Sort Hoare Partition cheme algorithm, one per line.

12. Dealer



1000-sort_deck.c: C function that sorts a deck_node_t doubly-linked list deck of cards.

Assumes that there are exactly 52 elements in the doubly-linked list.

Orders the deck from spades to diamonds and from aces to kings.
