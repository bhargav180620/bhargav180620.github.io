# Will You Go Out With Me?

This is a simple page I created. You can view it live at [My GitHub Page](https://bhargav180620.github.io/repositoryname/).

Alternatively, you can also check out the HTML code below.


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Will You Go Out With Me?</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-image: url('https://source.unsplash.com/11600x900/?nature');
            background-size: cover;
            background-position: center;
            font-family: 'Courier New', Courier, monospace;
            color: #fff;
            text-shadow: 2px 2px 4px #000;
        }
        .container {
            text-align: center;
            background: rgba(0, 0, 0, 0.5);
            padding: 20px;
            border-radius: 10px;
        }
        .button {
            padding: 10px 20px;
            margin: 10px;
            font-size: 16px;
            cursor: pointer;
            border: none;
            border-radius: 5px;
            transition: background-color 0.3s;
        }
        #yes {
            background-color: #ff69b4;
            color: #fff;
        }
        #yes:hover {
            background-color: #ff1493;
        }
        #no {
            background-color: #ff6347;
            color: #fff;
            position: absolute;
        }
        #no:hover {
            background-color: #ff4500;
        }
    </style>
</head>

<body>
    <div class="container">
        <h1>Will You Go Out With Me?</h1>
        <button class="button" id="yes">Yes</button>
        <button class="button" id="no">No</button>
    </div>
    <script>
        const noButton = document.getElementById('no');
        noButton.addEventListener('mouseover', () => {
            const x = Math.random() * (window.innerWidth - noButton.offsetWidth);
            const y = Math.random() * (window.innerHeight - noButton.offsetHeight);
            noButton.style.left = `${x}px`;
            noButton.style.top = `${y}px`;
        });
    </script>
</body>
</html>
