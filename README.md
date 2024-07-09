# DSA for E-Commerce Domain

<dl>
<dt>Course Name</dt>
<dd>Algorithmic Problem Solving</dd>
<dt>Course Code</dt>
<dd>23ECSE309</dd>
<dt>Student Name</dt>
<dd>Jatin Kalal</dd>
<dt>University</dt>
<dd>KLE Technological University, Hubballi-31</dd>
</dl>

## Introduction

<div style="display: flex; align-items: center;">
  <img src="https://aeldraconsultancy.in/site/views//assets/images/eCommerce.jpg" alt="E-commerce " style="width: 50%; height: auto; margin-right: 50px; margin-left:50px;"/>
  <p>In this work we identify several business cases within the domain of electronic commerce (e-commerce), where transactions of goods and services occur over the internet. E-commerce involves different market segments, involving both businesses and individual sellers. I will delve into specific challenges faced in e-commerce operations and propose algorithmic solutions designed to enhance efficiency.</p>
</div>

### Functionalities of E-commerce system

- Delivery Service System
- Order Processing System
- Inventory Management System
- Recommendation System
- Item in range filter system
- Shopping cart system

### Objectives

- To identify set of buisness cases/ functionalities for the e-commerce domain
- Provide algorithmic solution to each of the identified buisness cases
- Justify with time and space complexities for the provided solution

### Role of DSA in this?
Data structures play a crucial role in E-commerce systems by enabling efficient retrieval, and management of data. They are fundamental components that help E-commerce platforms perform various tasks such as inventory management, order processing, customer recommendations effectively. 

## Business cases are identified under this domain.
### Delivery Service System
- **What it is:** It is about tracking orders which are out for delivery and finding the shortest path to the customer.
- **Algorithm Used:** Dijkstra's Algorithm, time complexity O(V^2) using arrays where V is the number of vertices.
- **Alternate Algorithm:** A* algorithm, a faster alternative with time complexity O(E), where E is the number of edges.
- [Code for A*](https://github.com/Jatinkalal/Jatin-Kalal.github.io/blob/main/codes/A*.cpp)

### Order Processing System
- **What it is:** It involves keeping track of the incoming orders and its processing.
- **Data Structure Used:** Priority Queue (Heap) to maintain incoming orders, time complexity O(log n) for insertions and deletions.
- **Alternate Data Structure:** Skip List, although the implementation could be challenging, it offers a time complexity of O(log n).
- [Code for SkipList](https://github.com/Jatinkalal/Jatin-Kalal.github.io/blob/main/codes/SkipList.cpp)
  

### Inventory Management System
- **What it is:** Inventory management is about keeping track of inventory levels, orders, sales, and deliveries.
- **Data Structure Used:** AVL Trees, defined as a self-balancing BST where the difference between heights of left and right subtrees for any node cannot be more than one. It offers a time complexity of O(log n) for all three tree operations.
- **Alternate Data Structure:** Red Black Trees are self-balancing, using a simple color-coding scheme to adjust the tree after each modification. It offers a time complexity of O(log n) for all three operations.
- [Code for Red Black Trees](https://github.com/Jatinkalal/Jatin-Kalal.github.io/blob/main/codes/RedBlackTree.cpp)


### Recommendation System
- **What it is:** Recommendation service suggests items based on user preferences and behavior.
- **Algorithm Used:** Collaborative Filtering recommends items based on similarity measures between users and/or items.
- [Code for Collaborative Filtering](https://github.com/Jatinkalal/Jatin-Kalal.github.io/blob/main/codes/recommendation.cpp)

### Item in Range System
- **What it is:** Item range system determines which items to display based on user's preferences and behavior.
- **Data Structure Used:** Segment Tree, an advanced data structure that allows querying which of the N segments contain a given value. It offers a time complexity of O(log n).
- [Code for Segment Tree](https://github.com/Jatinkalal/Jatin-Kalal.github.io/blob/main/codes/segmenTree.cpp)

### Shopping Cart Service
- **What it is:** It maintains items which are selected to buy. Add and delete are the major two functions of this service.
- **Data Structure Used:** Linked List is a common data strcuture used with time complexity O(n) for addition and deletion
- [Code for ShopCart](https://github.com/Jatinkalal/Jatin-Kalal.github.io/blob/main/codes/ShopCart.cpp)

### Location Based Item Suggestion
- **What it is:** It suggests/recommends items based on local region of the user.
- **Algorithm Used:** Geographical Based Location. Time complexity O(n) for generating recomendation and O(1) for updating
- [External Code](https://github.com/shakasom/location-based-recommendations)

### Customer Information Storage
- **What it is:** It stores customer information.
- **Data Structure Used:** Linked List, with Time complexity O(n) for addition and deletion at a given position x.
- [External Code](https://github.com/HozefaRauf/DSA-project-Online-Ecommerce-Store/blob/main/project.cpp)

### Optimize discount distribution for different cities
- **What it is:** The reason for using this is that we want to give discount to user and previous distance is not used.
- **Algorithm Used:** Prim's algorithm can be used to find the minimum spanning tree of a graph. So, it provides the distances between areas in a city. The edges included in the MST represent the optimal paths where discounts should be applied. By following these paths, the e-commerce platform can distribute discounts in a manner that minimizes the overall cost while still reaching all relevant areas.
- [External Code](https://github.com/HozefaRauf/DSA-project-Online-Ecommerce-Store/blob/main/project.cpp)

### Dynamic price service
- **What it is:** Dynamic price of items during festivals/sales.
- **Algorithm Used:** Segment Tree with lazy propogation
- [External Code](https://github.com/vivek1011/Segment-tree-lazy-propagation-)

### Time and Space Complexities

| **Algorithm**                         | **Time Complexity**                            | **Space Complexity**                          |
|---------------------------------------|------------------------------------------------|-----------------------------------------------|
| **Segment Trees**                     | Build: O(n log n), Query/Update: O(log n)      | O(n)                                          |
| **Red-Black Trees**                   | Insert/Delete/Search: O(log n)                 | O(n)                                          |
| **Dijkstra's Algorithm**              | O((V + E) log V)                               | O(V^2)                                        |
| **A_star Search Algorithm**           | O(E)                                           | O(E)                                          |
| **Skip List**                         | Insert/Delete/Search: O(log n)                 | O(n)                                          |
| **Linked List**                       | Insert/Delete: O(n)                            | O(n)                                          |
| **Prim's Algorithm**                  | Using adj List: O(VlogV + ElogV) = O(ElogV)    | O(V+E)                                        |

## References
1. Pugh, W., 1990. Skip lists: a probabilistic alternative to balanced trees. Communications of the ACM, 33(6), pp.668-676.
2. GeeksforGeeks (GFG) 'System Architecture for E-commerce'. Available at: https://www.geeksforgeeks.org/e-commerce-architecture-system-design-for-e-commerce-website/
3. Medium 'Building scalable E-commerce empire'. Available at: https://medium.com/@samarthasthan/building-a-scalable-e-commerce-empire-a-micro-services-system-design-approach-96118bbcef8e







