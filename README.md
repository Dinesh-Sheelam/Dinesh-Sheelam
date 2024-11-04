<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Name - Portfolio</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/particles.js/2.0.0/particles.min.js"></script>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
        }

        body {
            background: #ffeee6;
            color: #2d3436;
            min-height: 100vh;
            overflow-x: hidden;
        }

        #particles-js {
            position: absolute;
            width: 100%;
            height: 100%;
            z-index: 1;
        }

        nav {
            position: fixed;
            top: 0;
            width: 100%;
            padding: 1.5rem;
            display: flex;
            justify-content: center;
            gap: 2rem;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(5px);
            z-index: 10;
        }

        nav a {
            color: #2d3436;
            text-decoration: none;
            font-size: 1.1rem;
            transition: color 0.3s ease;
        }

        nav a:hover {
            color: #ff6b6b;
        }

        .content {
            position: relative;
            z-index: 2;
            padding: 0 2rem;
            margin-top: 40vh;
            text-align: left;
            max-width: 1200px;
            margin-left: auto;
            margin-right: auto;
        }

        .intro {
            font-size: 3rem;
            font-weight: bold;
            margin-bottom: 1rem;
        }

        .intro span {
            color: #ff6b6b;
        }

        .title {
            font-size: 1.5rem;
            color: #636e72;
        }

        @media (max-width: 768px) {
            .intro {
                font-size: 2rem;
            }
            .title {
                font-size: 1.2rem;
            }
        }
    </style>
</head>
<body>
    <div id="particles-js"></div>
    
    <nav>
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#expertise">Expertise</a>
        <a href="#portfolio">Portfolio</a>
        <a href="#contact">Contact</a>
        <a href="#resume">Resume</a>
    </nav>

    <main class="content">
        <h1 class="intro">I am <span>Your Name</span></h1>
        <h2 class="title">Your Title</h2>
    </main>

    <script>
        particlesJS('particles-js',
            {
                "particles": {
                    "number": {
                        "value": 80,
                        "density": {
                            "enable": true,
                            "value_area": 800
                        }
                    },
                    "color": {
                        "value": "#ff6b6b"
                    },
                    "shape": {
                        "type": "circle"
                    },
                    "opacity": {
                        "value": 0.5,
                        "random": false
                    },
                    "size": {
                        "value": 3,
                        "random": true
                    },
                    "line_linked": {
                        "enable": true,
                        "distance": 150,
                        "color": "#ff6b6b",
                        "opacity": 0.2,
                        "width": 1
                    },
                    "move": {
                        "enable": true,
                        "speed": 2,
                        "direction": "none",
                        "random": false,
                        "straight": false,
                        "out_mode": "out",
                        "bounce": false
                    }
                },
                "interactivity": {
                    "detect_on": "canvas",
                    "events": {
                        "onhover": {
                            "enable": true,
                            "mode": "grab"
                        },
                        "onclick": {
                            "enable": true,
                            "mode": "push"
                        },
                        "resize": true
                    }
                },
                "retina_detect": true
            }
        );
    </script>
</body>
</html>
