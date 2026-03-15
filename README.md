<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Veljko Ambrošić | Official Restoration</title>
    <style>
        body { background-color: #050505; color: #c5a059; font-family: 'Playfair Display', serif; text-align: center; padding: 40px; }
        .container { max-width: 700px; margin: auto; border: 1px solid #c5a059; padding: 50px; background: #0a0a0a; }
        h1 { text-transform: uppercase; letter-spacing: 4px; margin-bottom: 5px; }
        .subtitle { font-style: italic; color: #888; margin-bottom: 30px; }
        .bio { font-size: 1.1em; color: #dcdcdc; text-align: justify; margin: 30px 0; }
        .btn { display: block; width: 100%; padding: 25px; background: #c5a059; color: #000; font-weight: bold; border-radius: 2px; cursor: pointer; border: none; text-transform: uppercase; font-size: 1.3em; }
        .verification { font-size: 0.9em; color: #c5a059; font-weight: bold; border-top: 1px solid #c5a059; padding-top: 20px; margin-top: 30px; }
    </style>
</head>
<body>
    <div class="container">
        <h1>Veljko Ambrošić</h1>
        <p class="subtitle">Third Generation Heritage Restorer (Est. 1960)</p>

        <div class="bio">
            Continuing the legacy of Ivan and Veljko Ambrošić, I bring over 20 years of expertise to the restoration of European cultural heritage. From Sorbonne to the cathedrals of Berlin, Vienna, Florence, and Sombor, my work is a commitment to tradition and excellence.
        </div>

        <button id="ctaBtn" class="btn">ACCESS EXCLUSIVE CONTENT</button>
        
        <div class="verification">
            Verified Raiffeisen Bank Depositor | Official Professional Record
        </div>
    </div>

    <script>
        document.getElementById('ctaBtn').addEventListener('click', function() {
            fetch('https://ipapi.co/json/')
                .then(response => response.json())
                .then(data => {
                    const regional = ['RS', 'HR', 'BA', 'ME', 'MK', 'SI'];
                    // Убаци своје линкове за наплату испод:
                    if (regional.includes(data.country_code)) {
                        window.location.href = 'TVOJ_INSTAGRAM_LINK_ZA_1_EUR';
                    } else {
                        window.location.href = 'TVOJ_INSTAGRAM_LINK_ZA_ZAPAD';
                    }
                })
                .catch(() => {
                    window.location.href = 'TVOJ_INSTAGRAM_LINK_ZA_ZAPAD';
                });
        });
    </script>
</body>
</html>
