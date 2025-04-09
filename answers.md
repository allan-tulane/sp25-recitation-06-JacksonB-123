# CMPS 2200 Recitation 06
## Answers

**Name:**_____Jackson Burch____________________
**Name:**_________________________


Place all written answers from `recitation-07.md` here for easier grading.



- **2)** Write a recurrence for the work of this algorithm and solve it. Assume the input is $n$ to compute $F_n$.

F_n = (F_n-1) + (F_n-2)

W(n) = W(n-1) + W(n-2) + O(1)

W(n) = O(2^n)

- **3)** Write a recurrence for the span of this algorithm and solve it.

S(n) = S(n-1) + O(1)

S(n) = O(n)

- **4)** Inspecting the counts list, what interesting pattern emerges?

The count list looks like a fibonacci sequence because counts [i] = f(n-i)

- **6)**  When computing $F_n$, what is the maximum number of times that fib_top_down(i) will be called for any value $i$? Based on this, what is the work and span of this algorithm?

the maximum time that fib_top_down(i) will be called for any value is 1 time.

W(n) = O(n)

S(n) = O(n)

fibonacci sequences are sequential because F(n) = (n-1) + f(n-2) with f(n-1 ) being called first, forming a chain of dependencies.

- **8)** When computing $F_n$, what is the maximum number of times that $F_i$ will be read for any value $i$? Based on this, what is the work and span of fib_bottom_up?

When computing $F_n$ the maximum number of times that $F_i$ will be read for any value $i$ is 2 times.

W(n) = O(n)

S(n) = O(n)

for fibonacci sequences each value depends only on the two previous ones and is computed sequentially.
