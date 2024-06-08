<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Staff Time Management</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <h1>Staff Time Management</h1>
        <div id="admin-section">
            <h2>Admin Section</h2>
            <input type="text" id="staffName" placeholder="Staff Name">
            <input type="text" id="staffId" placeholder="Staff ID">
            <button onclick="addStaff()">Add Staff</button>
        </div>
        <div id="manager-section">
            <h2>Manager Section</h2>
            <select id="staffSelect"></select>
            <input type="time" id="startTime">
            <input type="time" id="endTime">
            <button onclick="recordTime()">Record Time</button>
        </div>
        <div id="records-section">
            <h2>Records</h2>
            <ul id="recordsList"></ul>
            <button onclick="exportToExcel()">Export to Excel</button>
        </div>
    </div>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.16.9/xlsx.full.min.js"></script>
    <script src="script.js"></script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    margin: 0;
    padding: 0;
}

.container {
    max-width: 600px;
    margin: auto;
    padding: 20px;
    background: white;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

h1, h2 {
    text-align: center;
}

input, select, button {
    display: block;
    width: 100%;
    padding: 10px;
    margin: 10px 0;
    border-radius: 4px;
    border: 1px solid #ccc;
}

button {
    background-color: #007BFF;
    color: white;
    cursor: pointer;
}

button:hover {
    background-color: #0056b3;
}

#recordsList {
    list-style-type: none;
    padding: 0;
}

#recordsList li {
    background: #e2e2e2;
    margin: 5px 0;
    padding: 10px;
    border-radius: 4px;
}
body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    margin: 0;
    padding: 0;
}

.container {
    max-width: 600px;
    margin: auto;
    padding: 20px;
    background: white;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

h1, h2 {
    text-align: center;
}

input, select, button {
    display: block;
    width: 100%;
    padding: 10px;
    margin: 10px 0;
    border-radius: 4px;
    border: 1px solid #ccc;
}

button {
    background-color: #007BFF;
    color: white;
    cursor: pointer;
}

button:hover {
    background-color: #0056b3;
}

#recordsList {
    list-style-type: none;
    padding: 0;
}

#recordsList li {
    background: #e2e2e2;
    margin: 5px 0;
    padding: 10px;
    border-radius: 4px;
}
