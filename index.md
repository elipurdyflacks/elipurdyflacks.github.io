 <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mysterious Video Background</title>
    <style>
        body, html {
            margin: 0;
            padding: 0;
            width: 100%;
            height: 100%;
            overflow: hidden;
            font-family: Arial, sans-serif;
            color: #fff;
        }

        .video-background {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            overflow: hidden;
            z-index: -1;
        }

        .video-background video {
            min-width: 100%;
            min-height: 100%;
            width: auto;
            height: auto;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
        }

        .content {
            position: relative;
            z-index: 1;
            text-align: center;
            padding: 20px;
        }

        h1 {
            margin: 0;
            font-size: 4em;
        }

        p {
            font-size: 1.5em;
        }
    </style>
</head>
<body>
    <div class="video-background">
        <video autoplay loop muted>
            <source src="path/to/your-video.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>
    <div class="content">
        <h1>Mysterious Video Background</h1>
        <p>Welcome to the artsy and mysterious website</p>
    </div>
</body>
</html>