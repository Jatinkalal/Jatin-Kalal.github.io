
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
        }

        .introduction h2 {
            font-size: 1.8em;
            margin-bottom: 10px;
        }

        .intro-image {
            display: block;
            width: 50%;
            height: auto;
            margin-right: 50px;
            margin-left: 50px;
            margin-bottom: 10px;
        }

        .business-cases {
            margin-bottom: 20px;
        }

        .business-cases h2 {
            font-size: 1.8em;
            margin-bottom: 10px;
        }

        .case-circle {
            display: inline-block;
            width: 100px;
            height: 100px;
            border: 2px solid #000;
            border-radius: 50%;
            margin-right: 10px;
            text-align: center;
            line-height: 100px;
            color: white;
            font-weight: bold;
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
        <p>Intro still on the way.</p>
    </div>

    <div class="business-cases">
        <h2>Identified Business Cases</h2>
        <div class="case-circle case1">Order Processing System</div>
        <div class="case-circle case2">Delivery Service</div>
        <div class="case-circle case3">User Searchflow</div>
        <div class="case-circle case4">Inventory Management</div>
        <div class="case-circle case5">Notification and Recommendation</div>
    </div>

    <div class="case-description">
        <h3>Case 1</h3>
        <p>likh case1.</p>
        <h3>Case 2</h3>
        <p>write abt case2.</p>
        <h3>Case 3</h3>
        <p>abt case3.</p>
        <h3>Case 4</h3>
        <p>abt case4.</p>
        <h3>Case 5</h3>
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

