# Remainder-
<!DOCTYPE html>
<html>
<head>
    <title>Birthday Bash!</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            height: 100vh;
            overflow: hidden;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            font-family: Arial, Helvetica, sans-serif;
            background: linear-gradient(120deg, #fbc2eb, #a6c1ee, #fdfbfb, #ffecd2);
            background-size: 400% 400%;
            animation: gradientBG 20s ease infinite;
            color: #222;
        }

        @keyframes gradientBG {
            0% {background-position: 0% 50%;}
            50% {background-position: 100% 50%;}
            100% {background-position: 0% 50%;}
        }

        h1 {
            font-size: 3em;
            margin: 0;
            text-transform: uppercase;
            text-align: center;
            text-shadow: 2px 2px 5px #555;
        }

        p {
            font-size: 1.5em;
            margin-top: 20px;
            text-align: center;
            text-shadow: 1px 1px 3px #555;
        }

        /* Confetti */
        .confetti {
            position: absolute;
            width: 10px;
            height: 10px;
            background-color: white;
            opacity: 0.8;
            top: -10px;
            animation: fall 5s linear infinite;
        }

        @keyframes fall {
            0% { transform: translateY(0) rotate(0deg); }
            100% { transform: translateY(110vh) rotate(360deg); }
        }

        /* Balloons */
        .balloon {
            position: absolute;
            width: 50px;
            height: 70px;
            border-radius: 50% 50% 50% 50%;
            opacity: 0.9;
            bottom: -100px;
            animation: rise 8s infinite ease-in;
        }

        @keyframes rise {
            0% { transform: translateY(0) translateX(0) rotate(0deg); }
            50% { transform: translateY(-50vh) translateX(50px) rotate(10deg); }
            100% { transform: translateY(-110vh) translateX(-50px) rotate(-10deg); }
        }
