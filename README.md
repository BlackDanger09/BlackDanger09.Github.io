JO
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Selector de Color</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #f0f0f0;
        }
        #colorBox {
            width: 200px;
            height: 200px;
            background-color: #3498db;
            border: 2px solid #2980b9;
        }
        #colorPicker {
            margin-top: 20px;
        }
    </style>
</head>
<body>

    <div id="colorBox"></div>
    <input type="color" id="colorPicker" value="#3498db">

    <script>
        const colorBox = document.getElementById('colorBox');
        const colorPicker = document.getElementById('colorPicker');

        colorPicker.addEventListener('input', function() {
            colorBox.style.backgroundColor = colorPicker.value;
        });
    </script>

</body>
</html>
