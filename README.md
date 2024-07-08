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
            font-size: 1.5em; /* Adjusted font size */
        }

        .introduction {
            margin-bottom: 20px;
            text-align: center; /* Centering the introduction section */
        }

        .introduction h2 {
            font-size: 1.8em;
            margin-bottom: 10px;
        }

        .intro-image {
            display: block;
            width: 70%; /* Increased size */
            height: auto;
            margin: 0 auto; /* Centering the image */
            margin-bottom: 10px;
        }

        .business-cases {
            margin-bottom: 20px;
            text-align: center; /* Centering the business cases */
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
            padding: 10px 20px; /* Adjusted padding to fit text */
            box-sizing: border-box; /* Ensure padding is included in the dimensions */
        }

        .case1 {
            background-color: #f44336; /* Red */
        }

        .case2 {
            background-color: #2196F3; /* Blue */
        }

        .case3 {
            background-color: #4CAF50; /* Green */
        }

        .case4 {
            background-color: #FFEB3B; /* Yellow */
            color: black;
        }

        .case5 {
            background-color: #9C27B0; /* Purple */
        }

        .case-description {
            margin-top: 10px;
            padding-left: 20px;
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
        <p>In this work we idenfitfy several business cases within the domain of electronic commerce (e-commerce), where transactions of goods and services occur over the internet. E-commerce involves different market segments, involving both businesses and individual sellers. I will delve into specific challenges faced in e-commerce operations and propose algorithmic solutions designed to enhance efficiency.</p>
    </div>

    <div class="business-cases">
        <h2>Identified Business Cases</h2>
        <div class="case-rectangle case1">Delivery Service</div>
        <div class="case-rectangle case2">Order Processing</div>
        <div class="case-rectangle case3">Inv Management</div>
        <div class="case-rectangle case4">Recommendation</div>
        <div class="case-rectangle case5">Recommendation</div>
    </div>

    <div class="case-description">
        
        <h3>Delivery Service</h3>
        <p><strong>What it is:</strong> It is about tracking orders which are out for delivery and finding a shortest path to the customer.</p>
        <p><strong>Algorithm Used:</strong> Dijkstra's Algorithm, time complexity O(V2) using arrays where V is the number of vertices.</p>
        <p><strong>Alternative Algorithm:</strong> A* algorithm its a faster algorithm than Dijksta's which is now more commonly used with time complexity of O(E), where E is the number of edges.</p>
        <p><strong>Code:</strong> <a href="https://github.com/Jatinkalal/Jatin-Kalal.github.io/blob/main/codes/A*.cpp" class="code">A*</a></p>
        <p><strong>Source:</strong> <a href="https://www.geeksforgeeks.org/a-search-algorithm/">GFG</a></p>
        
        <h3>Order Processing System</h3>
        <p><strong>What it is:</strong> It involves keeping track of the incoming orders and its processing.</p>
        <p><strong>Data Structure Used:</strong> Priority Queue (Heap) to maintain incoming orders, time complexity O(log n) for insertions and deletions.</p>
        <p><strong>Alternative Data Structure:</strong> Skip List, although the implementation could be challenging, it offers a time complexity of O(log n).</p>
        <p><strong>Code:</strong> <a href="https://github.com/Jatinkalal/Jatin-Kalal.github.io/blob/main/codes/SkipList.cpp" class="code">SkipList</a></p>
        <p><strong>Source:</strong> <a href="https://www.geeksforgeeks.org/skip-list-set-2-insertion/">GFG</a></p>

        <h3>Inventory Management System</h3>
        <p><strong> What it is:</strong>Inventory management about keeping track of inventory levels(basically goods), orders, sales and deliveries.</p>
        <p><strong>Data Structure Used:</strong> AVL Trees,defined as a self-balancing BST where the difference between heights of left and right subtrees for any node cannot be more than one. It offers a time complexity of O(log<sub>2</sub>n) for all three tree operations.</p>
        <p><strong>Alternative Data Structure:</strong> Red Black Trees are self-balancing, using a simple color-coding scheme to adjust the tree after each modification. It offers a time complexity of O(logn) for all three operations.</p>
        <p><strong>Code:</strong> <a href="https://github.com/Jatinkalal/Jatin-Kalal.github.io/blob/main/codes/RedBlackTree.cpp" class="code">Red Black Tree</a></p>
        <p><strong>Source:</strong> <a href="https://www.geeksforgeeks.org/introduction-to-red-black-tree/">GFG</a></p>

        <h3>Recommendation Service</h3>
        <p><strong>What it is:</strong> Whenever you search for a book,some e-commerce webistes suggests you similiar books based on your liking, this is what recommendation service is.</p>
        <p><strong>Which method/Algo to be used:</strong> Collaborative Filtering recommends items based on similarity measures between users and/or items. The basic assumption behind the algorithm is that users with similar interests have common preferences.</p>
        <p><strong>Code:</strong> <a href="https://github.com/Jatinkalal/Jatin-Kalal.github.io/blob/main/codes/recommendation.cpp" class="code">Collaborative Filtering</a></p>
        <p><strong>Source:</strong> <a href="https://github.com/bowbowbow/CollaborativeFiltering/blob/master/recommender.cpp">External Github Repo</a></p>

         <h3>Recommendation Service</h3>
        <p><strong>What it is:</strong> Whenever you search for a book,some e-commerce webistes suggests you similiar books based on your liking, this is what recommendation service is.</p>
        <p><strong>Which method/Algo to be used:</strong> Collaborative Filtering recommends items based on similarity measures between users and/or items. The basic assumption behind the algorithm is that users with similar interests have common preferences.</p>
        <p><strong>Code:</strong> <a href="https://github.com/Jatinkalal/Jatin-Kalal.github.io/blob/main/codes/recommendation.cpp" class="code">Collaborative Filtering</a></p>
        <p><strong>Source:</strong> <a href="https://github.com/bowbowbow/CollaborativeFiltering/blob/master/recommender.cpp">External Github Repo</a></p>

        
    </div>

    <div class="references">
    <h2>References</h2>
    <ol>
        <li><a href="https://medium.com/@samarthasthan/building-a-scalable-e-commerce-empire-a-micro-services-system-design-approach-96118bbcef8e" target="_blank">Building a Scalable E-commerce Empire</a></li>
        <li><a href="https://www.geeksforgeeks.org/e-commerce-architecture-system-design-for-e-commerce-website/" target="_blank">System Architecuture for E-commerce</a></li>
        
    </ol>
    
</div>

</body>
</html>
