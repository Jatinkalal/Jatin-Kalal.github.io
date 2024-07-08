<!DOCTYPE html>
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

        .highlighted {
            background-color: yellow;
            font-weight: bold;
        }
    </style>
    <script>
        function highlightWords() {
            var wordsToHighlight = ["E-commerce", "algorithmic", "time complexity", "Dijkstra's Algorithm", "A* algorithm", "Priority Queue", "Heap", "Skip List", "AVL Trees", "Red Black Trees", "Collaborative Filtering", "Segment Trees"];
            wordsToHighlight.forEach(word => {
                var elements = document.getElementsByTagName('*');
                for (var i = 0; i < elements.length; i++) {
                    var element = elements[i];
                    for (var j = 0; j < element.childNodes.length; j++) {
                        var node = element.childNodes[j];
                        if (node.nodeType === 3) {
                            var text = node.nodeValue;
                            var replacedText = text.replace(word, `<span class="highlighted">${word}</span>`);
                            if (replacedText !== text) {
                                element.replaceChild(document.createRange().createContextualFragment(replacedText), node);
                            }
                        }
                    }
                }
            });
        }
    </script>
</head>
<body onload="highlightWords()">
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
        <p>In this work we idenfitfy several business cases within the domain of <span class="highlighted">electronic commerce (e-commerce)</span>, where transactions of goods and services occur over the internet. E-commerce involves different market segments, involving both businesses and individual sellers. I will delve into specific challenges faced in e-commerce operations and propose algorithmic solutions designed to enhance efficiency.</p>
    </div>

    <div class="business-cases">
        <h2>Identified Business Cases</h2>
        <div class="case-rectangle case1">Delivery Service</div>
        <div class="case-rectangle case2">Order Processing</div>
        <div class="case-rectangle case3">Inv Management</div>
        <div class="case-rectangle case4">Recommendation</div>
        <div class="case-rectangle case5">Item Range Sys</div>
    </div>

    <div class="case-description">
        
        <h3>Delivery Service</h3>
        <p><strong>What it is:</strong> It is about tracking orders which are out for delivery and finding a shortest path to the customer.</p>
        <p><strong>Algorithm Used:</strong> <span class="highlighted">Dijkstra's Algorithm</span>, time complexity O(V2) using arrays where V is the number of vertices.</p>
        <p><strong>Alternative Algorithm:</strong> <span class="highlighted">A* algorithm</span> its a faster algorithm than Dijksta's which is now more commonly used with time complexity of O(E), where E is the number of edges.</p>
        <p><strong>Code:</strong> <a href="https://github.com/Jatinkalal/Jatin-Kalal.github.io/blob/main/codes/A*.cpp" class="code">A*</a></p>
        <p><strong>Source:</strong> <a href="https://www.geeksforgeeks.org/a-search-algorithm/">GFG</a></p>
        
        <h3>Order Processing System</h3>
        <p><strong>What it is:</strong> It involves keeping track of the incoming orders and its processing.</p>
        <p><strong>Data Structure Used:</strong> <span class="highlighted">Priority Queue (Heap)</span> to maintain incoming orders, time complexity O(log n) for insertions and deletions.</p>
        <p><strong>Alternative Data Structure:</strong> <span class="highlighted">Skip List</span>, although the implementation could be challenging, it offers a time complexity of O(log n).</p>
        <p><strong>Code:</strong> <a href="https://github.com/Jatinkalal/Jatin-Kalal.github.io/blob/main/codes/SkipList.cpp" class="code">SkipList</a></p>
        <p><strong>Source:</strong> <a href="https://www.geeksforgeeks.org/skip-list-set-2-insertion/">GFG</a></p>

        <h3>Inventory Management System</h3>
        <p><strong> What it is:</strong>Inventory management about keeping track of inventory levels(basically goods), orders, sales and deliveries.</p>
        <p><strong>Data Structure Used:</strong> <span class="highlighted">AVL Trees</span>,defined as a self-balancing BST where the difference between heights of left and right subtrees for any node cannot be more than one. It offers a time complexity of O(log<sub>2</sub>n) for all three tree operations.</p>
        <p><strong>Alternative Data Structure:</strong> <span class="highlighted">Red Black Trees</span> are self-balancing, using a simple color-coding scheme to adjust the tree after each modification. It offers a time complexity of O(logn) for all three operations.</p>
        <p><strong>Code:</strong> <a href="https://github.com/Jatinkalal/Jatin-Kalal.github.io/blob/main/codes/RedBlackTree.cpp" class="code">Red Black Tree</a></p>
        <p><strong>Source:</strong> <a href="https://www.geeksforgeeks.org/introduction-to-red-black-tree/">GFG</a></p>

        <h3>Recommendation Service</h3>
        <p><strong>What it is:</strong> Whenever you search for a book,some e-commerce webistes suggests you similiar books based on your liking, this is what recommendation service is.</p>
        <p><strong>Which method/Algo to be used:</strong> <span class="highlighted">Collaborative Filtering</span> recommends
