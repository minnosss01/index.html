# index.html
<!DOCTYPE html>
<html lang="ms">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Walimatulurus Amin & Alysa</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

body{
    font-family: Arial, sans-serif;
    background:#f7fbfb;
    color:#333;
    text-align:center;
}

.hero{
    min-height:100vh;
    background:linear-gradient(135deg,#0f766e,#14b8a6);
    color:white;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    padding:30px;
}

.hero h1{
    font-size:2.2rem;
    margin-bottom:15px;
}

.hero p{
    margin-bottom:20px;
}

.btn{
    display:inline-block;
    background:white;
    color:#0f766e;
    padding:12px 25px;
    border-radius:30px;
    text-decoration:none;
    font-weight:bold;
}

.section{
    padding:60px 20px;
}

.section h2{
    color:#0f766e;
    margin-bottom:20px;
}

.countdown{
    font-size:1.5rem;
    font-weight:bold;
}

.card{
    max-width:700px;
    margin:auto;
}

.map-btn{
    display:inline-block;
    margin:10px;
    padding:12px 20px;
    border-radius:25px;
    text-decoration:none;
    background:#0f766e;
    color:white;
}

.gallery{
    display:grid;
    grid-template-columns:repeat(2,1fr);
    gap:10px;
    max-width:700px;
    margin:auto;
}

.gallery img{
    width:100%;
    border-radius:10px;
}

.footer{
    background:#0f766e;
    color:white;
    padding:40px 20px;
}
</style>
</head>

<body>

<section class="hero">
    <h3>Walimatulurus</h3>

    <h1>
        Muhammad Amin Nursiddiq<br>
        bin Mat Noor
    </h1>

    <p>&</p>

    <h1>
        Alysa Syuhaidah<br>
        binti Mohd Sharizan
    </h1>

    <p>08 Ogos 2026</p>

    <a href="#jemputan" class="btn">
        Buka Jemputan
    </a>
</section>

<section id="jemputan" class="section">
    <div class="card">
        <h2>Assalamualaikum W.B.T</h2>

        <p>
            Dengan penuh kesyukuran ke hadrat Allah SWT,
            kami menjemput Dato', Datin, Tuan, Puan,
            Saudara dan Saudari ke Majlis Walimatulurus kami.
        </p>
    </div>
</section>

<section class="section">
    <h2>Countdown Hari Bahagia</h2>

    <div class="countdown" id="countdown">
        Loading...
    </div>
</section>

<section class="section">
    <h2>Maklumat Majlis</h2>

    <p><strong>Tarikh:</strong> 08 Ogos 2026</p>
    <br>
    <p><strong>Masa:</strong> 11.00 Pagi - 4.00 Petang</p>
    <br>
    <p><strong>Lokasi:</strong></p>

    <p>
        Masjid Universiti Putra Malaysia (UPM)<br>
        43400 Serdang, Selangor
    </p>

    <br>

    <a class="map-btn"
    href="https://maps.app.goo.gl/c7BTA1nXyMPWPgKv7?g_st=ic">
        Google Maps
    </a>

    <a class="map-btn"
    href="https://waze.com/ul/hw2834dkwc">
        Waze
    </a>
</section>

<section class="section">
    <h2>Galeri</h2>

    <div class="gallery">
        <img src="gambar1.jpg">
        <img src="gambar2.jpg">
        <img src="gambar3.jpg">
        <img src="gambar4.jpg">
    </div>

    <br>

    <small>
        Tukar gambar1.jpg dan seterusnya dengan gambar sebenar.
    </small>
</section>

<section class="section">
    <h2>Hadiah & Sumbangan</h2>

    <p>
        Kehadiran dan doa restu anda amat kami hargai.
    </p>

    <br>

    <img src="duitnow.png"
    width="250"
    alt="QR DuitNow">

    <br><br>

    <strong>
        Muhammad Amin Nursiddiq bin Mat Noor
    </strong>
</section>

<section class="section">
    <h2>Doa</h2>

    <p>
        Semoga Allah SWT memberkati
        perkahwinan kami dan mengurniakan
        kebahagiaan hingga ke syurga.
    </p>
</section>

<footer class="footer">
    <h3>Amin & Alysa</h3>
    <br>
    <p>08.08.2026</p>
</footer>

<script>

const targetDate =
new Date("August 8, 2026 00:00:00").getTime();

setInterval(function(){

let now = new Date().getTime();

let distance = targetDate - now;

let days =
Math.floor(distance/(1000*60*60*24));

let hours =
Math.floor((distance%(1000*60*60*24))
/(1000*60*60));

let minutes =
Math.floor((distance%(1000*60*60))
/(1000*60));

let seconds =
Math.floor((distance%(1000*60))
/1000);

document.getElementById("countdown")
.innerHTML =
days + " Hari " +
hours + " Jam " +
minutes + " Minit " +
seconds + " Saat";

},1000);

</script>

</body>
</html>