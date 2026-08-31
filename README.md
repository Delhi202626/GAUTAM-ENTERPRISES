<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>GAUTAM ENTERPRISES | Luxury Jewellery</title>
<style>
:root{--gold:#b8891f;--gold2:#e7c86e;--gold3:#f7e9b1;--ink:#2a2418;--cream:#fffdf7;--ivory:#f8f4ea;--line:#e8dcc0;--muted:#766f62}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{font-family:Georgia,"Times New Roman",serif;background:var(--cream);color:var(--ink);line-height:1.6}
a{text-decoration:none;color:inherit}
.container{width:min(1180px,92%);margin:auto}
header{position:sticky;top:0;z-index:50;background:rgba(255,253,247,.94);backdrop-filter:blur(16px);border-bottom:1px solid rgba(184,137,31,.25);box-shadow:0 6px 26px rgba(94,65,11,.07)}
.nav{height:82px;display:flex;align-items:center;justify-content:space-between;gap:25px}
.logo{font-size:25px;letter-spacing:3px;color:#6e5316;font-weight:bold}
.logo span{display:block;font:10px Arial;letter-spacing:5px;color:#84775f;text-align:center}
nav{display:flex;gap:25px;font:12px Arial;text-transform:uppercase;letter-spacing:1.5px;color:#554d40}
nav a{position:relative}
nav a:after{content:"";position:absolute;left:0;bottom:-7px;width:0;height:1px;background:var(--gold);transition:.3s}
nav a:hover{color:var(--gold);}.nav a:hover:after{width:100%}
.actions{display:flex;gap:10px}.icon{border:1px solid rgba(184,137,31,.4);background:#fff;color:#6d541c;border-radius:50%;width:39px;height:39px;cursor:pointer;box-shadow:0 5px 15px rgba(96,67,13,.08)}
.hero{min-height:690px;display:grid;place-items:center;text-align:center;position:relative;overflow:hidden;background:
radial-gradient(circle at 50% 30%,rgba(232,201,111,.30),transparent 25%),
linear-gradient(135deg,#fffdf8 0%,#fbf6e9 48%,#fff 100%)}
.hero:before,.hero:after{content:"";position:absolute;border-radius:50%;filter:blur(1px);pointer-events:none}
.hero:before{width:520px;height:520px;border:1px solid rgba(184,137,31,.20);box-shadow:0 0 0 18px rgba(184,137,31,.03),0 0 0 36px rgba(184,137,31,.025),inset 0 0 70px rgba(184,137,31,.06);animation:float 7s ease-in-out infinite}
.hero:after{width:8px;height:220px;background:linear-gradient(transparent,var(--gold2),transparent);transform:rotate(36deg);left:16%;top:10%;opacity:.22;animation:shimmer 5s infinite}
@keyframes float{50%{transform:translateY(-10px) scale(1.015)}}@keyframes shimmer{50%{left:82%;top:65%;opacity:.55}}
.hero-content{position:relative;z-index:1;padding:50px 15px}
.kicker{font:11px Arial;letter-spacing:5px;color:#9a7218;text-transform:uppercase}
h1{font-size:clamp(52px,8vw,98px);line-height:.92;margin:20px 0;background:linear-gradient(135deg,#4f3a0d 10%,#c39a32 48%,#7e5d12 85%);-webkit-background-clip:text;color:transparent;text-shadow:0 5px 35px rgba(184,137,31,.10)}
.hero p{font:15px Arial;color:#6b6457;max-width:700px;margin:0 auto 32px}
.btn{display:inline-block;padding:14px 29px;border:1px solid #b88a22;background:linear-gradient(135deg,#f2d77c,#c89b32,#ebcf72);color:#372809;font:bold 11px Arial;letter-spacing:1.5px;text-transform:uppercase;border-radius:999px;cursor:pointer;box-shadow:0 12px 30px rgba(183,136,31,.20);transition:.3s}
.btn:hover{transform:translateY(-3px);box-shadow:0 16px 35px rgba(183,136,31,.28)}
.btn.outline{background:rgba(255,255,255,.6);color:#755613;margin-left:8px}
section{padding:86px 0}.section-title{text-align:center;margin-bottom:42px}.section-title small{font:10px Arial;letter-spacing:4px;color:#a37a1b}.section-title h2{font-size:42px;margin-top:8px;color:#312818}
.categories{display:grid;grid-template-columns:repeat(4,1fr);gap:20px}
.cat{height:260px;border:1px solid var(--line);padding:29px;display:flex;flex-direction:column;justify-content:end;background:
linear-gradient(145deg,rgba(255,255,255,.96),rgba(250,244,229,.96));position:relative;overflow:hidden;border-radius:18px;box-shadow:0 12px 35px rgba(72,52,14,.07);transition:.35s}
.cat:before{content:"";position:absolute;inset:0;background:radial-gradient(circle at 80% 20%,rgba(232,200,105,.35),transparent 28%)}
.cat:after{content:"✦";position:absolute;right:20px;top:13px;font-size:80px;color:rgba(184,137,31,.12);transform:rotate(15deg)}
.cat:hover{transform:translateY(-8px);box-shadow:0 20px 45px rgba(72,52,14,.12);border-color:#d6bc75}
.cat h3{font-size:25px;color:#775915;position:relative;z-index:1}.cat p{font:12px Arial;color:#847b6b;position:relative;z-index:1}
.products{display:grid;grid-template-columns:repeat(4,1fr);gap:22px}
.product{background:#fff;border:1px solid var(--line);overflow:hidden;border-radius:18px;box-shadow:0 12px 32px rgba(72,52,14,.07);transition:.35s}
.product:hover{transform:translateY(-8px);box-shadow:0 22px 45px rgba(72,52,14,.13);border-color:#d5b866}
.pic{height:255px;display:grid;place-items:center;background:radial-gradient(circle at 50% 45%,#fffdf5,#f6ecd0 45%,#fff 76%);position:relative}
.pic:after{content:"";position:absolute;inset:14px;border:1px solid rgba(184,137,31,.18);border-radius:14px}
.jewel{font-size:102px;filter:drop-shadow(0 12px 18px rgba(82,59,13,.18));color:#c89a2d;position:relative;z-index:1}
.info{padding:20px}.info h3{font-size:19px;color:#3e3527}.info p{font:12px Arial;color:#8c8373;margin:5px 0 12px}.price{color:#9a7217;font:bold 16px Arial}.buy{float:right;background:#fff;border:1px solid #ceb365;color:#8d6817;padding:7px 11px;cursor:pointer;border-radius:999px}
.banner{background:linear-gradient(135deg,#fff,#f7efda 55%,#fff);border:1px solid #e1cf9e;padding:60px;text-align:center;border-radius:24px;box-shadow:0 18px 50px rgba(72,52,14,.08);position:relative;overflow:hidden}
.banner:before{content:"";position:absolute;inset:-40%;background:linear-gradient(90deg,transparent,rgba(255,255,255,.8),transparent);transform:rotate(25deg);animation:bannerShine 6s infinite}
@keyframes bannerShine{50%{transform:translateX(45%) rotate(25deg)}} .banner>*{position:relative;z-index:1}
.banner h2{font-size:45px;color:#6f5214}.banner p{font:14px Arial;color:#776f62;margin:10px 0 24px}
.about{display:grid;grid-template-columns:1fr 1fr;gap:55px;align-items:center}
.about-art{min-height:355px;border:1px solid #ddca94;display:grid;place-items:center;border-radius:24px;background:
radial-gradient(circle,#f3dd9b 0,#f9f0d9 30%,#fff 72%);font-size:132px;color:#a87b17;box-shadow:inset 0 0 70px rgba(184,137,31,.09),0 20px 45px rgba(72,52,14,.08)}
.about h2{font-size:44px;margin:10px 0;color:#30281b}.about p{font:15px Arial;color:#746c5d;margin-bottom:18px}
.contact{display:grid;grid-template-columns:1fr 1fr;gap:28px}
.box{border:1px solid var(--line);padding:32px;background:#fff;border-radius:20px;box-shadow:0 14px 35px rgba(72,52,14,.06)}
.box h3{color:#735515;font-size:24px;margin-bottom:15px}.box p{font:14px Arial;color:#756d5f;margin:9px 0}
form{display:grid;gap:12px}input,textarea{width:100%;padding:14px 15px;background:#fffcf5;border:1px solid #ded2b8;color:#3a3224;font:14px Arial;border-radius:10px;outline:none}input:focus,textarea:focus{border-color:#c8a44b;box-shadow:0 0 0 3px rgba(200,164,75,.10)}textarea{min-height:110px}
footer{border-top:1px solid var(--line);padding:38px 0;text-align:center;color:#8b8375;font:12px Arial;background:#fffdf8}footer strong{color:#8d6817}
.cart{position:fixed;right:22px;bottom:22px;z-index:60;background:linear-gradient(135deg,#f0d373,#b9871d);color:#3b2c09;border:0;padding:15px 20px;border-radius:999px;font:bold 12px Arial;box-shadow:0 12px 35px rgba(86,61,12,.22);cursor:pointer}
#count{background:#fff;color:#6e5316;border-radius:50%;padding:3px 7px;margin-left:5px}
@media(max-width:850px){nav{display:none}.categories,.products{grid-template-columns:repeat(2,1fr)}.about,.contact{grid-template-columns:1fr}.hero{min-height:590px}}
@media(max-width:520px){.categories,.products{grid-template-columns:1fr}.hero h1{font-size:57px}.banner{padding:38px 20px}.banner h2{font-size:32px}.btn.outline{margin-left:0;margin-top:10px}.actions{display:none}.section-title h2{font-size:34px}}
</style>
</head>
<body>
<header><div class="container nav">
<div class="logo">GAUTAM ENTERPRISES<span>JEWELLERY &amp; LUXURY</span></div>
<nav><a href="#home">Home</a><a href="#collections">Collections</a><a href="#products">Jewellery</a><a href="#about">About</a><a href="#contact">Contact</a></nav>
<div class="actions"><button class="icon" onclick="searchProducts()">⌕</button><button class="icon" onclick="showCart()">🛒</button></div>
</div></header>

<main id="home">
<section class="hero"><div class="hero-content"><div class="kicker">Timeless Elegance • Crafted For You</div><h1>Wear Your<br>Story.</h1><p>Discover exquisite jewellery designed to celebrate every unforgettable moment. Sophisticated craftsmanship with a signature touch of luxury.</p><a class="btn" href="#products">Explore Collection</a><a class="btn outline" href="#contact">Enquire Now</a></div></section>

<section style="padding:26px 0 10px;background:#fff;border-bottom:1px solid #eee2c7;">
<div class="container" style="display:grid;grid-template-columns:repeat(4,1fr);gap:15px;text-align:center;font:12px Arial;color:#766d5d;">
<div>✧ <b>Premium Craftsmanship</b></div><div>✧ <b>Elegant Designs</b></div><div>✧ <b>Personalised Service</b></div><div>✧ <b>Luxury Gifting</b></div>
</div></section>
<section id="collections"><div class="container"><div class="section-title"><small>OUR COLLECTIONS</small><h2>Find Your Signature</h2></div>
<div class="categories">
<div class="cat"><h3>Rings</h3><p>Elegant pieces for every occasion</p></div>
<div class="cat"><h3>Necklaces</h3><p>Statement luxury, beautifully crafted</p></div>
<div class="cat"><h3>Earrings</h3><p>Subtle sparkle to timeless glamour</p></div>
<div class="cat"><h3>Bracelets</h3><p>Refined details around your wrist</p></div>
</div></div></section>

<section id="products"><div class="container"><div class="section-title"><small>CURATED FOR YOU</small><h2>Featured Jewellery</h2></div>
<div class="products" id="productGrid">
<div class="product"><div class="pic"><div class="jewel">💍</div></div><div class="info"><h3>Royal Solitaire Ring</h3><p>Premium finish • Elegant design</p><span class="price">₹24,999</span><button class="buy" onclick="addCart('Royal Solitaire Ring')">ADD</button></div></div>
<div class="product"><div class="pic"><div class="jewel">📿</div></div><div class="info"><h3>Golden Heritage Necklace</h3><p>Classic statement collection</p><span class="price">₹39,999</span><button class="buy" onclick="addCart('Golden Heritage Necklace')">ADD</button></div></div>
<div class="product"><div class="pic"><div class="jewel">✨</div></div><div class="info"><h3>Diamond Glow Earrings</h3><p>Graceful • Lightweight • Chic</p><span class="price">₹18,999</span><button class="buy" onclick="addCart('Diamond Glow Earrings')">ADD</button></div></div>
<div class="product"><div class="pic"><div class="jewel">🔗</div></div><div class="info"><h3>Signature Gold Bracelet</h3><p>Minimal luxury for every day</p><span class="price">₹29,999</span><button class="buy" onclick="addCart('Signature Gold Bracelet')">ADD</button></div></div>
</div></div></section>

<section><div class="container"><div class="banner"><div class="kicker">SPECIAL COLLECTION</div><h2>Luxury That Lasts Forever</h2><p>Make your special moments shine brighter with Gautam Enterprises.</p><a class="btn" href="#contact">Book A Consultation</a></div></div></section>

<section id="about"><div class="container about"><div class="about-art">♕</div><div><div class="kicker">GAUTAM ENTERPRISES</div><h2>Crafted With Passion</h2><p>We bring together timeless jewellery aesthetics and contemporary elegance. Every piece is selected to add confidence, beauty and unforgettable sparkle to your story.</p><p>Visit us for personalised assistance, gifting and jewellery enquiries.</p><a class="btn" href="#contact">Talk To Us</a></div></div></section>

<section id="contact"><div class="container"><div class="section-title"><small>GET IN TOUCH</small><h2>Let's Create Something Beautiful</h2></div><div class="contact">
<div class="box"><h3>Gautam Enterprises</h3><p>📍 Your Jewellery Store Address</p><p>📞 +91 XXXXX XXXXX</p><p>✉️ info@gautamenterprises.com</p><p>🕐 Mon – Sun: 10:00 AM – 8:00 PM</p><br><a class="btn" style="background:linear-gradient(135deg,#e7cf82,#fff3c8,#d9ba5a)" href="https://wa.me/91XXXXXXXXXX" target="_blank">WhatsApp Enquiry</a></div>
<div class="box"><h3>Send An Enquiry</h3><form onsubmit="sendEnquiry(event)"><input id="name" placeholder="Your Name" required><input id="phone" placeholder="Mobile Number" required><input id="interest" placeholder="Jewellery you're interested in"><textarea id="message" placeholder="Your message"></textarea><button class="btn" type="submit">Send Enquiry</button></form></div>
</div></div></section>
</main>
<button class="cart" onclick="showCart()">🛒 Cart <span id="count">0</span></button>
<footer>© 2026 <strong>GAUTAM ENTERPRISES</strong> — Jewellery &amp; Luxury. All rights reserved.</footer>

<script>
let cart=[];
function addCart(name){cart.push(name);document.getElementById('count').textContent=cart.length;alert(name+' added to your enquiry cart.');}
function showCart(){alert(cart.length?('Your enquiry cart:\\n\\n'+cart.map((x,i)=>(i+1)+'. '+x).join('\\n')):'Your enquiry cart is empty.');}
function searchProducts(){let q=prompt('Search jewellery:');if(!q)return;let cards=document.querySelectorAll('.product');cards.forEach(c=>c.style.display=c.innerText.toLowerCase().includes(q.toLowerCase())?'block':'none');location.hash='products';}
function sendEnquiry(e){e.preventDefault();alert('Thank you, '+document.getElementById('name').value+'! Your enquiry has been recorded. Please connect your WhatsApp number/email in the HTML to receive real messages.');e.target.reset();}
</script>
</body>
</html>
