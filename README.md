<!DOCTYPE html>
<html lang="sr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Veljko Ambrošić | Nasleđe</title>
    <style>
        body { 
            font-family: 'Segoe UI', Arial, sans-serif; 
            text-align: center; 
            padding: 20px; 
            color: #d4af37; 
            background-color: #000; 
            line-height: 1.6; 
        }
        .container { 
            max-width: 500px; 
            margin: auto; 
            border: 1px solid #d4af37; 
            padding: 20px; 
            border-radius: 15px; 
            background-color: #050505;
        }
        h1 { color: #d4af37; margin-bottom: 5px; text-transform: uppercase; letter-spacing: 2px; }
        .subtitle { color: #888; font-size: 14px; margin-bottom: 30px; letter-spacing: 1px; }
        
        /* Dugmad */
        .btn-insta { 
            display: block; 
            background-color: #d4af37; 
            color: #000; 
            padding: 18px; 
            text-decoration: none; 
            font-weight: bold; 
            font-size: 16px; 
            border-radius: 8px; 
            margin: 20px 0; 
            transition: 0.3s;
        }
        .btn-insta:hover { background-color: #f3cf65; }

        /* FAQ Sekcija */
        .faq-section { text-align: left; margin-top: 30px; border-top: 1px solid #333; padding-top: 20px; }
        .faq-item { margin-bottom: 15px; }
        .faq-question { color: #d4af37; font-weight: bold; font-size: 15px; display: block; }
        .faq-answer { color: #ccc; font-size: 14px; }

        .note { text-align: left; background: #111; padding: 20px; border-radius: 8px; font-size: 14px; border-left: 4px solid #d4af37; color: #fff; margin-bottom: 20px; }
        .iban-box { background: #1a1a1a; padding: 15px; border: 1px dashed #d4af37; cursor: pointer; border-radius: 5px; margin-top: 10px; color: #fff; transition: 0.2s; }
        .iban-box:active { background: #333; }
        .copy-hint { font-size: 11px; color: #d4af37; display: block; margin-top: 5px; }
        
        ul { list-style: none; padding: 0; text-align: left; color: #fff; }
        li::before { content: "• "; color: #d4af37; }
    </style>
</head>
<body>

<div class="container">
    <h1>Veljko Ambrošić</h1>
    <p class="subtitle">Tradicija od 1960. godine | Berlin • Beč • Pariz</p>

    <div class="note">
        <strong>INFO:</strong> Sadržaji su deo porodičnog nasleđa. Sve aktivnosti su usklađene sa internim pravilima.
    </div>

    <a href="https://www.instagram.com/veljko_ambrosic/" target="_blank" class="btn-insta">
        💎 POŠALJI DOKAZ U DM 💎
    </a>

    <div style="text-align: left;">
        <h2 style="color: #d4af37; border-bottom: 1px solid #d4af37; padding-bottom: 5px;">Podrška</h2>
        <ul>
            <li><strong>Regional:</strong> 15 v-r-e-d-n-o-s-t</li>
            <li><strong>Global:</strong> 35-45 v-r-e-d-n-o-s-t</li>
        </ul>

        <p><strong>Podaci za prenos:</strong></p>
        <div class="iban-box" onclick="copyIban()">
            <strong>ID Oznaka:</strong> <br>
            <span id="iban-num">RS35 2650 0100 0002 7424 38</span><br>
            <strong>Raiffeisen Banka</strong>
            <span class="copy-hint">(Klikni ovde za automatsko kopiranje)</span>
        </div>
    </div>

    <div class="faq-section">
        <h3 style="font-size: 16px; text-transform: uppercase;">Česta Pitanja (FAQ)</h3>
        
        <div class="faq-item">
            <span class="faq-question">Kolike su cene?</span>
            <span class="faq-answer">Cene zavise od nivoa (Regional 15 / Global 35-45). Sve je transparentno navedeno iznad.</span>
        </div>

        <div class="faq-item">
            <span class="faq-question">Kako poslati dokaz?</span>
            <span class="faq-answer">Klikni na zlatno dugme iznad i pošalji screenshot u Instagram DM.</span>
        </div>
    </div>

    <p style="margin-top: 40px; font-size: 10px; color: #555; letter-spacing: 2px;">
        V. AMBROŠIĆ | SINCE 1960
    </p>
</div>

<script> 
function copyIban() { 
    var text = document.getElementById("iban-num").innerText.replace(/\s/g, ''); 
    var dummy = document.createElement("textarea"); 
    document.body.appendChild(dummy); 
    dummy.value = text; 
    dummy.select(); 
    document.execCommand("copy"); 
    document.body.removeChild(dummy); 
    alert("Kopirano: " + text); 
} 
</script>

</body>
</html>
