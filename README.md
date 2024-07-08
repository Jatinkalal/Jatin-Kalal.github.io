
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
        <p>In this work we idenfitfy several business cases within the domain of electronic commerce (e-commerce), where transactions of goods and services occur over the internet. E-commerce involves different market segments, involving both businesses and individual sellers. I will delve into specific challenges faced in e-commerce operations and propose algorithmic solutions designed to enhance efficiency.</p>
    </div>

    <div class="business-cases">
        <h2>Identified Business Cases</h2>
        <div class="case-rectangle case1">Delivery Service</div>
        <div class="case-rectangle case2">Order Processing</div>
        <div class="case-rectangle case3">Inventory Management</div>
        <div class="case-rectangle case4">Recommendation</div>
        <div class="case-rectangle case5">Item Range System</div>
    </div>

    <div class="case-description">
        <h3>Delivery Service</h3>
        <img src="https://www.odtap.com/wp-content/uploads/2018/10/doorstep.jpg" alt="Delivery Service Image">
        <p><strong>What it is:</strong> It is about tracking orders which are out for delivery and finding the shortest path to the customer.</p>
        <p><strong>Algorithm Used:</strong> Dijkstra's Algorithm, time complexity O(V^2) using arrays where V is the number of vertices.</p>
        <p><strong>Alternative Algorithm:</strong> A* algorithm, a faster alternative with time complexity O(E), where E is the number of edges.</p>
        <p><strong>Code:</strong> <a href="https://github.com/Jatinkalal/Jatin-Kalal.github.io/blob/main/codes/A*.cpp" class="code">A*</a></p>
        <p><strong>Source:</strong> <a href="https://www.geeksforgeeks.org/a-search-algorithm/">GeeksforGeeks</a></p>
    </div>

    <div class="references">
        <h2>References</h2>
        <ol>
            <li><a href="https://medium.com/@samarthasthan/building-a-scalable-e-commerce-empire-a-micro-services-system-design-approach-96118bbcef8e" target="_blank">Building a Scalable E-commerce Empire</a></li>
            <li><a href="https://www.geeksforgeeks.org/e-commerce-architecture-system-design-for-e-commerce-website/" target="_blank">System Architecture for E-commerce</a></li>
        </ol>
    </div>

</body>
</html>
