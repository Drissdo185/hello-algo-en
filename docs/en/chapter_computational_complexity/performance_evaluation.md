---
comments: true
---

# Algorithm Efficiency Evaluation

## Evaluation Factors

Before we start learning algorithms, we need to understand the design principles of algorithms, or in other words, how to evaluate the quality of algorithms. In general, we pursue two levels of goals when designing algorithms.

1. **Find a solution**. The algorithm should be able to find a correct solution to the problem under the specified input range.
2. **Find the optimal solution**. There may be multiple solutions to the same problem, and we want the algorithm to be as efficient as possible.

In other words, under the premise of being able to solve the problem, the efficiency of the algorithm is the main evaluation metric, including:

- **Time efficiency**, that is, the speed of the algorithm.
- **Space efficiency**, that is, the size of the memory space occupied by the algorithm.

In data structure and algorithm, we prefer "fast running and small memory usage", but how to evaluate the efficiency of an algorithm is a very important topic, because only knowing how to evaluate an algorithm can we make comparisons and optimizations between algorithms.

## Efficiency Evaluation Methods

### Real-life Testing

Suppose we have algorithm A and algorithm B, both of which can solve the same problem. Now we need to compare the efficiency between the two algorithms. The most direct way we can think of is to use a computer, run both algorithms to their completion, and monitor and record the running time and memory usage. This evaluation method can reflect the real-life situations, but there are also some serious drawbacks.

**It is difficult to exclude the interference factors in the test environment**. The hardware specs can affect the performance of the algorithm. For example, in one computer, algorithm A runs faster than algorithm B; but in another computer with different hardware configuration, the test results may be reversed. This means that we need to test on various machines, which is unrealistic.

**It is extremely resource-consuming to run the complete test**. The efficiency of an algorithm can vary with the size of the input data. For example, algorithm A may run faster than algorithm B when the input data is small, but the test results may be reversed when the input data is large. Therefore, in order to obtain convincing comparison results, we need to test with various data volumes, which requires a lot of computing resources.

### Theoretical Estimation

The real-life testing method has serious drawbacks, so can we estimate the efficiency of an algorithm only by calculations? The answer is yes. We call this estimation method *Complexity Analysis* or *Asymptotic Complexity Analysis*.

**Complexity analysis estimates the trend of the running time and space occupied by the algorithm as the input data volume increases**. In terms of time and space, complexity can be divided into *Time Complexity* and *Space Complexity*.

**Complexity analysis overcomes the shortcomings of the real-life testing method**. Firstly, it is independent of the test environment, and the analysis results are applicable to all platforms. Secondly, it can reflect the efficiency of the algorithm under different data volumes, especially the performance of the algorithm under large data volumes.

## The Importance of Complexity Analysis

Complexity analysis gives us a "ruler" to evaluate the efficiency of algorithms, telling us how much time and space an algorithm needs, and also allows us to make comparisons between different algorithms.

Computational complexity is a mathematical concept, which can be a bit abstract for beginners and is relatively difficult to comprehend. From this point of view, it is not very suitable as a part of the first chapter. However, when we discuss the characteristics of a data structure or algorithm, it is difficult to avoid the need to analyze its running speed and space usage. **Therefore, before learning data structures and algorithms, it is recommended that readers first have a preliminary understanding of computational complexity and be able to complete the complexity analysis of simple cases**.
