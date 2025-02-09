<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Be My Valentine?</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #ffcccb;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            flex-direction: column;
        }
        h1 {
            color: #d63384;
        }
        .buttons {
            margin-top: 20px;
        }
        button {
            font-size: 20px;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            transition: 0.3s;
        }
        .yes {
            background-color: #28a745;
            color: white;
        }
        .no {
            background-color: #dc3545;
            color: white;
            position: absolute;
        }
    </style>
</head>
<body>
    <h1>Will you be my Valentine? ❤️</h1>
    <div class="buttons">
        <button class="yes" onclick="alert('Yay! ❤️')">Yes</button>
        <button class="no" onmouseover="moveButton()">No</button>
    </div>
    <script>
        function moveButton() {
            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 50);
            document.querySelector('.no').style.left = `${x}px`;
            document.querySelector('.no').style.top = `${y}px`;
        }
    </script>
</body>
</html>
