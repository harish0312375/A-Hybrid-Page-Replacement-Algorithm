```markdown
# A Novel Hybrid Page Replacement Algorithm

## Introduction
This project implements a novel hybrid page replacement algorithm, which combines FIFO (First-In-First-Out), LRU (Least Recently Used), and LFU (Least Frequently Used) page replacement strategies to optimize memory management. The project compares the performance of the hybrid approach with traditional algorithms based on page hit and fault metrics.

## Implementation Details
The implementation simulates a memory of three frames and generates a random page reference string of 100 pages ranging from 0 to 9. The program evaluates different page replacement algorithms and calculates the average number of hits and faults for each approach.

### Page Replacement Algorithms Implemented
1. **FIFO (First-In-First-Out)**
   - Replaces the oldest page in memory when a new page is requested and memory is full.
2. **LRU (Least Recently Used)**
   - Replaces the page that has not been used for the longest time.
3. **LFU (Least Frequently Used)**
   - Replaces the page with the lowest usage count.
4. **Hybrid Algorithm**
   - Cycles through FIFO, LRU, and LFU dynamically to improve performance.

## Code Explanation
1. **Generate Random Pages**: A function generates a sequence of 100 random page requests.
2. **FIFO Implementation**: Keeps track of page hits and faults using a queue-based approach.
3. **LRU Implementation**: Tracks recently used pages and replaces the least recently used one.
4. **LFU Implementation**: Maintains a frequency counter to replace the least frequently used page.
5. **Hybrid Implementation**: Cycles between FIFO, LRU, and LFU algorithms to balance performance.
6. **Simulation Execution**:
   - Runs each algorithm 100 times and records results.
   - Computes the average number of page hits and faults for comparison.

## Results
### Sample Output 1:
```
Average Hits FIFO: 29.81
Average Faults FIFO: 70.19
Average Hits LRU: 29.49
Average Faults LRU: 70.51
Average Hits LFU: 29.49
Average Faults LFU: 70.51
Average Hits Hybrid: 29.49
Average Faults Hybrid: 70.51
```
### Sample Output 2:
```
Average Hits FIFO: 29.3
Average Faults FIFO: 70.7
Average Hits LRU: 29.3
Average Faults LRU: 70.7
Average Hits LFU: 29.3
Average Faults LFU: 70.7
Average Hits Hybrid: 29.34
Average Faults Hybrid: 70.66
```

## References
1. T. Ma, Y. Hao, Y. Tian, M. Al-Rodhaan, "An improved web cache replacement algorithm based on weighting and cost," IEEE Access, vol 6, 2021.
2. W. Ali, S. Mariyam Shamsuddin, A. Samad Ismail, "A survey of web caching and Prefetching," Int. J. Advance. Soft Comput. Appl., 3(1), ISSN 2074–8523; ICSRS Publication, 2022.
3. D. Singh, S. Kumar, S. Kapoor, "An explore view of Web caching techniques," Int. J. Adv. Eng. Sci., 1(3), 38–43 (2021).

## Conclusion
This project presents a comparative analysis of FIFO, LRU, LFU, and a hybrid page replacement algorithm. The hybrid method balances performance by leveraging different strategies dynamically. Future improvements may include adapting the hybrid approach to real-world workloads and optimizing it further for modern memory systems.

## Thank You
```

