<!DOCTYPE html>
<html lang="sr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Veljko Ambrošić | Nasleđe</title>
    <style>
        body { font-family: 'Segoe UI', Arial, sans-serif; text-align: center; padding: 20px; color: #d4af37; background-color: #000; line-height: 1.6; }
        .container { max-width: 500px; margin: auto; border: 1px solid #d4af37; padding: 25px; border-radius: 15px; background-color: #050505; box-shadow: 0 0 20px rgba(212, 175, 55, 0.1); }
        h1 { color: #d4af37; margin-bottom: 5px; text-transform: uppercase; letter-spacing: 3px; font-size: 24px; }
        .subtitle { color: #888; font-size: 13px; margin-bottom: 30px; letter-spacing: 1px; text-transform: uppercase; }
        
        .note { text-align: left; background: #111; padding: 15px; border-radius: 8px; font-size: 14px; border-left: 4px solid #d4af37; color: #fff; margin-bottom: 25px; }
        
        .btn-insta { display: block; background-color: #d4af37; color: #000; padding: 18px; text-decoration: none; font-weight: bold; font-size: 16px; border-radius: 8px; margin: 20px 0; transition: 0.3s; text-transform: uppercase; }
        .btn-insta:hover { background-color: #f3cf65; transform: scale(1.02); }

        .info-box { text-align: left; margin-top: 20px; }
        .info-title { color: #d4af37; border-bottom: 1px solid #d4af37; padding-bottom: 5px; font-size: 18px; margin-bottom: 15px; }
        
        ul { list-style: none; padding: 0; color: #fff; margin-bottom: 25px; }
        li { margin-bottom: 8px; font-size: 15px; }
        li::before { content: "• "; color: #d4af37; font-weight: bold; }

        .payment-card { background: #1a1a1a; padding: 20px; border: 1px dashed #d4af37; border-radius: 8px; color: #fff; cursor: pointer; transition: 0.2s; position: relative; }
        .payment-card:active { background: #222; }
        .copy-hint { font-size: 11px; color: #d4af37; display: block; margin-top: 10px; font-style: italic; }

        .faq-section { text-align: left; margin-top: 35px; border-top: 1px solid #333; padding-top: 20px; }
        .faq-item { margin-bottom: 18px; }
        .faq-question { color: #d4af37; font-weight: bold; font-size: 15px; display: block; margin-bottom: 3px; }
        .faq-answer { color: #ccc; font-size: 14px; display: block; line-height: 1.4; }

        .footer-logo { margin-top: 50px; font-size: 10px; color: #555; letter-spacing: 3px; text-transform: uppercase; }
    </style>
</head>
<body>

<div class="container">
    <h1>Veljko Ambrošić</h1>
    <div class="subtitle">Tradicija od 1960. godine | Berlin • Beč • Pariz</div>

    <div class="note">
        <strong>VAŽNO:</strong> Svi sadržaji su deo porodičnog arhiva. Pristup je omogućen u skladu sa internim pravilima o nasleđu.
    </div>

    <a href="https://www.instagram.com/veljko_ambrosic/" target="_blank" class="btn-insta">
        💎 POŠALJI DOKAZ U DM 💎
    </a>

    <div class="info-box">
        <div class="info-title">Planovi Podrške</div>
        <ul>
            <li><strong>Regional:</strong> 15 v-r-e-d-n-o-s-t</li>
            <li><strong>Global:</strong> 35-45 v-r-e-d-n-o-s-t</li>
        </ul>

        <div class="info-title">Podaci za Pristup</div>
        <div class="payment-card" onclick="copyValue()">
            <strong>ID Identifikacija:</strong><br>
            <span id="target-id" style="letter-spacing: 1px; font-family: monospace; font-size: 16px;">RS35 2650 0100 0002 7424 38</span><br>
            <span style="font-size: 13px; color: #aaa;">Raiffeisen Banka</span>
            <span class="copy-hint">Klikni za automatsko kopiranje broja</span>
        </div>
    </div>

    <div class="faq-section">
        <h3 style="font-size: 16px; letter-spacing: 1px;">ČESTA PITANJA (FAQ)</h3>
        
        <div class="faq-item">
            <span class="faq-question">Kako funkcioniše plaćanje?</span>
            <span class="faq-answer">Koristite ID Identifikaciju iznad. Iznos zavisi od izabranog nivoa (Regional/Global).</span>
        </div>

        <div class="faq-item">
            <span class="faq-question">Gde poslati potvrdu?</span>
            <span class="faq-answer">Screenshot uplate šaljete direktno u DM klikom na zlatno dugme.</span>
        </div>

        <div class="faq-item">
            <span class="faq-question">Kada dobijam pristup?</span>
            <span class="faq-answer">Odmah nakon provere dokaza u DM-u, dobijate dalje instrukcije.</span>
        </div>
    </div>

    <div class="footer-logo">
        V. AMBROŠIĆ | SINCE 1960
    </div>
</div>

<script>
    function copyValue() {
        var text = document.getElementById("target-id").innerText.replace(/\s/g, '');
        var el = document.createElement("textarea");
        el.value = text;
        document.body.appendChild(el);
        el.select();
        document.execCommand("copy");
        document.body.removeChild(el);
        alert("Broj kopiran: " + text);
    }
</script>

</body>
</html>
