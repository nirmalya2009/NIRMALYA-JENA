<html>
<head>
    <title>Free Fire Profile Visitors</title>
</head>
<body>
    <h1>Free Fire Profile: mehe_run_nisa</h1>
    <input type="text" id="visitorName" placeholder="Enter your name">
    <button onclick="visitProfile()">Visit Profile</button>

    <h2>Visitor Log:</h2>
    <ul id="visitorList"></ul>

    <script>
        function visitProfile() {
            const name = document.getElementById("visitorName").value;
            if (name.trim() !== "") {
                const list = document.getElementById("visitorList");
                const li = document.createElement("li");
                li.textContent = name + " visited.";
                list.appendChild(li);
                document.getElementById("visitorName").value = "";
            }
        }
    </script>
</body>
</html>
