<!DOCTYPE html>
<html lang="sr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Veljko Ambrošić | Nasleđe</title>
    <style>
        body { font-family: 'Segoe UI', Arial, sans-serif; text-align: center; padding: 20px; color: #d4af37; background-color: #000; line-height: 1.6; }
        .container { max-width: 500px; margin: auto; border: 1px solid #d4af37; padding: 20px; border-radius: 15px; }
        h1 { color: #d4af37; margin-bottom: 5px; text-transform: uppercase; }
        .subtitle { color: #888; font-size: 14px; margin-bottom: 30px; letter-spacing: 1px; }
        .btn-insta { display: block; background-color: #d4af37; color: #000; padding: 18px; text-decoration: none; font-weight: bold; font-size: 16px; border-radius: 8px; margin: 25px 0; }
        .note { text-align: left; background: #111; padding: 20px; border-radius: 8px; font-size: 14px; border-left: 4px solid #d4af37; color: #fff; }
        .iban-box { background: #1a1a1a; padding: 15px; border: 1px dashed #d4af37; cursor: pointer; border-radius: 5px; margin-top: 10px; color: #fff; }
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
        <h2 style="color: #d4af37; border-bottom: 1px solid #d4af37;">Detalji</h2>
        <p><strong>Nivoi podrške:</strong></p>
        <ul>
            <li>Regional: 15 (v-r-e-d-n-o-s-t)</li>
            <li>Global: 35-45 (v-r-e-d-n-o-s-t)</li>
        </ul>

        <p><strong>Podaci:</strong></p>
        <div class="iban-box" onclick="copyIban()">
            <strong>ID Oznaka:</strong> <br>
            <span id="iban-num">RS35 2650 0100 0002 7424 38</span><br>
            <strong>R. B-a-n-k-a</strong>
            <span class="copy-hint">(Klikni ovde za automatsko kopiranje)</span>
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
    alert("Kopirano u memoriju telefona!");
} 
</script>

</body>
</html>
