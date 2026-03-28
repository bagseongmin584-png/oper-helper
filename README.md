index.html
<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>AI 운영 도우미</title>

<style>
body {
font-family: Arial;
background:#0f172a;
color:white;
padding:20px;
}

.card {
background:#1e293b;
padding:20px;
border-radius:10px;
margin-bottom:15px;
}

button {
background:#3b82f6;
border:none;
padding:10px;
border-radius:8px;
color:white;
width:100%;
margin-top:10px;
}

input {
width:100%;
padding:10px;
margin-top:10px;
border-radius:8px;
border:none;
}

</style>

</head>

<body>

<h2>🚀 AI 자동 운영 도우미</h2>

<div class="card">
<h3>수익 아이디어 생성</h3>
<button onclick="generate()">아이디어 생성</button>
<p id="idea"></p>
</div>

<div class="card">
<h3>자동 콘텐츠 생성</h3>
<input placeholder="주제 입력" id="topic">
<button onclick="content()">생성</button>
<p id="result"></p>
</div>

<script>

function generate(){

const ideas = [
"AI 자동 블로그 운영",
유튜브 자동 쇼츠 채널,
AI 뉴스 자동 생성,
AI 상품 추천 자동화,
AI 블로그 자동 수익화
]

document.getElementById("idea").innerText =
ideas[Math.floor(Math.random()*ideas.length)]

}

function content(){

let topic =
document.getElementById("topic").value

document.getElementById("result").innerText =
topic + " 자동 콘텐츠 생성 완료"

}

</script>

</body>
</html>
