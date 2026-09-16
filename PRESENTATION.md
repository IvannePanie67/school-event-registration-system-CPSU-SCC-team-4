# Final Defense Guide — CPSU EventHub

## Problem
Students need a centralized way to discover campus events and register while organizers need tools for capacity, student records, and registration processing.

## DSA Mapping
| DSA | Implementation | Why selected |
|---|---|---|
| Array | events[], students[], registrations[] | Simple master collections and iteration |
| Queue | queue[] | Registration processing must follow FIFO |
| Stack | history[] | Latest action is accessed first (LIFO) |
| Hash Table | 7 student-ID buckets | Fast average student-ID lookup/indexing |
| Binary Search Tree | Event ID index | Ordered event indexing, search and traversal |

## Algorithms
1. Linear Search — event keyword filtering across event records.
2. Merge Sort — orders events/students without built-in Array.sort().
3. Binary Search — searches sorted Student IDs.
4. Hashing — converts Student ID to a bucket index.
5. BST Search — finds an event ID in the event tree.
6. BST In-order Traversal — returns event IDs in ascending order.

## Demo flow
1. Add an event (CRUD).
2. Add a student in Student Directory.
3. Register the student for an open event.
4. Show the registration entering the FIFO queue.
5. Process the next registration and show it becoming completed.
6. Search a Student ID using Binary Search.
7. Sort events using Merge Sort.
8. Open DSA Lab and explain Queue, Stack, Hash Table, and BST visualizations.
9. Delete an event/student where validation allows it.
10. Export completed registrations to CSV.

## Requirements coverage
- Functional UI: yes
- Add/update/delete/display: yes
- Search and sorting: yes
- DSA-based processing: yes
- Data validation: yes
- Persistent storage: localStorage
- 5 data structures and 6 algorithms: yes
