# daily-quotes
<!DOCTYPE html>
<html lang="ar">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Daily Quotes - اقتباسات يومية</title>
<style>
body {
font-family: Arial, sans-serif;
background: #f0f0f0;
display: flex;
justify-content: center;
align-items: center;
height: 100vh;
margin: 0;
}
.container {
background: #fff;
padding: 30px;
border-radius: 10px;
box-shadow: 0 5px 15px rgba(0,0,0,0.2);
text-align: center;
max-width: 400px;
}
h1 {
font-size: 24px;
margin-bottom: 20px;
color: #333;
}
p {
font-size: 18px;
margin: 20px 0;
color: #555;
}
button {
padding: 10px 20px;
font-size: 16px;
background: #007bff;
color: #fff;
border: none;
border-radius: 5px;
cursor: pointer;
}
button:hover {
background: #0056b3;
}
</style>
</head>
<body>
<div class="container">
<h1>اقتباس اليوم</h1>
<p id="quote">اضغط على الزر لإظهار اقتباس</p>
<button onclick="showQuote()">اقتباس جديد</button>
</div>

<script>
const quotes = [
"الإصرار يصنع المستحيل.",
"لا تنتظر الفرصة، اصنعها.",
"العقل زينة، فزينه بالعلم.",
"كل يوم هو بداية جديدة.",
"الثقة بالنفس مفتاح النجاح.",
"الفشل هو خطوة نحو النجاح.",
"ابتسم، الحياة قصيرة."
];

function showQuote() {
const randomIndex = Math.floor(Math.random() * quotes.length);
document.getElementById('quote').textContent = quotes[randomIndex];
}
</script>
</body>
</html>
