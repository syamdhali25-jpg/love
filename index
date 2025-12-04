<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Animated Heart</title>
    
    <style>
        /* General body styling to center content and set background */
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            background-color: #000; /* Use black background like the video */
            overflow: hidden; /* Hide anything that goes off screen */
        }

        /* The classes from the video snippet go here */
        .ui .love_word {
            color: #ea80b0; /* Pink color */
            font-size: 1.4rem;
            /* The following transform line is what creates the rotating/translated position */
            transform: translateY(-100%) rotateZ(-30deg);
            text-shadow: 0 0 10px #ffff; 
            letter-spacing: 2px;
            white-space: nowrap;
        }

        .ui .love_horizontal {
            animation: horizontal 10000ms infinite alternate ease-in-out;
            animation-delay: calc(var(--i) * -300ms); /* Uses a custom property '--i' for stagger */
        }
        
        /* The full animation is not in the clip, but here is a sample to make it move */
        @keyframes horizontal {
            0% { transform: translateX(-100px); }
            50% { transform: translateX(100px); }
            100% { transform: translateX(-100px); }
        }
        
        /* You would need many of these elements to form the heart shape */
        .heart-container {
            position: relative;
            width: 300px;
            height: 300px;
            transform-style: preserve-3d;
            animation: pulse 4s infinite; /* Add a pulse effect to the whole heart */
        }

        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.05); }
        }

    </style>
</head>
<body>
    
    <div class="heart-container">
        <div class="ui love_word love_horizontal" style="--i:1;">I love you</div>
        <div class="ui love_word love_horizontal" style="--i:2;">I love you</div>
        <div class="ui love_word love_horizontal" style="--i:3;">I love you</div>
        </div>
    
</body>
</html>
