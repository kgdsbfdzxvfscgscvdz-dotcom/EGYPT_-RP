<!DOCTYPE html>
<html lang="ar" dir="rtl">

<head>

<meta charset="UTF-8">

<meta
name="viewport"
content="width=device-width, initial-scale=1.0"
>

<meta
name="theme-color"
content="#08070d"
>

<title>Egypt RP | التقديم</title>

<style>

*{
box-sizing:border-box;
margin:0;
padding:0;
-webkit-tap-highlight-color:transparent;
}

:root{
--bg:#07060b;
--card:#12101b;
--card2:#181423;
--pink:#ff0059;
--purple:#a900ff;
--text:#fff;
--muted:#aaa3b5;
--border:rgba(255,255,255,.09);
}

body{
min-height:100vh;
font-family:Tahoma,Arial,sans-serif;
color:white;
background:
radial-gradient(
circle at 50% -10%,
rgba(169,0,255,.25),
transparent 35%
),
radial-gradient(
circle at 0 40%,
rgba(255,0,89,.12),
transparent 30%
),
#07060b;
}

button,
input,
textarea{
font:inherit;
}

button{
cursor:pointer;
}

.container{
width:min(920px,92%);
margin:auto;
}

.hidden{
display:none!important;
}

/* HEADER */

header{
position:sticky;
top:0;
z-index:20;
background:rgba(7,6,11,.82);
backdrop-filter:blur(18px);
border-bottom:1px solid var(--border);
}

.nav{
height:70px;
display:flex;
align-items:center;
justify-content:space-between;
}

.logo{
font-size:23px;
font-weight:1000;
}

.logo span{
background:
linear-gradient(
90deg,
#ff0059,
#a900ff
);
-webkit-background-clip:text;
color:transparent;
}

.status{
padding:8px 13px;
border-radius:999px;
font-size:12px;
background:rgba(0,255,120,.06);
border:1px solid rgba(0,255,120,.2);
color:#9dffc8;
}

/* HERO */

.hero{
text-align:center;
padding:80px 0 45px;
}

.badge{
display:inline-block;
padding:9px 17px;
border-radius:999px;
background:rgba(255,255,255,.035);
border:1px solid rgba(255,0,89,.25);
color:#ddd;
font-size:13px;
}

.hero h1{
font-size:clamp(42px,9vw,76px);
line-height:1.05;
margin:24px 0 18px;
font-weight:1000;
}

.gradient{
background:
linear-gradient(
90deg,
#ff0059,
#a900ff
);
-webkit-background-clip:text;
color:transparent;
}

.hero p{
max-width:680px;
margin:auto;
color:var(--muted);
line-height:2;
font-size:15px;
}

/* BUTTON */

.actions{
display:flex;
justify-content:center;
gap:12px;
flex-wrap:wrap;
margin-top:28px;
}

.btn{
border:1px solid var(--border);
background:rgba(255,255,255,.04);
color:white;
padding:14px 25px;
border-radius:15px;
font-weight:900;
transition:.2s;
}

.btn:hover{
transform:translateY(-3px);
}

.primary{
border:0;
background:
linear-gradient(
110deg,
#ff0059,
#a900ff
);
box-shadow:
0 15px 40px
rgba(255,0,89,.18);
}

/* CARD */

.card{
margin:25px 0;
padding:30px;
border-radius:27px;
background:
linear-gradient(
145deg,
rgba(27,22,41,.92),
rgba(11,9,17,.95)
);
border:1px solid var(--border);
box-shadow:
0 25px 80px
rgba(0,0,0,.28);
}

.title{
font-size:25px;
font-weight:1000;
margin-bottom:8px;
}

.desc{
color:var(--muted);
font-size:14px;
line-height:1.9;
margin-bottom:22px;
}

/* RULES */

.rules{
display:grid;
gap:11px;
}

.rule{
display:flex;
align-items:flex-start;
gap:12px;
padding:15px;
border-radius:16px;
background:rgba(255,255,255,.025);
border:1px solid rgba(255,255,255,.06);
}

.rule-number{
width:34px;
height:34px;
min-width:34px;
display:grid;
place-items:center;
border-radius:10px;
font-weight:1000;
background:
linear-gradient(
135deg,
#ff0059,
#a900ff
);
}

.rule-text{
color:#ddd;
line-height:1.8;
font-size:14px;
}

.agreement{
display:flex;
align-items:flex-start;
gap:11px;
margin-top:20px;
padding:16px;
border-radius:16px;
background:rgba(169,0,255,.05);
border:1px solid rgba(169,0,255,.2);
cursor:pointer;
}

.agreement input{
width:20px;
height:20px;
accent-color:#a900ff;
margin-top:3px;
}

.agreement span{
color:#ddd;
line-height:1.8;
font-size:14px;
}

/* FORM */

.field{
margin-bottom:19px;
}

label{
display:block;
margin-bottom:8px;
font-weight:900;
}

input,
textarea{
width:100%;
background:#09080e;
color:white;
border:1px solid rgba(255,255,255,.1);
border-radius:15px;
padding:15px;
outline:none;
}

input:focus,
textarea:focus{
border-color:#a900ff;
box-shadow:
0 0 0 4px
rgba(169,0,255,.07);
}

textarea{
min-height:170px;
resize:vertical;
}

/* QUIZ */

.progress-top{
display:flex;
justify-content:space-between;
align-items:center;
margin-bottom:11px;
}

.counter{
color:#aaa;
font-size:14px;
}

.timer{
font-size:26px;
font-weight:1000;
color:#ff1762;
}

.progress{
height:9px;
background:#292330;
border-radius:999px;
overflow:hidden;
margin-bottom:27px;
}

.progress-bar{
height:100%;
background:
linear-gradient(
90deg,
#ff0059,
#a900ff
);
transition:.3s;
}

.q-number{
font-size:13px;
font-weight:1000;
color:#ff1762;
}

.question{
font-size:clamp(22px,5vw,31px);
line-height:1.7;
font-weight:900;
margin:10px 0 20px;
}

.note{
font-size:12px;
color:#817b89;
margin-top:8px;
}

.form-actions{
display:flex;
justify-content:space-between;
gap:10px;
margin-top:24px;
}

/* REVIEW */

.review-item{
padding:16px 0;
border-bottom:1px solid var(--border);
}

.review-item:last-child{
border-bottom:0;
}

.review-q{
font-weight:1000;
margin-bottom:7px;
}

.review-a{
color:#c9c2d2;
white-space:pre-wrap;
line-height:1.8;
}

/* SUCCESS */

.success{
text-align:center;
padding:65px 25px;
}

.success-icon{
width:90px;
height:90px;
margin:0 auto 22px;
display:grid;
place-items:center;
border-radius:50%;
font-size:44px;
font-weight:1000;
background:
linear-gradient(
135deg,
#ff0059,
#a900ff
);
box-shadow:
0 20px 60px
rgba(169,0,255,.2);
}

.application-id{
display:inline-block;
margin-top:15px;
padding:10px 15px;
border-radius:10px;
background:rgba(255,255,255,.05);
font-family:monospace;
color:#ddd;
}

/* LOADING */

.loading{
display:none;
text-align:center;
color:#aaa;
margin-top:16px;
}

.spinner{
display:inline-block;
width:18px;
height:18px;
border:3px solid rgba(255,255,255,.15);
border-top-color:#ff0059;
border-radius:50%;
animation:spin .7s linear infinite;
vertical-align:middle;
margin-left:7px;
}

@keyframes spin{
to{
transform:rotate(360deg);
}
}

/* FOOTER */

footer{
text-align:center;
padding:40px 0;
color:#777181;
}

.small{
font-size:12px;
}

/* MOBILE */

@media(max-width:600px){

.nav{
height:64px;
}

.status{
display:none;
}

.hero{
padding:55px 0 30px;
}

.hero h1{
font-size:42px;
}

.card{
padding:21px;
border-radius:22px;
}

.form-actions{
flex-direction:column;
}

.form-actions .btn{
width:100%;
}

.question{
font-size:22px;
}

}

</style>

</head>

<body>

<header>

<div class="container nav">

<div class="logo">
<span>EGYPT</span> RP 🇪🇬
</div>

<div class="status">
● نظام التقديم
</div>

</div>

</header>

<main class="container">

<!-- HOME -->

<section id="home">

<div class="hero">

<div class="badge">
🇪🇬 مدينة Egypt RP
</div>

<h1>
ابدأ قصتك داخل
<br>
<span class="gradient">
Egypt RP
</span>
</h1>

<p>
مدينة متكاملة لعشاق الـ RolePlay،
أحداث، شرطة، عصابات، وظائف وفعاليات.
اقرأ القوانين وابدأ التقديم.
</p>

<div class="actions">

<button
class="btn primary"
onclick="startApplication()"
>
📋 ابدأ التقديم
</button>

</div>

</div>

</section>

<!-- RULES -->

<section
id="rules"
class="card hidden"
>

<div class="title">
📜 قوانين التقديم
</div>

<div class="desc">
اقرأ القوانين بالكامل قبل البدء.
استمرارك يعني موافقتك عليها.
</div>

<div class="rules">

<div class="rule">
<div class="rule-number">1</div>
<div class="rule-text">
الالتزام بقوانين الـ RolePlay داخل السيرفر.
</div>
</div>

<div class="rule">
<div class="rule-number">2</div>
<div class="rule-text">
ممنوع الغش أو استغلال الثغرات.
</div>
</div>

<div class="rule">
<div class="rule-number">3</div>
<div class="rule-text">
ممنوع RDM و VDM وأي تصرف يفسد تجربة اللاعبين.
</div>
</div>

<div class="rule">
<div class="rule-number">4</div>
<div class="rule-text">
احترام اللاعبين والإدارة.
</div>
</div>

<div class="rule">
<div class="rule-number">5</div>
<div class="rule-text">
ممنوع MetaGaming واستخدام معلومات خارج الـ RP.
</div>
</div>

<div class="
