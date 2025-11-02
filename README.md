# javascript1
A responsive webpage layout built with CSS Grid, featuring header, navigation, sidebars, main content, and footer — a clean example of modern web page structuring.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grid Layout</title>
    <style>
        html, body {
            margin: 0;
            padding: 0;
            font-family: sans-serif;
            height: 100vh;
        }

        body {
            display: grid;
            grid-template-areas:
                "header header header"
                "nav nav nav"
                "left main right"
                "footer footer footer";
            grid-template-columns: 1fr 2fr 1fr;
            grid-template-rows: auto auto 1fr auto;
            gap: 2px;
        }

        body > div {
            padding: 20px;
            border: 1px solid #000;
            text-align: center;
        }

        .header {
            grid-area: header;
            background-color: #ff0000;
        }

        .nav {
            grid-area: nav;
            background-color: #3b73c0;
        }

        .left {
            grid-area: left;
            background-color: #ff8000;
        }

        .main {
            grid-area: main;
            background-color: #ffffff;
        }

        .right {
            grid-area: right;
            background-color: #53e020;
        }

        .footer {
            grid-area: footer;
            background-color: #f60303;
        }
    </style>
</head>
<body>
    <div class="header" id="header"><img src="egal.png" alt="Header Image" style="width: 200px;" height="100"></div>
    <div class="nav" id="nav"><a href="#">home</a> | <a href="#">about</a> | <a href="#">contact</a></div>
    <div class="left" id="left"><a href="https://www.example.com">Example Link</a>
    <a href="https://www.example.com">Another Link</a>
<a href="https://www.example.com">Third Link</a></div>
    <div class="main" id="main"><p>I am a web developer with a passion for creating interactive and user-friendly websites.
    I enjoy learning new technologies and improving my skills in web development.
    In my free time, I like to read tech blogs and experiment with new coding techniques.
    I also enjoy collaborating with other developers on open-source projects.
    </p></div>
    <div class="right" id="right">Right</div>
    <div class="footer" id="footer">Footer</div>
</body>
</html>
