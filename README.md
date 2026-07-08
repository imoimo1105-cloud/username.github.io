<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<title>野獣先輩保護協会</title>
<style>
body{
    background:#111;
    color:white;
    font-family:sans-serif;
    text-align:center;
}
.box{
    margin:50px auto;
    width:600px;
    background:#222;
    border:4px solid red;
    padding:20px;
    border-radius:10px;
}
h1{
    color:red;
    font-size:40px;
}
button{
    padding:15px 40px;
    font-size:20px;
    background:red;
    color:white;
    border:none;
    cursor:pointer;
}
button:hover{
    background:darkred;
}
.small{
    color:#aaa;
    font-size:12px;
    margin-top:20px;
}
</style><meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>

<div class="box">
<h1>⚠ 野獣先輩保護協会 ⚠</h1>

<h2>あなたは野獣先輩を見すぎました。</h2>

<p>
保護活動費として<br>
<b style="font-size:35px;color:yellow;">
114,514円
</b><br>
の請求が発生しました。
</p>

<button onclick="revealJoke()">支払う</button>

<p id="result"></p>

<p class="small">
※これはジョークサイトです。実際の請求ではありません。
</p>

</div>

<script>
function revealJoke(function revealJoke() {

    // 音を鳴らす
    const sound = document.getElementById("sound");
    sound.currentTime = 0;
    sound.play().catch(() => {});

    // スマホ対応の短いバイブレーション
    if ("vibrate" in navigator) {
        navigator.vibrate(200);
    }

    // 以下は今までのカウントダウン
    const result = document.getElementById("result");
    let count = 5;

    result.innerHTML = `
        <h2>請求処理中...</h2>
        <h1 id="count">${count}</h1>
    `;

    const timer = setInterval(() => {
        count--;

        if (count > 0) {
            document.getElementById("count").textContent = count;
        } else {
            clearInterval(timer);

            result.innerHTML = `
                <h1 style="color:lime;">😂 ドッキリ成功！😂</h1>
                <p>これはジョークサイトです！</p>
            `;
        }
    }, 1000);
}){
    document.getElementById("result").innerHTML =
    "<h2>😎 ドッキリ成功！</h2><p>もちろん請求なんてありません！</p>";
}
</script>

</body><audio id="sound" src="yaju-u.mp3" preload="auto"></audio>
</html>index.html
yaju-u.mp3
<script>
function revealJoke(){

    const result = document.getElementById("result");
    let count = 5;

    result.innerHTML = `<h2>請求処理中...</h2><h1 id="count">${count}</h1>`;

    const timer = setInterval(() => {
        count--;

        if(count > 0){
            document.getElementById("count").innerText = count;
        }else{
            clearInterval(timer);

            result.innerHTML = `
            <h1 style="color:lime;">😂 ドッキリ成功！ 😂</h1>
            <h2>野獣先輩保護協会なんてありません！</h2>
            <p>もちろん請求もありません！</p>
            `;
        }

    },1000);
theme: jekyll-theme-minimal
title: Octocat's homepage
description: Bookmark this to keep an eye on my project updates!
