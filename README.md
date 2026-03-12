# SS.Lipan-Art
Website for SS Lipan Art – Handmade lipan art products
<!DOCTYPE html>
<html>
<head>
<title>SS Lipan Art</title>
<meta name="viewport" content="width=device-width, initial-scale=1">

<style>

body{
font-family:Arial;
margin:0;
background:linear-gradient(120deg,#ff9a9e,#fad0c4,#fbc2eb);
}

header{
background:#7b2cbf;
color:white;
padding:25px;
text-align:center;
}

nav{
background:#ffb703;
padding:10px;
text-align:center;
}

nav a{
margin:15px;
text-decoration:none;
font-weight:bold;
color:black;
}

.container{
padding:20px;
}

.product{
background:white;
border-radius:12px;
padding:15px;
margin:20px 0;
box-shadow:0 5px 15px rgba(0,0,0,0.2);
}

.product img{
width:100%;
max-width:250px;
border-radius:10px;
}

button{
padding:10px 15px;
margin:5px;
border:none;
border-radius:5px;
cursor:pointer;
}

.cart{
background:#2a9d8f;
color:white;
}

.fav{
background:#e63946;
color:white;
}

.pay{
background:#264653;
color:white;
}

#cart{
background:white;
padding:15px;
border-radius:10px;
margin-top:20px;
}

.review{
background:white;
padding:15px;
margin:10px 0;
border-radius:10px;
}

footer{
background:#333;
color:white;
text-align:center;
padding:15px;
}

</style>

</head>

<body>

<header>
<h1>SS Lipan Art</h1>
<p>Handmade Lipan Art & Craft</p>
</header>

<nav>
<a href="#about">About</a>
<a href="#products">Products</a>
<a href="#cart">Cart</a>
<a href="#reviews">Reviews</a>
</nav>

<div class="container">

<h2 id="about">About Lipan Art</h2>

<p>
Lipan Art is a traditional clay and mirror craft from the Kutch region of Gujarat, India. 
It is made by creating patterns using clay and decorating them with mirrors. 
Traditionally used to decorate village homes, Lipan art has now become a popular form of 
wall decoration, name plates, and customized gifts.
</p>

<h2 id="products">Products</h2>

<div class="product">
<img src="birthday.jpg">
<h3>Birthday Customized Art</h3>
<p>Size: 12x12 inch</p>
<p>Price: ₹700</p>

<button class="cart" onclick="addToCart('Birthday Art',700)">Add to Cart</button>
<button class="fav">❤ Favourite</button>

</div>

<div class="product">
<img src="anniversary.jpg">
<h3>Anniversary Art</h3>
<p>Size: 12x12 inch</p>
<p>Price: ₹750</p>

<button class="cart" onclick="addToCart('Anniversary Art',750)">Add to Cart</button>
<button class="fav">❤ Favourite</button>

</div>

<div class="product">
<img src="nameplate.jpg">
<h3>Name Plate</h3>
<p>Size: 10x10 inch</p>
<p>Price: ₹500</p>

<button class="cart" onclick="addToCart('Name Plate',500)">Add to Cart</button>
<button class="fav">❤ Favourite</button>

</div>

<div class="product">
<img src="jagannath.jpg">
<h3>Jagannath Lipan Art</h3>
<p>Size: 12x12 inch</p>
<p>Price: ₹900</p>

<button class="cart" onclick="addToCart('Jagannath Art',900)">Add to Cart</button>
<button class="fav">❤ Favourite</button>

</div>

<div class="product">
<img src="keychain.jpg">
<h3>Lipan Keychain</h3>
<p>Price: ₹150</p>

<button class="cart" onclick="addToCart('Keychain',150)">Add to Cart</button>
<button class="fav">❤ Favourite</button>

</div>

<h2 id="cart">Shopping Cart</h2>

<div id="cart">
<p>No items added</p>
</div>

<h2>Payment</h2>

<p>Pay using Google Pay or PhonePe</p>

<a href="upi://pay?pa=yourupi@upi&pn=SSLipanArt">
<button class="pay">Pay Now</button>
</a>

<h2 id="reviews">Customer Reviews</h2>

<div class="review">
⭐⭐⭐⭐⭐ Amazing handmade work!
</div>

<div class="review">
⭐⭐⭐⭐ Beautiful craft and perfect gift.
</div>

<div class="review">
⭐⭐⭐⭐⭐ Loved the mirror design.
</div>

</div>

<footer>

<p>© 2026 SS Lipan Art</p>

</footer>

<script>

let cart=[];

function addToCart(product,price){

cart.push({product,price});

let cartHTML="";

let total=0;

cart.forEach(item=>{
cartHTML+= item.product+" - ₹"+item.price+"<br>";
total+=item.price;
});

cartHTML+="<br><b>Total: ₹"+total+"</b>";

document.getElementById("cart").innerHTML=cartHTML;

}

</script>

</body>
</html>
