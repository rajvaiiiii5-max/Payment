<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>German Grammar Courses A1–B2</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@700&family=Roboto&display=swap" rel="stylesheet">
<style>
  *{box-sizing:border-box;margin:0;padding:0;font-family:'Roboto',sans-serif;}
  body{background: linear-gradient(135deg,#0ff,#00f,#0040ff); color:white;scroll-behavior:smooth;overflow-x:hidden;}
  header{background: rgba(0,0,0,0.6); padding:15px 20px;text-align:center;position:sticky;top:0;z-index:100;font-family:'Poppins',sans-serif;}
  nav a{color:white;margin:0 10px;text-decoration:none;font-weight:bold;}
  nav a:hover{text-decoration: underline;}
  .hero{padding:60px 20px;text-align:center;position:relative;}
  .hero h1{font-size:3rem;margin-bottom:15px; color:#0ff; text-shadow:0 0 10px #0ff;}
  .hero p{font-size:1.3rem;margin-bottom:25px;}
  .btn{background: linear-gradient(90deg,#00f,#0ff);color:white;padding:15px 25px;border:none;border-radius:30px;cursor:pointer;margin-top:15px;transition:0.3s;font-weight:bold; font-size:1.1rem;}
  .btn:hover{box-shadow:0 0 20px #0ff;transform:scale(1.05);}
  .section{padding:50px 20px;text-align:center;transition:all 0.5s ease;}
  .courses{display:grid;grid-template-columns:repeat(auto-fit,minmax(280px,1fr));gap:25px;justify-items:center;}
  .card{background: rgba(255,255,255,0.1); border-radius:20px;padding:25px;box-shadow:0 6px 20px rgba(0,0,0,0.4);transition:0.5s;width:100%; max-width:320px; cursor:pointer;}
  .card:hover{transform:translateY(-5px) scale(1.02);box-shadow:0 10px 30px rgba(0,0,0,0.6);}
  .card h3{font-family:'Poppins',sans-serif; font-size:1.6rem; margin-bottom:10px; color:#0ff; text-shadow:0 0 5px #00f;}
  .price{font-size:1.4rem;color:#0ff;font-weight:bold;margin-top:15px;}
  .topics{margin-top:15px;font-size:1rem;max-height:0;overflow:hidden;transition:max-height 0.5s ease;padding-left:15px;}
  .topics li{margin:6px 0;}
  .reviews{max-width:800px;margin:auto;}
  .review{background: rgba(255,255,255,0.1); padding:18px; border-radius:15px;margin:18px 0; box-shadow:0 4px 15px rgba(0,0,0,0.4);}
  .stars{color:gold;font-size:1.3rem;}
  .contact{max-width:600px;margin:auto;text-align:center;font-size:1.1rem;}
  footer{background: rgba(0,0,0,0.6); color:white; padding:20px;text-align:center;margin-top:20px;}

  /* Floatable Secret Button */
  .secret-btn{position:fixed;top:50%;right:0;background:#ff6600;color:white;padding:18px 25px;border-radius:30px 0 0 30px;cursor:pointer;z-index:999; font-weight:bold; box-shadow:0 4px 15px rgba(0,0,0,0.5); transform:translateY(-50%);}

  /* Secret Modal */
  .secret-page{display:none;position:fixed;top:0;left:0;width:100%;height:100%;background:rgba(0,0,0,0.95);z-index:200;overflow:auto;padding:50px 20px;}
  .secret-content{max-width:900px;margin:auto;background: rgba(0,0,0,0.85); padding:30px; border-radius:20px; color:white; animation:fadeIn 0.6s ease;}
  .secret-content h2{margin-bottom:30px;font-size:2rem;color:#0ff;text-align:center;}
  .bookshelf{display:flex;justify-content:center;gap:25px;flex-wrap:wrap;margin-bottom:30px;}
  .book-card{background: rgba(255,255,255,0.1); border-radius:20px; padding:15px; box-shadow:0 6px 20px rgba(0,0,0,0.5);transition:0.3s;width:200px; color:white;}
  .book-card:hover{transform:translateY(-5px) scale(1.05); box-shadow:0 8px 30px rgba(0,0,0,0.6);}
  .book-card img{width:100%;border-radius:12px;margin-bottom:10px;transition:0.3s;}
  .book-card img:hover{transform:scale(1.05);}
  .book-card h4{margin-bottom:5px;font-size:1rem; color:#0ff;}
  .resources{max-width:600px;margin:0 auto;text-align:left;}
  .resources ul{list-style:disc; padding-left:20px;}

  @keyframes fadeIn{from{opacity:0}to{opacity:1}}
</style>
</head>
<body>

<div class="secret-btn" onclick="openSecretPage()">Secret</div>

<header>
  <h2>German Grammar A1–B2</h2>
  <nav>
    <a href="#bundle">Bundle</a>
    <a href="#courses">Courses</a>
    <a href="#pricing">Payment</a>
    <a href="#reviews">Reviews</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<section class="hero">
  <h1>Master German Grammar</h1>
  <p>Learn A1 to B2 — only grammar topics, structured & clear.</p>
  <button class="btn" onclick="scrollToPayment()">Buy Full Package</button>
</section>

<section id="bundle" class="section">
  <h2>Full Package</h2>
  <div class="courses">
    <div class="card bundle">
      <h3>A1–B2 Grammar Full Access</h3>
      <p>All 40 grammar topics in one package.</p>
      <p class="price">Rs. 2000</p>
      <button class="btn" onclick="scrollToPayment()">Buy Course</button>
    </div>
  </div>
  <div class="section" style="margin-top:20px; background:rgba(255,255,255,0.1); border-radius:15px; padding:20px; max-width:700px; margin-left:auto; margin-right:auto;">
    <h3 style="color:#0ff;">Refund Policy</h3>
    <p>If you are not satisfied, you can request a refund within <strong>3 days</strong> of purchase.</p>
  </div>
</section>

<section id="courses" class="section">
  <h2>Individual Courses</h2>
  <div class="courses">
    <!-- A1 Card -->
    <div class="card">
      <h3>A1 Grammar</h3>
      <button class="btn" onclick="toggleSingle('a1-topics')">View Course</button>
      <ul class="topics" id="a1-topics">
        <li>Present tense (regular verbs)</li>
        <li>Sein & haben usage</li>
        <li>Definite/indefinite articles</li>
        <li>Noun plurals</li>
        <li>Personal pronouns</li>
        <li>Basic negation (kein/nicht)</li>
        <li>Modal verbs basics</li>
        <li>Word order in main clause</li>
        <li>Yes/No & W-questions</li>
        <li>Accusative case basics</li>
      </ul>
      <p class="price">Rs. 500</p>
      <button class="btn" onclick="scrollToPayment(event)">Buy Course</button>
    </div>

    <!-- Repeat similar for A2, B1, B2 -->
    <div class="card">
      <h3>A2 Grammar</h3>
      <button class="btn" onclick="toggleSingle('a2-topics')">View Course</button>
      <ul class="topics" id="a2-topics">
        <li>Perfect tense (haben/sein)</li>
        <li>Simple past of sein & haben</li>
        <li>Dative case basics</li>
        <li>Two-way prepositions</li>
        <li>Comparatives & superlatives</li>
        <li>Reflexive verbs</li>
        <li>Modal verbs extended</li>
        <li>Separable verbs</li>
        <li>Conjunctions (weil, dass)</li>
        <li>Time expressions in sentences</li>
      </ul>
      <p class="price">Rs. 700</p>
      <button class="btn" onclick="scrollToPayment(event)">Buy Course</button>
    </div>

    <div class="card">
      <h3>B1 Grammar</h3>
      <button class="btn" onclick="toggleSingle('b1-topics')">View Course</button>
      <ul class="topics" id="b1-topics">
        <li>Passive voice basics</li>
        <li>Indirect speech</li>
        <li>Future tense</li>
        <li>Relative clauses</li>
        <li>Subjunctive II (würde)</li>
        <li>Advanced prepositions</li>
        <li>Modal verbs past tense</li>
        <li>Separable & inseparable verbs review</li>
        <li>Advanced word order</li>
        <li>Conditional sentences</li>
      </ul>
      <p class="price">Rs. 900</p>
      <button class="btn" onclick="scrollToPayment(event)">Buy Course</button>
    </div>

    <div class="card">
      <h3>B2 Grammar</h3>
      <button class="btn" onclick="toggleSingle('b2-topics')">View Course</button>
      <ul class="topics" id="b2-topics">
        <li>Advanced passive voice</li>
        <li>Subjunctive II advanced</li>
        <li>Reported speech complex</li>
        <li>Nominalization</li>
        <li>Complex sentence connectors</li>
        <li>Adjective endings full review</li>
        <li>Prepositional phrases</li>
        <li>Advanced conditional sentences</li>
        <li>Indirect questions</li>
        <li>Modal verbs complex usage</li>
      </ul>
      <p class="price">Rs. 1100</p>
      <button class="btn" onclick="scrollToPayment(event)">Buy Course</button>
    </div>

  </div>
</section>

<section id="pricing" class="section">
  <h2>Payment</h2>
  <img src="https://i.ibb.co/R46YHVyw/qr.png" alt="QR Payment" style="width:220px; border-radius:15px; box-shadow:0 4px 15px rgba(0,0,0,0.5);">
  <p style="margin-top:10px;">Scan this QR to pay</p>
  <button class="btn" onclick="window.open('https://tally.so/r/w457JX','_blank')">Submit Payment Screenshot</button>
</section>

<section id="reviews" class="section">
  <h2>Student Reviews</h2>
  <div class="reviews">
    <div class="review"><p class="stars">★★★★★</p><p>“Goethe exam became so easy after this grammar course!”</p></div>
    <div class="review"><p class="stars">★★★★★</p><p>“Passed VHS B1 confidently — structured lessons helped me a lot.”</p></div>
    <div class="review"><p class="stars">★★★★☆</p><p>“Very useful, only grammar focus — exactly what I needed.”</p></div>
  </div>
</section>

<section id="contact" class="section">
  <h2>Contact</h2>
  <div class="contact">
    Email: <a href="mailto:rajvaiiiii5@gmail.com" style="color:#0ff;">rajvaiiiii5@gmail.com</a>
  </div>
</section>

<section class="secret-page" id="secret">
  <div class="secret-content">
    <h2>You access all these resources</h2>
    <div class="bookshelf">
      <div class="book-card">
        <img src="https://i.ibb.co/YBpWcNHX/book1.png" alt="Einfach Gramitik">
        <h4>Einfach Gramitik A1–B1</h4>
      </div>
      <div class="book-card">
        <img src="https://i.ibb.co/jZMf592X/book2.png" alt="Basic German">
        <h4>Basic German</h4>
      </div>
      <div class="book-card">
        <img src="https://i.ibb.co/tp9M7vVj/book3.png" alt="Collins Easy German">
        <h4>Collins Easy German</h4>
      </div>
    </div>
    <div class="resources">
      <h3>Also you get:</h3>
      <ul>
        <li>Vocabulary list PDF</li>
        <li>GOOTHE and VHS 5 model set of all levels</li>
        <li>Vocabulary book</li>
        <li>A1 handwritten notes</li>
        <li>Conventional German book</li>
        <li>Short story German book</li>
        <li>Quiz on every grammar topic</li>
      </ul>
    </div>
    <button class="btn" style="margin-top:20px;" onclick="closeSecretPage()">Close</button>
  </div>
</section>

<footer>
  <p>&copy; 2025 German Grammar Course. All Rights Reserved.</p>
</footer>

<script>
function toggleSingle(id){
  const allTopics = document.querySelectorAll('.topics');
  allTopics.forEach(t => {if(t.id !== id){t.style.maxHeight='0';}});
  const el = document.getElementById(id);
  if(el.style.maxHeight && el.style.maxHeight !== '0px'){
    el.style.maxHeight='0';
  } else {
    el.style.maxHeight = el.scrollHeight + 'px';
  }
}

function scrollToPayment(e){
  if(e)
  
if(e) e.stopPropagation();
  document.getElementById('pricing').scrollIntoView({behavior:'smooth'});
}

function openSecretPage(){
  document.getElementById('secret').style.display='block';
}

function closeSecretPage(){
  document.getElementById('secret').style.display='none';
}
</script>

</body>
</html>
  
  
  
  
  
  
