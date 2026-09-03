<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1.0">
<meta name="theme-color" content="#08070d">
<title>Egypt RP | التقديم</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial,Tahoma,sans-serif;
}

html{
    scroll-behavior:smooth;
}

body{
    min-height:100vh;
    color:#fff;
    background:
        radial-gradient(circle at 20% 20%,rgba(185,0,255,.18),transparent 30%),
        radial-gradient(circle at 80% 80%,rgba(255,0,120,.12),transparent 30%),
        #07070b;
}

button,input,textarea{
    font:inherit;
}

button{
    cursor:pointer;
}

.hidden{
    display:none!important;
}

header{
    position:sticky;
    top:0;
    z-index:50;
    background:rgba(7,7,11,.88);
    backdrop-filter:blur(15px);
    border-bottom:1px solid rgba(255,255,255,.08);
}

.nav{
    max-width:1100px;
    margin:auto;
    padding:18px 20px;
    display:flex;
    align-items:center;
    justify-content:space-between;
    gap:15px;
}

.logo{
    font-size:22px;
    font-weight:900;
    letter-spacing:1px;
}

.logo span{
    color:#c000ff;
}

.discord-link{
    text-decoration:none;
    color:#fff;
    background:linear-gradient(135deg,#5865f2,#4752c4);
    padding:11px 18px;
    border-radius:12px;
    font-weight:bold;
    transition:.2s;
}

.discord-link:hover{
    transform:translateY(-2px);
}

.container{
    width:min(1100px,calc(100% - 30px));
    margin:auto;
}

.hero{
    min-height:72vh;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    text-align:center;
    padding:50px 0;
}

.badge{
    display:inline-block;
    padding:8px 14px;
    border-radius:50px;
    background:rgba(191,0,255,.1);
    border:1px solid rgba(191,0,255,.35);
    color:#d97aff;
    margin-bottom:20px;
}

.hero h1{
    font-size:clamp(48px,9vw,90px);
    font-weight:1000;
    background:linear-gradient(90deg,#fff,#d55cff,#ff4db8);
    -webkit-background-clip:text;
    color:transparent;
}

.hero p{
    color:#aaa;
    font-size:18px;
    margin:15px 0 30px;
}

.btn{
    border:0;
    border-radius:14px;
    padding:14px 24px;
    color:white;
    font-weight:900;
    transition:.2s;
}

.btn:hover{
    transform:translateY(-2px);
}

.primary{
    background:linear-gradient(135deg,#b000ff,#ff168c);
    box-shadow:0 10px 30px rgba(190,0,255,.2);
}

.discord{
    background:#5865f2;
}

.secondary{
    background:#202027;
}

.danger{
    background:#d71945;
}

.success{
    background:#13a86b;
}

.card{
    background:rgba(16,15,22,.9);
    border:1px solid rgba(255,255,255,.08);
    border-radius:22px;
    padding:25px;
    margin:30px auto;
    box-shadow:0 20px 70px rgba(0,0,0,.25);
}

.title{
    font-size:28px;
    font-weight:900;
    margin-bottom:10px;
}

.subtitle{
    color:#999;
    margin-bottom:22px;
}

.rules{
    display:grid;
    gap:12px;
    margin:20px 0;
}

.rule{
    background:#111017;
    border:1px solid rgba(255,255,255,.07);
    border-radius:14px;
    padding:15px;
    color:#ddd;
}

.agreement{
    display:flex;
    align-items:center;
    gap:10px;
    padding:15px;
    border-radius:14px;
    background:#111017;
    margin:20px 0;
    cursor:pointer;
}

.agreement input{
    width:20px;
    height:20px;
    accent-color:#c000ff;
}

.actions{
    display:flex;
    flex-wrap:wrap;
    gap:10px;
}

.form-grid{
    display:grid;
    grid-template-columns:repeat(2,1fr);
    gap:15px;
}

.field{
    display:flex;
    flex-direction:column;
    gap:8px;
}

.field.full{
    grid-column:1/-1;
}

label{
    color:#ddd;
    font-weight:bold;
}

input,textarea{
    width:100%;
    background:#0c0b10;
    color:white;
    border:1px solid #292631;
    border-radius:12px;
    padding:14px;
    outline:none;
}

input:focus,textarea:focus{
    border-color:#bd00ff;
    box-shadow:0 0 0 3px rgba(189,0,255,.08);
}

textarea{
    min-height:120px;
    resize:vertical;
}

.question{
    margin-top:18px;
    padding:20px;
    border-radius:18px;
    background:#0d0c12;
    border:1px solid rgba(255,255,255,.07);
}

.question-number{
    color:#c85aff;
    font-size:13px;
    margin-bottom:7px;
}

.question h3{
    font-size:18px;
    margin-bottom:12px;
}

.timer{
    position:sticky;
    top:75px;
    z-index:10;
    background:#15121c;
    border:1px solid #30283b;
    padding:12px;
    border-radius:12px;
    text-align:center;
    margin-bottom:15px;
}

.timer strong{
    color:#ff54b8;
}

.progress{
    height:7px;
    background:#222027;
    border-radius:10px;
    overflow:hidden;
    margin:15px 0;
}

.progress-bar{
    height:100%;
    width:0%;
    background:linear-gradient(90deg,#a900ff,#ff299e);
    transition:.2s;
}

.review-item{
    background:#100f15;
    border:1px solid #25222d;
    border-radius:15px;
    padding:15px;
    margin:10px 0;
}

.review-q{
    color:#d264ff;
    font-weight:bold;
    margin-bottom:8px;
}

.review-a{
    color:#ddd;
    white-space:pre-wrap;
}

.success-box{
    text-align:center;
    padding:60px 20px;
}

.success-icon{
    font-size:70px;
    margin-bottom:15px;
}

.application-id{
    display:inline-block;
    margin:20px 0;
    padding:12px 20px;
    border-radius:12px;
    background:#100d15;
    border:1px solid #3a2545;
    color:#df75ff;
    font-weight:bold;
}

.admin-login{
    max-width:500px;
    margin:60px auto;
}

.admin-list{
    display:grid;
    gap:15px;
}

.admin-card{
    background:#0e0d13;
    border:1px solid #292531;
    border-radius:18px;
    padding:20px;
}

.admin-head{
    display:flex;
    justify-content:space-between;
    gap:15px;
    align-items:center;
    flex-wrap:wrap;
    margin-bottom:15px;
}

.status{
    padding:7px 12px;
    border-radius:30px;
    font-size:13px;
    font-weight:bold;
}

.pending{
    background:#3b2e10;
    color:#ffd45c;
}

.accepted{
    background:#0d3929;
    color:#4dffb0;
}

.rejected{
    background:#3b101a;
    color:#ff6686;
}

.answer-box{
    margin-top:10px;
    padding:12px;
    background:#121017;
    border-radius:12px;
}

.answer-box b{
    color:#c965ff;
}

footer{
    text-align:center;
    color:#666;
    padding:40px 15px;
}

.toast{
    position:fixed;
    bottom:20px;
    left:50%;
    transform:translateX(-50%) translateY(100px);
    background:#18151f;
    border:1px solid #3b3045;
    padding:14px 20px;
    border-radius:12px;
    z-index:999;
    transition:.3s;
}

.toast.show{
    transform:translateX(-50%) translateY(0);
}

@media(max-width:700px){
    .form-grid{
        grid-template-columns:1fr;
    }

    .nav{
        padding:14px 10px;
    }

    .logo{
        font-size:18px;
    }

    .discord-link{
        padding:9px 12px;
        font-size:13px;
    }

    .card{
        padding:18px;
    }
}
</style>
</head>

<body>

<header>
    <div class="nav">
        <div class="logo">
            <span>EGYPT</span> RP 🇪🇬
        </div>

        <a
            class="discord-link"
            href="https://discord.gg/BkHAxZAMw"
            target="_blank"
        >
            💬 Discord
        </a>
    </div>
</header>

<main class="container">

<!-- HOME -->
<section id="home" class="hero">

    <div class="badge">🇪🇬 EGYPT RP • APPLICATION SYSTEM</div>

    <h1>EGYPT RP</h1>

    <p>
        أهلاً بيك في نظام التقديم الرسمي لسيرفر Egypt RP
    </p>

    <div class="actions">
        <button class="btn primary" onclick="showRules()">
            🚀 التقديم الآن
        </button>

        <a
            class="btn discord"
            href="https://discord.gg/BkHAxZAMw"
            target="_blank"
        >
            💬 دخول Discord
        </a>

        <button class="btn secondary" onclick="showAdminLogin()">
            🔐 الإدارة
        </button>
    </div>

</section>


<!-- RULES -->
<section id="rules" class="card hidden">

    <div class="title">📜 قوانين التقديم</div>

    <div class="subtitle">
        اقرأ القوانين بالكامل قبل بداية التقديم.
    </div>

    <div class="rules">

        <div class="rule">1️⃣ يجب الإجابة على جميع الأسئلة بجدية وبدون عشوائية.</div>

        <div class="rule">2️⃣ ممنوع استخدام إجابات منسوخة من شخص آخر.</div>

        <div class="rule">3️⃣ يجب الالتزام بقوانين الـRP داخل السيرفر.</div>

        <div class="rule">4️⃣ يمنع تقديم معلومات غير صحيحة.</div>

        <div class="rule">5️⃣ يجب أن تكون إجاباتك واضحة ومفهومة.</div>

        <div class="rule">6️⃣ الإدارة لها الحق في قبول أو رفض أي تقديم.</div>

        <div class="rule">7️⃣ التقديم أكثر من مرة بهدف تجاوز الرفض غير مسموح.</div>

        <div class="rule">8️⃣ أي محاولة غش أو تلاعب قد تؤدي إلى رفض التقديم.</div>

        <div class="rule">9️⃣ يجب الالتزام بآداب التعامل مع الإدارة وأعضاء السيرفر.</div>

        <div class="rule">🔟 إرسال التقديم يعني موافقتك على القوانين.</div>

    </div>

    <label class="agreement">
        <input type="checkbox" id="agreeRules" onchange="checkRules()">
        <span>قرأت القوانين بالكامل وأوافق عليها.</span>
    </label>

    <div class="actions">

        <button
            id="continueBtn"
            class="btn primary"
            onclick="startApplication()"
            disabled
        >
            🔒 وافق على القوانين أولاً
        </button>

        <button class="btn secondary" onclick="goHome()">
            رجوع
        </button>

    </div>

</section>


<!-- BASIC DATA -->
<section id="basic" class="card hidden">

    <div class="title">👤 بيانات المتقدم</div>

    <div class="subtitle">
        اكتب بياناتك بشكل صحيح.
    </div>

    <div class="form-grid">

        <div class="field">
            <label>الاسم</label>
            <input
                id="name"
                maxlength="50"
                placeholder="اكتب اسمك"
            >
        </div>

        <div class="field">
            <label>العمر</label>
            <input
                id="age"
                type="number"
                min="10"
                max="80"
                placeholder="اكتب عمرك"
            >
        </div>

        <div class="field full">
            <label>Discord Username</label>
            <input
                id="discord"
                maxlength="100"
                placeholder="مثال: username"
            >
        </div>

    </div>

    <br>

    <div class="actions">

        <button class="btn primary" onclick="startQuestions()">
            التالي ➜
        </button>

        <button class="btn secondary" onclick="showRules()">
            رجوع
        </button>

    </div>

</section>


<!-- QUESTIONS -->
<section id="questionsSection" class="card hidden">

    <div class="title">📝 أسئلة التقديم</div>

    <div class="subtitle">
        جاوب على الأسئلة التالية.
    </div>

    <div class="timer">
        ⏱️ الوقت المتبقي للسؤال:
        <strong id="timer">60</strong>
        ثانية
    </div>

    <div class="progress">
        <div id="progressBar" class="progress-bar"></div>
    </div>

    <div id="questions"></div>

    <div class="actions">

        <button
            id="reviewBtn"
            class="btn primary"
            onclick="showReview()"
        >
            📋 مراجعة التقديم
        </button>

    </div>

</section>


<!-- REVIEW -->
<section id="review" class="card hidden">

    <div class="title">🔎 مراجعة التقديم</div>

    <div class="subtitle">
        راجع إجاباتك قبل الإرسال.
    </div>

    <div id="reviewData"></div>

    <div class="actions">

        <button
            class="btn success"
            onclick="submitApplication()"
        >
            🚀 إرسال التقديم
        </button>

        <button
            class="btn secondary"
            onclick="backToQuestions()"
        >
            ✏️ تعديل الإجابات
        </button>

    </div>

</section>


<!-- SUCCESS -->
<section id="success" class="card hidden">

    <div class="success-box">

        <div class="success-icon">✅</div>

        <div class="title">
            تم إرسال التقديم بنجاح
        </div>

        <p class="subtitle">
            تم استلام طلبك وسيتم مراجعته من الإدارة.
        </p>

        <div class="application-id">
            رقم الطلب:
            <span id="applicationID"></span>
        </div>

        <br>

        <a
            class="btn discord"
            href="https://discord.gg/BkHAxZAMw"
            target="_blank"
        >
            💬 دخول Discord
        </a>

        <br><br>

        <button class="btn secondary" onclick="goHome()">
            🏠 الرئيسية
        </button>

    </div>

</section>


<!-- ADMIN LOGIN -->
<section id="adminLogin" class="card admin-login hidden">

    <div class="title">🔐 غرفة الإدارة</div>

    <div class="subtitle">
        سجل دخولك للوصول إلى التقديمات.
    </div>

    <div class="field">
        <label>كلمة مرور الإدارة</label>

        <input
            id="adminPassword"
            type="password"
            placeholder="••••••••"
        >
    </div>

    <br>

    <div class="actions">

        <button class="btn primary" onclick="adminLogin()">
            🔓 دخول
        </button>

        <button class="btn secondary" onclick="goHome()">
            رجوع
        </button>

    </div>

</section>


<!-- ADMIN PANEL -->
<section id="adminPanel" class="card hidden">

    <div class="admin-head">

        <div>
            <div class="title">🛡️ غرفة الإدارة</div>
            <div class="subtitle">
                إدارة جميع طلبات التقديم.
            </div>
        </div>

        <div class="actions">

            <button
                class="btn secondary"
                onclick="loadApplications()"
            >
                🔄 تحديث
            </button>

            <button
                class="btn danger"
                onclick="adminLogout()"
            >
                خروج
            </button>

        </div>

    </div>

    <div id="adminApplications" class="admin-list"></div>

</section>

</main>


<footer>
    EGYPT RP 🇪🇬 • Application System
</footer>

<div id="toast" class="toast"></div>


<script>

const questions = [

    "ما معنى RP؟",
    "ما معنى Fail RP؟",
    "ما معنى VDM؟",
    "ما معنى RDM؟",
    "ما معنى MetaGaming؟",
    "ما معنى PowerGaming؟",
    "ما معنى Fear RP؟",
    "ما معنى TK؟",
    "ما معنى SK؟",
    "ما معنى LTA؟",
    "ما معنى السيرفر؟",
    "ما معنى الراديو؟",
    "ما معنى أفعال صوتية؟",
    "ما معنى صداع؟",
    "ما معنى إعصار؟",
    "ما معنى فيلم / معركة؟",
    "ما معنى دفاعي؟",
    "ما معنى الحرارة؟",
    "ما معنى عين؟",
    "ما معنى سفر؟",
    "ما معنى مسرح؟",
    "ما معنى بنام؟",
    "ما معنى الأمن الوطني؟"

];

let answers = new Array(questions.length).fill("");
let currentQuestion = 0;
let timerInterval = null;
let timeLeft = 60;


function hideAll(){

    document
        .querySelectorAll("main > section")
        .forEach(section => {
            section.classList.add("hidden");
        });

}


function goHome(){

    clearInterval(timerInterval);

    hideAll();

    document
        .getElementById("home")
        .classList.remove("hidden");

    window.scrollTo({
        top:0,
        behavior:"smooth"
    });

}


function showRules(){

    hideAll();

    document
        .getElementById("rules")
        .classList.remove("hidden");

    document.getElementById("agreeRules").checked = false;

    checkRules();

    window.scrollTo({
        top:0,
        behavior:"smooth"
    });

}


function checkRules(){

    const checkbox =
        document.getElementById("agreeRules");

    const button =
        document.getElementById("continueBtn");

    button.disabled = !checkbox.checked;

    if(checkbox.checked){

        button.textContent =
            "🚀 ابدأ التقديم";

    }else{

        button.textContent =
            "🔒 وافق على القوانين أولاً";

    }

}


function startApplication(){

    if(!document.getElementById("agreeRules").checked){

        showToast("يجب الموافقة على القوانين أولاً");

        return;
    }

    hideAll();

    document
        .getElementById("basic")
        .classList.remove("hidden");

}


function startQuestions(){

    const name =
        document.getElementById("name").value.trim();

    const age =
        document.getElementById("age").value.trim();

    const discord =
        document.getElementById("discord").value.trim();

    if(!name || !age || !discord){

        showToast("من فضلك اكتب جميع البيانات");

        return;
    }

    currentQuestion = 0;

    hideAll();

    document
        .getElementById("questionsSection")
        .classList.remove("hidden");

    renderQuestion();

}


function renderQuestion(){

    clearInterval(timerInterval);

    const box =
        document.getElementById("questions");

    const q = questions[currentQuestion];

    box.innerHTML = `

        <div class="question">

            <div class="question-number">
                السؤال ${currentQuestion + 1} من ${questions.length}
            </div>

            <h3>${escapeHTML(q)}</h3>

            <textarea
                id="currentAnswer"
                maxlength="500"
                placeholder="اكتب إجابتك هنا..."
            >${escapeHTML(answers[currentQuestion])}</textarea>

        </div>

    `;

    const answerBox =
        document.getElementById("currentAnswer");

    answerBox.focus();

    answerBox.addEventListener("input",function(){

        answers[currentQuestion] =
            this.value;

    });

    updateProgress();

    timeLeft = 60;

    updateTimer();

    timerInterval = setInterval(() => {

        timeLeft--;

        updateTimer();

        if(timeLeft <= 0){

            clearInterval(timerInterval);

            answers[currentQuestion] =
                answerBox.value.trim();

            if(currentQuestion < questions.length - 1){

                currentQuestion++;

                renderQuestion();

            }else{

                showReview();

            }

        }

    },1000);

}


function updateTimer(){

    document.getElementById("timer")
        .textContent = timeLeft;

}


function updateProgress(){

    const percent =
        ((currentQuestion + 1) / questions.length) * 100;

    document.getElementById("progressBar")
        .style.width = percent + "%";

}


function showReview(){

    clearInterval(timerInterval);

    const answerBox =
        document.getElementById("currentAnswer");

    if(answerBox){

        answers[currentQuestion] =
            answerBox.value.trim();

    }

    hideAll();

    const review =
        document.getElementById("reviewData");

    let html = "";

    questions.forEach((question,index) => {

        html += `

            <div class="review-item">

                <div class="review-q">
                    ${index + 1}. ${escapeHTML(question)}
                </div>

                <div class="review-a">
                    ${escapeHTML(
                        answers[index] || "بدون إجابة"
                    )}
                </div>

            </div>

        `;

    });

    review.innerHTML = html;

    document
        .getElementById("review")
        .classList.remove("hidden");

    window.scrollTo({
        top:0,
        behavior:"smooth"
    });

}


function backToQuestions(){

    hideAll();

    document
        .getElementById("questionsSection")
        .classList.remove("hidden");

    renderQuestion();

}


async function submitApplication(){

    const name =
        document.getElementById("name").value.trim();

    const age =
        document.getElementById("age").value.trim();

    const discord =
        document.getElementById("discord").value.trim();

    if(
        !name ||
        !age ||
        !discord ||
        answers.some(a => !a.trim())
    ){

        showToast(
            "لازم تجاوب على جميع الأسئلة قبل الإرسال"
        );

        return;
    }

    const buttons =
        document.querySelectorAll("#review button");

    buttons.forEach(button => {
        button.disabled = true;
    });

    try{

        const response =
            await fetch("/api/application",{

                method:"POST",

                headers:{
                    "Content-Type":"application/json"
                },

                body:JSON.stringify({

                    name,
                    age,
                    discord,
                    answers

                })

            });

        const data =
            await response.json();

        if(!response.ok || !data.success){

            throw new Error(
                data.message ||
                "حدث خطأ"
            );

        }

        document
            .getElementById("applicationID")
            .textContent =
            data.applicationID;

        hideAll();

        document
            .getElementById("success")
            .classList.remove("hidden");

        window.scrollTo({
            top:0,
            behavior:"smooth"
        });

    }catch(error){

        buttons.forEach(button => {
            button.disabled = false;
        });

        showToast(
            error.message ||
            "حدث خطأ أثناء إرسال التقديم"
        );

    }

}


function showAdminLogin(){

    hideAll();

    document
        .getElementById("adminLogin")
        .classList.remove("hidden");

}


async function adminLogin(){

    const password =
        document.getElementById("adminPassword")
        .value;

    if(!password){

        showToast("اكتب كلمة المرور");

        return;
    }

    try{

        const response =
            await fetch("/api/admin/login",{

                method:"POST",

                headers:{
                    "Content-Type":"application/json"
                },

                body:JSON.stringify({
                    password
                })

            });

        const data =
            await response.json();

        if(!response.ok || !data.success){

            showToast(
                data.message ||
                "كلمة المرور غير صحيحة"
            );

            return;
        }

        document
            .getElementById("adminPassword")
            .value = "";

        hideAll();

        document
            .getElementById("adminPanel")
            .classList.remove("hidden");

        loadApplications();

    }catch(error){

        showToast(
            "تعذر الاتصال بالسيرفر"
        );

    }

}


async function loadApplications(){

    const box =
        document.getElementById("adminApplications");

    box.innerHTML =
        `<div class="subtitle">جاري تحميل التقديمات...</div>`;

    try{

        const response =
            await fetch("/api/admin/applications");

        const data =
            await response.json();

        if(!response.ok || !data.success){

            throw new Error(
                data.message ||
                "تعذر تحميل التقديمات"
            );

        }

        if(!data.applications.length){

            box.innerHTML =
                `<div class="subtitle">لا توجد تقديمات حتى الآن.</div>`;

            return;
        }

        box.innerHTML =
            data.applications
                .map(renderAdminApplication)
                .join("");

    }catch(error){

        box.innerHTML =
            `<div class="subtitle">${escapeHTML(
                error.message
            )}</div>`;

    }

}


function renderAdminApplication(app){

    let answersHTML = "";

    app.answers.forEach((answer,index) => {

        answersHTML += `

            <div class="answer-box">

                <b>
                    ${index + 1}. ${escapeHTML(
                        questions[index]
                    )}
                </b>

                <br><br>

                ${escapeHTML(answer)}

            </div>

        `;

    });

    let statusClass = "pending";

    if(app.status === "accepted"){
        statusClass = "accepted";
    }

    if(app.status === "rejected"){
        statusClass = "rejected";
    }

    let statusText = "⏳ قيد المراجعة";

    if(app.status === "accepted"){
        statusText = "✅ مقبول";
    }

    if(app.status === "rejected"){
        statusText = "❌ مرفوض";
    }

    return `

        <div class="admin-card">

            <div class="admin-head">

                <div>

                    <h2>
                        📝 ${escapeHTML(app.id)}
                    </h2>

                    <p style="color:#888;margin-top:5px">
                        ${escapeHTML(app.createdAt)}
                    </p>

                </div>

                <div class="status ${statusClass}">
                    ${statusText}
                </div>

            </div>

            <div class="answer-box">
                <b>👤 الاسم:</b>
                ${escapeHTML(app.name)}
            </div>

            <div class="answer-box">
                <b>🎂 العمر:</b>
                ${escapeHTML(app.age)}
            </div>

            <div class="answer-box">
                <b>💬 Discord:</b>
                ${escapeHTML(app.discord)}
            </div>

            <br>

            ${answersHTML}

            ${
                app.status === "pending"
                ?
                `
                <br>

                <div class="actions">

                    <button
                        class="btn success"
                        onclick="changeStatus('${app.id}','accepted')"
                    >
                        ✅ قبول التقديم
                    </button>

                    <button
                        class="btn danger"
                        onclick="changeStatus('${app.id}','rejected')"
                    >
                        ❌ رفض التقديم
                    </button>

                </div>
                `
                :
                ""
            }

        </div>

    `;

}


async function changeStatus(id,status){

    const action =
        status === "accepted"
        ? "قبول"
        : "رفض";

    if(!confirm(`هل تريد ${action} هذا التقديم؟`)){

        return;

    }

    try{

        const response =
            await fetch(
                `/api/admin/application/${encodeURIComponent(id)}`,
                {
                    method:"POST",

                    headers:{
                        "Content-Type":"application/json"
                    },

                    body:JSON.stringify({
                        status
                    })
                }
            );

        const data =
            await response.json();

        if(!response.ok || !data.success){

            throw new Error(
                data.message ||
                "تعذر تغيير الحالة"
            );

        }

        showToast("تم تحديث حالة التقديم ✅");

        loadApplications();

    }catch(error){

        showToast(
            error.message ||
            "حدث خطأ"
        );

    }

}


async function adminLogout(){

    await fetch(
        "/api/admin/logout",
        {
            method:"POST"
        }
    );

    goHome();

}


function showToast(message){

    const toast =
        document.getElementById("toast");

    toast.textContent = message;

    toast.classList.add("show");

    setTimeout(() => {

        toast.classList.remove("show");

    },3000);

}


function escapeHTML(value){

    return String(value ?? "")
        .replace(/&/g,"&amp;")
        .replace(/</g,"&lt;")
        .replace(/>/g,"&gt;")
        .replace(/"/g,"&quot;")
        .replace(/'/g,"&#039;");

}

</script>

</body>
</html>
