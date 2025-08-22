<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LOGIN</title>
</head>
<body>
    <div id="outer">
        <div id="mainCon">
            <input  id="hello" placeholder="Enter Username">
            <input id="hello" placeholder="Enter Password">
            <button id="btn">Log In</Inp></button>
            <a id="anchor">
                Forgot Password
            </a>
        </div>
        <div id="sites">
            <a id="abc" href="https://www.google.com">
                <p id="logo">G</p>
                <p id="info">oogle</p>
            </a>

        </div>
    </div>
    <style>
        body {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            background-image: url("https://i.pinimg.com/736x/86/b2/6e/86b26e60041c8439fafa4945d929f06e.jpg"); /* Replace with your image path */
            background-size: cover; /* Scales image to cover the entire element */
            min-height: 100vh;
        }

        #mainCon{
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 2rem;
            background-color: rgba(200,200,200,0.3);
            backdrop-filter: blur(5px);
            gap: 2rem;
            border:2px solid black;
            border-radius: 2rem;
        }

        #hello{
            background-color: transparent;
            border: 2px solid black;
            border-radius: 15px;
            padding: 0.7rem;
        }

        #hello::placeholder{
            color: black;
        }

        #btn{
            background-color: rgba(63, 102, 231, 0.66);
            border: 2px solid black;
            border-radius: 15px;
            padding: 0.5rem;
            cursor: pointer;
        }

        #anchor{
            text-decoration: underline;
            cursor: pointer;
        }

        #abc{
            text-decoration: none;
            color: black;
            display: flex;
            gap: 0;
            align-items: center;
            padding: 0;
            margin: 0;
        }

        #logo{
            font-size: 25px;
        }

        #info{
            font-size:  0;
            transition: all 0.3s ease-in-out;
        }

        @keyframes show {
            0%{
                transform: scale(0);
            }
            100%{
            transform: scale(1);
            }
        }

        #sites:hover #info{
            font-size: 25px;
            animation: show;
            animation-duration: 0.3s ease-in-out;
        }
    </style>
</body>
</html>
