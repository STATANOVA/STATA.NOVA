<!DOCTYPE html>
<html lang="ar">
<head>
<meta charset="UTF-8">
<title>صفحاتي</title>

<style>
body {
    font-family: Arial;
    direction: rtl;
    padding: 20px;
}
h1 {
    text-align: center;
}
.grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
    gap: 10px;
}
a {
    padding: 10px;
    background: #f2f2f2;
    text-align: center;
    text-decoration: none;
    border-radius: 8px;
}
a:hover {
    background: #ddd;
}
</style>

</head>

<body>

<h1>📊 جميع الصفحات</h1>

<div class="grid" id="links"></div>

<script>
let totalPages = 100; // نبدأ بـ 100 للتجربة

let container = document.getElementById("links");

for (let i = 1; i <= totalPages; i++) {
    let a = document.createElement("a");
    a.href = "pages/page" + i + ".html";
    a.textContent = "صفحة " + i;
    container.appendChild(a);
}
</script>

</body>
</html>
