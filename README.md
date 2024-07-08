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
        <div class="case-rectangle case1">Order Processing</div>
        <div class="case-rectangle case2">Delivery Service</div>
        <div class="case-rectangle case3">User Searchflow</div>
        <div class="case-rectangle case4">Inv Management</div>
        <div class="case-rectangle case5">Recommendation</div>
    </div>

    <div class="case-description">
        <h3>Order Processing System</h3>
        <p><strong>What it is:</strong> It involves keeping track of the incoming orders and its processing.</p>
        <p><strong>Data Structure Used:</strong> Priority Queue (Heap) to maintain incoming orders, time complexity O(log n) for insertions and deletions.</p>
        <p><strong>Alternative Data Structure:</strong> Skip List, although the implementation could be challenging, it offers a time complexity of O(log n).</p>
        <p><strong>Code:</strong> <a href="/codes/skipList.cpp" class="code">SkipList</a></p>
        <p><strong>Source:</strong> <a href="https://www.example.com">Example Website</a></p>
        <h3>Delivery Service</h3>
        <p>write abt case2.</p>
        <h3>User Searchflow</h3>
        <p>abt case3.</p>
        <h3>Inventory Management</h3>
        <p>abt case4.</p>
        <h3>Notification and Recommendation Service</h3>
        <p>abt case5.</p>
    </div>

    <div class="references">
        <h2>References</h2>
        <ol>
            <li>add kar1</li>
            <li>add kar2</li>
        </ol>
    </div>
</body>
</html>
