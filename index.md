<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio</title>
    <style>
        @font-face {
            font-family: 'Samarkan';
            src: url('fonts/SamarkanNormal-Gg5D.ttf') format('truetype');
            font-weight: normal;
            font-style: normal;
        }

        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }

        dl {
            margin-bottom: 20px;
        }

        .custom-font {
            font-family: 'Samarkan', serif;
            font-size: 1.5em;
        }

        .introduction {
            margin-bottom: 20px;
            text-align: center;
        }

        .introduction h2 {
            font-size: 1.8em;
            margin-bottom: 10px;
        }

        .intro-image {
            display: block;
            width: 70%;
            height: auto;
            margin: 0 auto;
            margin-bottom: 10px;
        }

        .business-cases {
            margin-bottom: 20px;
            text-align: center;
        }

        .business-cases h2 {
            font-size: 1.8em;
            margin-bottom: 10px;
        }

        .case-rectangle {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 200px;
            height: 100px;
            border: 2px solid #000;
            border-radius: 10px;
            margin: 10px;
            text-align: center;
            color: white;
            font-weight: bold;
            padding: 10px 20px;
            box-sizing: border-box;
        }

        .case1 {
            background-color: #f44336;
        }

        .case2 {
            background-color: #2196F3;
        }

        .case3 {
            background-color: #4CAF50;
        }

        .case4 {
            background-color: #FFEB3B;
            color: black;
        }

        .case5 {
            background-color: #9C27B0;
        }

        .case6 {
            background-color: #FF003B;
        }

        .case-description {
            margin-top: 10px;
            padding-left: 20px;
            text-align: center; /* Center align the content */
        }

        .case-description img {
            max-width: 100%; /* Ensure the image doesn't exceed its container width */
        }

        .references {
            margin-bottom: 20px;
        }

        .references h2 {
            font-size: 1.8em;
            margin-bottom: 10px;
        }
    </style>
</head>
<body>
    <dl>
        <dt>Course Name</dt>
        <dd>Algorithmic Problem Solving (APS 2024)</dd>
        <dt>Course Code</dt>
        <dd>23ECSE309</dd>
        <dt>Student Name</dt>
        <dd class="custom-font">Jatin Kalal</dd>
        <dt>University</dt>
        <dd>KLE Technological University, Hubballi-31</dd>
    </dl>

    <div class="introduction">
        <h2>Introduction</h2>
        <img src="https://aeldraconsultancy.in/site/views//assets/images/eCommerce.jpg" alt="Introduction Image" class="intro-image">
        <p>In this work we identify several business cases within the domain of electronic commerce (e-commerce), where transactions of goods and services occur over the internet. E-commerce involves different market segments, involving both businesses and individual sellers. I will delve into specific challenges faced in e-commerce operations and propose algorithmic solutions designed to enhance efficiency.</p>
    </div>

     <div class="business-cases">
        <h2>Identified Business Cases</h2>
        <div class="case-rectangle case1">Delivery Service</div>
        <div class="case-rectangle case2">Order Processing</div>
        <div class="case-rectangle case3">Inv Management</div>
        <div class="case-rectangle case4">Recommendation</div>
        <div class="case-rectangle case5">Item Range Sys</div>
        <div class="case-rectangle case6">Shopping Cart</div>
    </div>


    <div class="case-description">
        <h3>Delivery Service System</h3>
        <img src="https://www.odtap.com/wp-content/uploads/2018/10/doorstep.jpg" alt="Delivery Service Image">
        <p><strong>What it is:</strong> It is about tracking orders which are out for delivery and finding the shortest path to the customer.</p>
        <p><strong>Algorithm Used:</strong> Dijkstra's Algorithm, time complexity O(V^2) using arrays where V is the number of vertices.</p>
        <p><strong>Alternative Algorithm:</strong> A* algorithm, a faster alternative with time complexity O(E), where E is the number of edges.</p>
        <p><strong>Code:</strong> <a href="https://github.com/Jatinkalal/Jatin-Kalal.github.io/blob/main/codes/A*.cpp" class="code">A*</a></p>
        <p><strong>Source:</strong> <a href="https://www.geeksforgeeks.org/a-search-algorithm/">GeeksforGeeks</a></p>
    </div>

    <div class="case-description">
        <h3>Order Processing System</h3>
        <img src="https://www.sweetprocess.com/wp-content/uploads/2023/04/Order_management_system.jpg" alt="Order Processing Image">
        <p><strong>What it is:</strong> It involves keeping track of the incoming orders and its processing.</p>
        <p><strong>Data Structure Used:</strong> Priority Queue (Heap) to maintain incoming orders, time complexity O(log n) for insertions and deletions.</p>
        <p><strong>Alternative Data Structure:</strong> Skip List, although the implementation could be challenging, it offers a time complexity of O(log n).</p>
        <p><strong>Code:</strong> <a href="https://github.com/Jatinkalal/Jatin-Kalal.github.io/blob/main/codes/SkipList.cpp" class="code">Skip List</a></p>
        <p><strong>Source:</strong> <a href="https://www.geeksforgeeks.org/skip-list-set-2-insertion/">GeeksforGeeks</a></p>
    </div>

    <div class="case-description">
        <h3>Inventory Management System</h3>
        <img src="https://jelvix.com/wp-content/uploads/2021/05/7.png" alt="Inventory Management Image">
        <p><strong>What it is:</strong> Inventory management is about keeping track of inventory levels, orders, sales, and deliveries.</p>
        <p><strong>Data Structure Used:</strong> AVL Trees, defined as a self-balancing BST where the difference between heights of left and right subtrees for any node cannot be more than one. It offers a time complexity of O(log n) for all three tree operations.</p>
        <p><strong>Alternative Data Structure:</strong> Red Black Trees are self-balancing, using a simple color-coding scheme to adjust the tree after each modification. It offers a time complexity of O(log n) for all three operations.</p>
        <p><strong>Code:</strong> <a href="https://github.com/Jatinkalal/Jatin-Kalal.github.io/blob/main/codes/RedBlackTree.cpp" class="code">Red Black Tree</a></p>
        <p><strong>Source:</strong> <a href="https://www.geeksforgeeks.org/introduction-to-red-black-tree/">GeeksforGeeks</a></p>
    </div>

    <div class="case-description">
        <h3>Recommendation Service</h3>
        <img src="https://useinsider.com/assets/media/2021/05/recommendation-systems-sm-2.png" alt="Recommendation Service Image">
        <p><strong>What it is:</strong> Recommendation service suggests items based on user preferences and behavior.</p>
        <p><strong>Method/Algorithm Used:</strong> Collaborative Filtering recommends items based on similarity measures between users and/or items.</p>
        <p><strong>Code:</strong> <a href="https://github.com/Jatinkalal/Jatin-Kalal.github.io/blob/main/codes/recommendation.cpp" class="code">Collaborative Filtering</a></p>
        <p><strong>Source:</strong> <a href="https://github.com/bowbowbow/CollaborativeFiltering/blob/master/recommender.cpp">External GitHub Repo</a></p>
    </div>

    <div class="case-description">
        <h3>Item Range System</h3>
        <img src="https://woobewoo.com/wp-content/uploads/2020/07/Price-Range.png" alt="Item Range System Image">
        <p><strong>What it is:</strong> Item range system determines which items to display based on user's preferences and behavior.</p>
        <p><strong>Data Structure Used:</strong> Segment Tree, an advanced data structure that allows querying which of the N segments contain a given value. It offers a time complexity of O(log n) </p>
        <p><strong>Code:</strong> <a href="https://github.com/Jatinkalal/Jatin-Kalal.github.io/blob/main/codes/segment.cpp" class="code">Segment Tree</a></p>
        <p><strong>Source:</strong> <a href="https://www.geeksforgeeks.org/segment-tree-set-1-sum-of-given-range/">GeeksforGeeks</a></p>
    </div>


    <div class="case-description">
        <h3>Shopping Cart Service</h3>
        <img src="https://theecommmanager.com/wp-content/uploads/sites/6/2022/11/what-is-a-shopping-cart-in-ecommerce-featured-image-01-1024x576.png" alt="Shopping cart">
        <p><strong>What it is:</strong> It maintains items which are selected to buy. Add and delete are the major two functions of this service.</p>
        <p><strong>Data Structure Used:</strong> Linked List is a common data strcuture used with time complexity O(n) for addition and deletion</p>
        <p><strong>Code:</strong> <a href="https://github.com/Jatinkalal/Jatin-Kalal.github.io/blob/main/codes/ShopCart.cpp" class="code">Shopping Cart</a></p>
        <p><strong>Source:</strong> <a href="https://stackoverflow.com/questions/18115186/data-structure-to-represent-a-shopping-cart">Stack Overflow</a></p>
    </div>

### Time and Space Complexities

| **Algorithm**                         | **Time Complexity**                            | **Space Complexity**                          |
|---------------------------------------|------------------------------------------------|-----------------------------------------------|
| **Segment Trees**                     | Build: O(n log n), Query/Update: O(log n)      | O(n)                                          |
| **Red-Black Trees**                   | Insert/Delete/Search: O(log n)                 | O(n)                                          |
| **Dijkstra's Algorithm**              | O((V + E) log V)                               | O(V^2)                                        |
| **A_star Search Algorithm**           | O(E)                                           | O(E)                                          |
| **Skip List**                         | Insert/Delete/Search: O(log n)                 | O(n)                                          |

    <div class="references">
        <h2>References</h2>
        <ol>
            <li><a href="https://medium.com/@samarthasthan/building-a-scalable-e-commerce-empire-a-micro-services-system-design-approach-96118bbcef8e" target="_blank">Building a Scalable E-commerce Empire</a></li>
            <li><a href="https://www.geeksforgeeks.org/e-commerce-architecture-system-design-for-e-commerce-website/" target="_blank">System Architecture for E-commerce</a></li>
        </ol>
    </div>

</body>
</html>
