<!DOCTYPE html>
<html lang="sr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Veljko Ambrošić | Zvanična Prezentacija</title>
    
    <meta property="og:title" content="Veljko Ambrošić | Portfolio">
    <meta property="og:description" content="Tradicija i nasleđe od 1960. godine.">
    <meta property="og:type" content="website">
    
    <style>
        body { font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; text-align: center; padding: 20px; color: #333; line-height: 1.6; background-color: #fff; }
        .container { max-width: 500px; margin: auto; }
        h1 { color: #000; margin-bottom: 5px; }
        .subtitle { color: #888; font-size: 14px; margin-bottom: 30px; text-transform: uppercase; letter-spacing: 1px; }
        .btn-insta { display: block; background-color: #000; color: #d4af37; padding: 18px; text-decoration: none; font-weight: bold; font-size: 16px; border: 2px solid #d4af37; border-radius: 8px; margin: 25px 0; transition: 0.3s; }
        .btn-insta:hover { background-color: #d4af37; color: #000; }
        .note { text-align: left; background: #fdfdfd; padding: 20px; border-radius: 8px; font-size: 14px; border-left: 4px solid #d4af37; box-shadow: 0 2px 5px rgba(0,0,0,0.05); }
        .faq { margin-top: 40px; padding: 20px; border-top: 2px solid #d4af37; text-align: left; }
        .iban-box { background: #f4f4f4; padding: 15px; border: 1px dashed #d4af37; cursor: pointer; position: relative; border-radius: 5px; margin-top: 10px; }
        .copy-hint { font-size: 11px; color: #d4af37; font-weight: bold; display: block; margin-top: 5px; }
        .price-list { list-style: none; padding: 0; }
        .price-list li { margin-bottom: 10px; padding-left: 20px; position: relative; }
        .price-list li::before { content: "•"; color: #d4af37; font-weight: bold; position: absolute; left: 0; }
    </style>
</head>
<body>

<div class="container">
    <h1>Veljko Ambrošić</h1>
    <p class="subtitle">Tradicija od 1960. godine | Berlin • Beč • Pariz • Rđica</p>

    <div class="note">
        <strong>O b e v e š t e nj e:</strong> Svi sadržaji su povezani sa porodičnim nasleđem. Podrška se realizuje kroz zvanične bankarske kanale (R. Banka).
    </div>

    <a href="https://www.instagram.com/veljko_ambrosic/" target="_blank" class="btn-insta">
        💎 POŠALJI POTVRDU NA INSTAGRAM 💎
    </a>

    <div id="cesta-pitanja" class="faq">
        <h2 style="color: #d4af37;">Informacije</h2>
        <p><strong>Članstvo (po regijama):</strong></p>
        <ul class="price-list">
            <li>Balkan zona: 15 (EUR/RSD)</li>
            <li>Int. zona: 35-45 (EUR)</li>
        </ul>

        <p><strong>Podaci za podršku:</strong></p>
        <div class="iban-box" onclick="copyIban()">
            <strong>Primalac:</strong> Veljko Ambrošić<br>
            <strong>Banka:</strong> R. Banka<br>
            <strong>I-B-A-N:</strong> <span id="iban-num">RS35 2650 0100 0002 7424 38</span>
            <span class="copy-hint">(Klikni polje za kopiranje)</span>
        </div>

        <p style="margin-top: 25px;"><strong>Koraci:</strong> Nakon potvrde uplate, pošaljite screenshot u DM. Pristup se odobrava odmah nakon obrade.</p>
    </div>

    <p style="margin-top: 50px; font-size: 11px; color: #999; letter-spacing: 2px;">
        VELJKO AMBROŠIĆ | TRADICIJA I KVALITET
    </p>
</div>

<script>
function copyIban() {
    // Uklanjamo razmake pre kopiranja da bi broj bio ispravan za banku
    var ibanText = document.getElementById("iban-num").innerText.replace(/\s/g, '');
    navigator.clipboard.writeText(ibanText).then(function() {
        alert("Podaci su kopirani!");
    }, function(err) {
        console.error('Greška: ', err);
    });
}
</script>

</body>
</html
