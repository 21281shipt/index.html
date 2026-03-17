<!DOCTYPE html>
<html lang="sr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Veljko Ambrošić | Nasleđe i Ekskluzivnost</title>
    <style>
        body { font-family: sans-serif; text-align: center; padding: 20px; color: #333; line-height: 1.6; }
        .container { max-width: 500px; margin: auto; }
        .btn-insta { display: block; background-color: #000; color: #d4af37; padding: 20px; text-decoration: none; font-weight: bold; font-size: 18px; border: 1px solid #d4af37; border-radius: 5px; margin: 20px 0; }
        .note { text-align: left; background: #f9f9f9; padding: 20px; border-radius: 5px; font-size: 14px; }
        .faq { margin-top: 40px; padding: 20px; border-top: 2px solid #d4af37; text-align: left; }
        .iban-box { background: #eee; padding: 15px; border: 1px dashed #d4af37; cursor: pointer; position: relative; }
        .iban-box:active { background: #e0e0e0; }
        .copy-hint { font-size: 10px; color: #d4af37; font-weight: bold; }
    </style>
</head>
<body>

<div class="container">
    <h1 style="font-size: 32px; margin-bottom: 5px;">Veljko Ambrošić</h1>
    <p style="font-size: 16px; color: #555; margin-bottom: 30px;">
        Tradicija od 1960. godine | Generacijski projekti: Berlin, Beč, Pariz, Rđica
    </p>

    <div class="note">
        <p><strong>Napomena o legitimitetu:</strong> Svi prihodi ostvareni kroz digitalnu ekskluzivnu zonu povezani su sa višedecenijskim porodičnim nasleđem. Sve transakcije se obavljaju putem zvaničnih platformi na račun u Raiffeisen banci.</p>
    </div>

    <a href="https://www.instagram.com/veljko_ambrosic/" class="btn-insta">
        💎 POŠALJI POTVRDU NA INSTAGRAM 💎
    </a>

    <div id="cesta-pitanja" class="faq">
        <h2 style="color: #d4af37;">Česta pitanja</h2>
        <p><strong>Cena (zavisno od regije):</strong></p>
        <ul>
            <li>Balkan: 15 EUR (ili protivvrednost u RSD)</li>
            <li>Internacionalni deo: 35-45 EUR</li>
        </ul>

        <p><strong>Podaci za uplatu:</strong></p>
        <div class="iban-box" onclick="copyIban()">
            <strong>Primalac:</strong> Veljko Ambrošić<br>
            <strong>Banka:</strong> Raiffeisen Banka<br>
            <strong>IBAN:</strong> <span id="iban-num">RS35265001000002742438</span>
            <br><span class="copy-hint">(Klikni na polje da kopiraš IBAN)</span>
        </div>

        <p style="margin-top: 20px;"><strong>Instrukcije:</strong> Nakon uplate, slikajte potvrdu (e-banking screenshot ili uplatnicu) i pošaljite je u DM. Pristup dobijate odmah nakon provere.</p>
    </div>

    <p style="margin-top: 30px; font-size: 11px; color: #999; letter-spacing: 2px;">
        VELJKO AMBROŠIĆ | NASLEĐE I KVALITET
    </p>
</div>

<script>
    function copyIban() {
        var ibanText = document.getElementById("iban-num").innerText;
        navigator.clipboard.writeText(ibanText);
        alert("IBAN je kopiran: " + ibanText);
    }
</script>

</body>
</html>
