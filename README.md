# assignment2-Bhogireddy

# Vamsi Bhogireddy

###### Vijayawada

Vijayawada is famous city which is located near my hometown. It has famous temple which name is **Durgamathalli** Temple. This temple is located beside famous river Krishna. This temple is located on **Indrakeladri Hill**.

---

# Directions from Kansas City to Seatle.
1. Book a cab from Maryville to Kansas airport.
2. Finish the check-in through online.
    1.Take the Boarding pass.
    2.Wait at the gate untill the passengers are allowed to board.
    3.Board the flight.
3. Reach the seattle the explore the city.


* Clothes
    * Shoes
    * Jacket
* Cosmetics
    * Facewash
* Wallet
* Snakes
    * Chocolates
    * Milk shake

    [AboutMe](https://github.com/Vamsi735/assignment2-Bhogireddy/blob/main/AboutMe.md)


    ---

    # Table Creation 

    A table with three columns recommends the some of the best foods that i experienced in India.

    | Food/Drink    |   Location    | Price |
    |   ---         |   ---         |  ---  |
    | Mixed Biryani |   Falcons     |  $4   |
    | Chicken Pizza |   PizzaHut    |  $3   |
    | Burger        |   Subway      |  $2   |

    ---

    # Quotes

    > "Don't judge each day by the harvest you reap but by the seeds that you plant." 
    *Robert Louis Stevenson*     <br>
    > "Spread love everywhere you go. Let no one ever come to you without leaving happier." 
    *Mother Teresa*

 -----

## Code Fencing (Graph traversal)
In computer science, graph traversal (also known as graph search) refers to the process of visiting (checking and/or updating) each vertex in a graph. Such traversals are classified by the order in which the vertices are visited. Tree traversal is a special case of graph traversal.<https://en.wikipedia.org/wiki/Graph_traversal>

---

## Code Fencing (Graph traversal)
In computer science, graph traversal (also known as graph search) refers to the process of visiting (checking and/or updating) each vertex in a graph. Such traversals are classified by the order in which the vertices are visited. Tree traversal is a special case of graph traversal.<https://en.wikipedia.org/wiki/Graph_traversal>

```
vector<vector<int>> adj;  // adjacency list representation
int n; // number of nodes
int s; // source vertex

queue<int> q;
vector<bool> used(n);
vector<int> d(n), p(n);

q.push(s);
used[s] = true;
p[s] = -1;
while (!q.empty()) {
    int v = q.front();
    q.pop();
    for (int u : adj[v]) {
        if (!used[u]) {
            used[u] = true;
            q.push(u);
            d[u] = d[v] + 1;
            p[u] = v;
        }
    }
}
```
<https://cp-algorithms.com/graph/breadth-first-search.html>