<!DOCTYPE html>
<html>
<head>
<title>Sweet Bakery</title>

<style>

body{
font-family: Arial, sans-serif;
margin:0;
background:#fff5e6;
text-align:center;
}

header{
background:#ff7a59;
color:white;
padding:20px;
}

.products{
display:flex;
justify-content:center;
flex-wrap:wrap;
margin:30px;
}

.card{
background:white;
width:220px;
margin:15px;
padding:20px;
border-radius:10px;
box-shadow:0 4px 10px rgba(0,0,0,0.2);
}

.price{
font-size:20px;
color:green;
margin:10px;
}

button{
background:#ff7a59;
color:white;
border:none;
padding:10px 15px;
border-radius:5px;
cursor:pointer;
}

button:hover{
background:#ff4d2d;
}

.order{
background:white;
width:320px;
margin:40px auto;
padding:20px;
border-radius:10px;
box-shadow:0 4px 10px rgba(0,0,0,0.2);
}

input, select{
width:90%;
padding:8px;
margin:8px;
}

footer{
background:#333;
color:white;
padding:15px;
margin-top:40px;
}

</style>

</head>

<body>

<header>
<h1>Sweet Bakery 🍰</h1>
<p>Fresh & Delicious Bakery Items</p>
</header>

<div class="products">

<div class="card">
<h2>Pizza 🍕</h2>
<p class="price">₹50</p>
<button onclick="order('Pizza')">Order</button>
</div>

<div class="card">
<h2>Cake 🎂</h2>
<p class="price">₹40</p>
<button onclick="order('Cake')">Order</button>
</div>

<div class="card">
<h2>Cup Cake 🧁</h2>
<p class="price">₹30</p>
<button onclick="order('Cup Cake')">Order</button>
</div>

<div class="card">
<h2>Pudding 🍮</h2>
<p class="price">₹40</p>
<button onclick="order('Pudding')">Order</button>
</div>

</div>

<div class="order">

<h2>Place Your Order</h2>

<input type="text" placeholder="Your Name"><br>

<select id="product">
<option>Select Product</option>
<option>Pizza</option>
<option>Cake</option>
<option>Cup Cake</option>
<option>Pudding</option>
</select><br>

<input type="number" placeholder="Quantity"><br>

<input type="text" placeholder="Address"><br>

<button onclick="submitOrder()">Submit Order</button>

<p id="message"></p>

</div>

<footer>
<p>© 2026 Sweet Bakery</p>
</footer>

<script>

function order(item){
document.getElementById("product").value=item;
}

function submitOrder(){
document.getElementById("message").innerHTML="✅ Your order has been placed!";
}

</script>

</body>
</html># Ccc
