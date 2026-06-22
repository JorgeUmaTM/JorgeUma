<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ShoeUma | Corre hacia la victoria</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<style>

:root{
--navy:#0B1F3A;
--cyan:#2ED3E6;
--white:#FFFFFF;
--gold:#FFD54A;
--gray:#f4f7fa;
}

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
}

body{
background:var(--white);
color:#222;
}

header{
background:var(--navy);
padding:15px 8%;
display:flex;
justify-content:space-between;
align-items:center;
position:sticky;
top:0;
z-index:999;
}

.logo{
display:flex;
align-items:center;
gap:10px;
}

.logo img{
width:70px;
}

.logo h1{
color:white;
}

nav a{
color:white;
text-decoration:none;
margin:0 12px;
font-weight:500;
transition:.3s;
}

nav a:hover{
color:var(--cyan);
}

.hero{
height:90vh;
display:flex;
align-items:center;
justify-content:center;
text-align:center;
background:linear-gradient(135deg,var(--navy),#123b70);
color:white;
padding:20px;
}

.hero-content{
max-width:900px;
}

.hero h2{
font-size:4rem;
margin-bottom:20px;
}

.hero p{
font-size:1.2rem;
margin-bottom:25px;
}

.btn{
background:var(--cyan);
padding:15px 30px;
border:none;
border-radius:30px;
color:white;
font-size:1rem;
cursor:pointer;
transition:.3s;
}

.btn:hover{
transform:translateY(-4px);
background:var(--gold);
color:black;
}

section{
padding:80px 8%;
}

.section-title{
text-align:center;
font-size:2.5rem;
color:var(--navy);
margin-bottom:50px;
}

.products{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
gap:30px;
}

.card{
background:white;
border-radius:20px;
overflow:hidden;
box-shadow:0 8px 20px rgba(0,0,0,.08);
transition:.4s;
}

.card:hover{
transform:translateY(-10px);
}

.card img{
width:100%;
height:250px;
object-fit:cover;
}

.card-content{
padding:20px;
}

.price{
color:var(--cyan);
font-size:1.3rem;
font-weight:700;
}

.favorite{
background:var(--gold);
border:none;
padding:8px 15px;
border-radius:20px;
cursor:pointer;
margin-top:10px;
}

.filters{
display:flex;
flex-wrap:wrap;
gap:15px;
justify-content:center;
margin-bottom:40px;
}

.filters select{
padding:12px;
border:1px solid #ddd;
border-radius:10px;
}

.featured{
background:var(--gray);
}

.story{
display:grid;
grid-template-columns:1fr 1fr;
gap:40px;
align-items:center;
}

.story img{
width:100%;
border-radius:20px;
}

.reviews{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:25px;
}

.review{
padding:25px;
background:white;
box-shadow:0 4px 15px rgba(0,0,0,.08);
border-radius:15px;
}

.faq details{
margin-bottom:15px;
background:#f5f5f5;
padding:15px;
border-radius:10px;
}

.contact{
background:var(--navy);
color:white;
text-align:center;
}

.contact a{
color:var(--cyan);
text-decoration:none;
}

.cart{
position:fixed;
right:20px;
bottom:20px;
background:var(--gold);
padding:15px;
border-radius:50%;
font-size:25px;
cursor:pointer;
box-shadow:0 5px 15px rgba(0,0,0,.3);
}

footer{
background:#071426;
color:white;
padding:30px;
text-align:center;
}

.socials a{
margin:0 10px;
color:white;
font-size:1.2rem;
text-decoration:none;
}

@media(max-width:768px){

.hero h2{
font-size:2.5rem;
}

.story{
grid-template-columns:1fr;
}

}

</style>
</head>

<body>

<header>

<div class="logo">
<img src="logo.png" alt="ShoeUma">
<h1>ShoeUma</h1>
</div>

<nav>
<a href="#inicio">Inicio</a>
<a href="#catalogo">Catálogo</a>
<a href="#destacados">Destacados</a>
<a href="#historia">Historia</a>
<a href="#opiniones">Opiniones</a>
<a href="#faq">FAQ</a>
<a href="#contacto">Contacto</a>
</nav>

</header>

<section class="hero" id="inicio">

<div class="hero-content">

<h2>El eclipse primero. Todo lo demás, después.</h2>

<p>
Zapatos deportivos inspirados en Uma Musume Pretty Derby.
Diseñados para corredores, coleccionistas y amantes del anime.
</p>

<button class="btn">Explorar Catálogo</button>

</div>

</section>

<section id="catalogo">

<h2 class="section-title">Catálogo de Productos</h2>

<div class="filters">

<select>
<option>Diseño</option>
<option>Special Week</option>
<option>Tokai Teio</option>
<option>Silence Suzuka</option>
<option>Gold Ship</option>
</select>

<select>
<option>Talla</option>
<option>24</option>
<option>25</option>
<option>26</option>
<option>27</option>
<option>28</option>
</select>

<select>
<option>Precio</option>
<option>$29.99 - $35</option>
<option>$35 - $45</option>
<option>$45 - $50</option>
</select>

</div>

<div class="products">

<div class="card">
<img src="https://picsum.photos/400/300?1">
<div class="card-content">
<h3>Special Week Runner</h3>
<p class="price">$39.99</p>

<label>Talla:</label>
<select>
<option>24</option>
<option>25</option>
<option>26</option>
<option>27</option>
</select>

<br><br>

<button class="btn">Añadir al carrito</button>
<button class="favorite">❤ Favorito</button>

</div>
</div>

<div class="card">
<img src="https://picsum.photos/400/300?2">
<div class="card-content">
<h3>Tokai Teio Speed</h3>
<p class="price">$44.99</p>

<label>Talla:</label>
<select>
<option>24</option>
<option>25</option>
<option>26</option>
<option>27</option>
</select>

<br><br>

<button class="btn">Añadir al carrito</button>
<button class="favorite">❤ Favorito</button>

</div>
</div>

<div class="card">
<img src="https://picsum.photos/400/300?3">
<div class="card-content">
<h3>Silence Suzuka Pro</h3>
<p class="price">$49.99</p>

<label>Talla:</label>
<select>
<option>24</option>
<option>25</option>
<option>26</option>
<option>27</option>
</select>

<br><br>

<button class="btn">Añadir al carrito</button>
<button class="favorite">❤ Favorito</button>

</div>
</div>

</div>

</section>

<section class="featured" id="destacados">

<h2 class="section-title">Modelos Destacados</h2>

<p style="text-align:center;">
Los modelos más populares de la colección ShoeUma incorporan
tecnología de amortiguación, materiales ligeros y diseños inspirados
en las corredoras legendarias de Uma Musume.
</p>

</section>

<section id="historia">

<h2 class="section-title">Historia e Inspiración</h2>

<div class="story">

<div>

<p>
ShoeUma nace de la pasión por el running y la franquicia Uma Musume
Pretty Derby. Nuestro objetivo es combinar el rendimiento deportivo
con diseños inspirados en personajes icónicos de las carreras,
permitiendo que cada corredor exprese su estilo mientras alcanza
nuevas metas.
</p>

</div>

<div>
<img src="https://picsum.photos/700/500">
</div>

</div>

</section>

<section id="opiniones">

<h2 class="section-title">Opiniones de Clientes</h2>

<div class="reviews">

<div class="review">
⭐⭐⭐⭐⭐
<p>Excelente comodidad y diseño espectacular.</p>
</div>

<div class="review">
⭐⭐⭐⭐⭐
<p>Perfectos para correr y para coleccionar.</p>
</div>

<div class="review">
⭐⭐⭐⭐
<p>Muy ligeros y llamativos.</p>
</div>

</div>

</section>

<section id="faq">

<h2 class="section-title">Preguntas Frecuentes</h2>

<div class="faq">

<details>
<summary>¿Realizan envíos internacionales?</summary>
<p>Sí, enviamos a la mayoría de países.</p>
</details>

<details>
<summary>¿Qué métodos de pago aceptan?</summary>
<p>Tarjeta, PayPal, Google Pay y Apple Pay.</p>
</details>

<details>
<summary>¿Cómo elijo mi talla?</summary>
<p>Utiliza el selector de talla incluido en cada producto.</p>
</details>

</div>

</section>

<section>

<h2 class="section-title">Métodos de Pago y Envíos</h2>

<p style="text-align:center;">
Visa, Mastercard, PayPal, Google Pay y Apple Pay.
Envíos nacionales e internacionales con seguimiento.
</p>

</section>

<section class="contact" id="contacto">

<h2>Contacto</h2>

<br>

<p>WhatsApp: 1701377872</p>

<p>
Correo:
<a href="mailto:umashoe@gmail.com">
umashoe@gmail.com
</a>
</p>

<br>

<div class="socials">
<a href="#">Instagram</a>
<a href="#">TikTok</a>
<a href="#">Facebook</a>
<a href="#">X</a>
</div>

</section>

<div class="cart">
🛒
</div>

<footer>

<p>© 2026 ShoeUma. Todos los derechos reservados.</p>

<p>Donde la velocidad encuentra el estilo.</p>

</footer>

</body>
</html>