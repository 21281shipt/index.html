<!DOCTYPE html>
<html lang="sr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Veljko Ambrošić | Nasleđe i Ekskluzivnost</title>
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
        .iban-box:active { background: #e0e0e0; }
        .copy-hint { font-size: 11px; color: #d4af37; font-weight: bold; display: block; margin-top: 5px; }
        .price-list { list-style: none; padding: 0; }
        .price-list li { margin-bottom: 10px; padding-left: 20px; position: relative; }
        .price-list li::before { content: "•"; color: #d4af37; font-weight: bold; position: absolute; left: 0; }
    </style>
</head>
<body>

<div class="container">
    <h1>Veljko Ambrošić</h1>
    <div class="subtitle">Tradicija od 1960. godine | Berlin • Beč • Pariz • Rđica</div>

    <div class="note">
        <strong>Napomena o legitimitetu:</strong> Svi prihodi ostvareni kroz digitalnu ekskluzivnu zonu povezani su sa višedecenijskim porodičnim nasleđem. Sve transakcije se obavljaju putem zvaničnih platformi na račun u Raiffeisen banci.
    </div>

    <a href="https://www.instagram.com/veljko_ambrosic/" target="_blank" class="btn-insta">
        💎 POŠALJI POTVRDU NA INSTAGRAM 💎
    </a>

    <div id="cesta-pitanja" class="faq">
        <h2 style="color: #d4af37;">Česta pitanja</h2>
        <p><strong>Cena (zavisno od regije):</strong></p>
        <ul class="price-list">
            <li>Balkan: 15 EUR (ili protivvrednost u RSD)</li>
            <li>Internacionalni deo: 35-45 EUR</li>
        </ul>

        <p><strong>Podaci za uplatu:</strong></p>
        <div class="iban-box" onclick="copyIban()">
            <strong>Primalac:</strong> Veljko Ambrošić<br>
            <strong>Banka:</strong> Raiffeisen Banka<br>
            <strong>IBAN:</strong> <span id="iban-num">RS35265001000002742438</span>
            <span class="copy-hint">(Klikni na polje da kopiraš IBAN)</span>
        </div>

        <p style="margin-top: 25px;"><strong>Instrukcije:</strong> Nakon uplate, slikajte potvrdu (screenshot ili uplatnicu) i pošaljite je u DM. Pristup dobijate odmah nakon provere.</p>
    </div>

    <p style="margin-top: 50px; font-size: 11px; color: #999; letter-spacing: 2px;">
        VELJKO AMBROŠIĆ | NASLEĐE I KVALITET
    </p>
</div>

<script>
    function copyIban() {
        var ibanText = document.getElementById("iban-num").innerText;
        navigator.clipboard.writeText(ibanText).then(function() {
            alert("IBAN je uspešno kopiran: " + ibanText);
        }, function(err) {
            console.error('Greška pri kopiranju: ', err);
        });
    }
</script>

</body>
</html>
