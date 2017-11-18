# Christofides algorithm

The **Christofides algorithm** is an algorithm for finding approximate solutions to the travelling salesman problem, on instances where the distances form a metric space(they are symmetric and obey the triangle inequality).
It is an approximation algorithm that guarantees that its solutions will be within a factor of 3/2 of the optimal solution length, and is named after Nicos Christofides, who published it in 1976.  As of 2017, this is the best approximation ratio that has been proven for the traveling salesman problem on general metric spaces, although better approximations are known for some special cases [Wikipedia](https://en.wikipedia.org/wiki/Christofides_algorithm)



**Basic steps of algorithm:**

1. Find a minimum spanning tree **(T)**
2. Find vertexes in **T** with odd degree **(O)**
3. Find minimum weight matching **(M)** edges to **T**
4. Build an Eulerian circuit using the edges of **M** and **T**
5. Make a Hamiltonian circuit by skipping repeated vertexes




## Python implementation

In the file **christofides.py** there is an implementation of algorithm with comments and several test inputs.

You can simply use this code by calling the tsp() function with an array of point(with its coordinates x, y)

**Example:**

```python
# array of points
points = [
    [0, 0], [3, 0], [6, 0],
    [0, 3], [3, 3], [6, 3],
  	[0, 6], [3, 6], [6, 6]
]

length, path = tsp(points)

```



If you have some questions or advices, please give me know

## Authors

* **Andrew Zhuravchak** - student of CS@UCU