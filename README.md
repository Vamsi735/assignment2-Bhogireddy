# assignment2-Bhogireddy

# Vamsi Bhogireddy

###### Vijayawada

Vijayawada is famous city which is located near my hometown. It has famous temple which name is **Durgamathalli** Temple. This temple is located beside famous river Krishna. This temple is located on **Indrakeladri Hill**.

---

# Directions from Kansas City to Seattle.
1. Book a cab from Maryville to Kansas airport.
2. Finish the check-in through online.
    1.Take the Boarding pass.
    2.Wait at the gate untill the passengers are allowed to board.
    3.Board the flight.
3. Reach the seattle the explore the city.

---

# Items that should be brought people to Seattle for maximum enjoyment
* Clothes
    * Shoes
    * Jacket
* Cosmetics
    * Facewash
* Wallet
* Snacks
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
    | Pizza         |  Pizza Hub    |  $3   |

    ---

    # Quotes

    > "Don't judge each day by the harvest you reap but by the seeds that you plant." 
    *Robert Louis Stevenson*     <br>
    > "Spread love everywhere you go. Let no one ever come to you without leaving happier." 
    *Mother Teresa*

 -----

## Code Fencing (Graph traversal)
 
 We define a variable minEle that stores the current minimum element in the stack. Now the interesting part is, how to handle the case when minimum element is removed.
 To handle this, we push “2x – minEle” into the stack instead of x so that previous minimum element can be retrieved using current minEle and its value stored in stack.
 
 [Minimum Stack](https://www.geeksforgeeks.org/design-a-stack-that-supports-getmin-in-o1-time-and-o1-extra-space/)
 
 ```
 stack<pair<int, int>> s1, s2;
 if (s1.empty() || s2.empty()) 
    minimum = s1.empty() ? s2.top().second : s1.top().second;
else
    minimum = min(s1.top().second, s2.top().second);
    int minimum = s1.empty() ? new_element : min(new_element, s1.top().second);
s1.push({new_element, minimum});
if (s2.empty()) {
    while (!s1.empty()) {
        int element = s1.top().first;
        s1.pop();
        int minimum = s2.empty() ? element : min(element, s2.top().second);
        s2.push({element, minimum});
    }
}
int remove_element = s2.top().first;
s2.pop();
 
 ```
[Minimum stack / Minimum queue](https://cp-algorithms.com/data_structures/stack_queue_modification.html)
