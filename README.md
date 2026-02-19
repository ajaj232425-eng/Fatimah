<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>بوابة القائدة الملهمة</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        :root {
            --primary: #006d51;
            --gold: #d4af37;
            --light-bg: #f8fbf9;
            --white: #ffffff;
            --whatsapp-color: #25d366;
        }

        body {
            font-family: 'Segoe UI', Tahoma, sans-serif;
            margin: 0;
            background-color: var(--light-bg);
            color: #333;
            line-height: 1.6;
        }

        header {
            background: linear-gradient(45deg, var(--primary), #004d39);
            color: white;
            padding: 50px 20px;
            text-align: center;
            border-bottom: 8px solid var(--gold);
            border-bottom-left-radius: 100px;
        }

        .header-container img { 
            width: 160px; 
            margin-bottom: 20px; 
            filter: brightness(0) invert(1); 
        }

        .header-container h1 { font-size: 2.2em; margin: 10px 0; }
        .inspirational-title { color: var(--gold); font-size: 1.4em; font-weight: bold; margin-top: 10px; }

        .container { max-width: 1100px; margin: auto; padding: 20px; }

        .transparent-kindergarten {
            background: var(--white);
            padding: 30px;
            border-radius: 30px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.05);
            margin-top: -60px;
            border: 1px solid #eee;
        }

        .section-title {
            color: var(--primary);
            display: flex;
            align-items: center;
            gap: 10px;
            font-size: 1.5em;
            margin-bottom: 20px;
            border-right: 5px solid var(--gold);
            padding-right: 15px;
        }

        .transparency-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .info-card {
            background: #fdfdfd;
            padding: 20px;
            border-radius: 20px;
            border: 1px solid #f0f0f0;
        }

        .passport-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 25px;
            margin-top: 25px;
        }

        .passport-item {
            background: var(--white);
            padding: 30px;
            border-radius: 25px;
            text-align: center;
            transition: 0.4s;
            cursor: pointer;
            border: 2px solid #f0f0f0;
            position: relative;
        }

        .passport-item:hover {
            border-color: var(--gold);
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }

        .passport-item i { font-size: 45px; color: var(--primary); margin-bottom: 15px; }

        /* --- أيقونة "اسألني" المنبثقة --- */
        .chat-widget {
            position: fixed;
            bottom: 30px;
            left: 30px;
            z-index: 10000;
        }

        .chat-button {
            background-color: var(--whatsapp-color);
            color: white;
            width: 70px;
            height: 70px;
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 30px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.2);
            cursor: pointer;
            transition: 0.3s;
            border: none;
        }

        .chat-button:hover { transform: scale(1.1); }

        .chat-box {
            display: none;
            position: absolute;
            bottom: 85px;
            left: 0;
            width: 300px;
            background: white;
            border-radius: 20px;
            box-shadow: 0 15px 40px rgba(0,0,0,0.2);
            overflow: hidden;
            animation: slideUp 0.3s ease-out;
        }

        .chat-header {
            background: var(--primary);
            color: white;
            padding: 15px;
            text-align: center;
            font-weight: bold;
        }

        .chat-body {
            padding: 15px;
        }

        .chat-body textarea {
            width: 100%;
            border: 1px solid #ddd;
            border-radius: 10px;
            padding: 10px;
            font-family: inherit;
            resize: none;
            box-sizing: border-box;
        }

        .send-btn {
            background: var(--whatsapp-color);
            color: white;
            border: none;
            width: 100%;
            padding: 10px;
            border-radius: 10px;
            margin-top: 10px;
            cursor: pointer;
            font-weight: bold;
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 10px;
        }

        @keyframes slideUp {
            from { transform: translateY(20px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }

        /* --- النافذة المنبثقة الأصلية للمهارات --- */
        .overlay {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            z-index: 9998;
            backdrop-filter: blur(5px);
        }

        .modal {
            display: none;
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background: white;
            padding: 40px;
            border-radius: 30px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.5);
            z-index: 9999;
            width: 85%;
            max-width: 500px;
            text-align: center;
            border-top: 10px solid var(--gold);
        }

        footer {
            margin-top: 60px;
            background: var(--primary);
            color: white;
            padding: 40px 20px;
            text-align: center;
        }
    </style>
</head>
<body>

<header>
    <div class="header-container">
        <img src="https://upload.wikimedia.org/wikipedia/commons/1/11/Ministry_of_Education_Saudi_Arabia_Logo.svg" alt="شعار وزارة التعليم">
        <h1>منصة الإنجاز والشفافية الرقمية</h1>
        <div class="inspirational-title">بوابة القائدة الملهمة</div>
    </div>
</header>

<div class="container">
    <section class="transparent-kindergarten">
        <div class="section-title">
            <i class="fas fa-certificate"></i> نظام الروضة الشفافة
        </div>
        <div class="transparency-grid">
            <div class="info-card">
                <h4 style="color:var(--primary)"><i class="fas fa-heart" style="color:var(--gold)"></i> قيمتنا الأسبوعية</h4>
                <p>"أنا طفل مؤدب" - نغرس فيهم آداب الحديث والاستئذان.</p>
            </div>
            <div class="info-card">
                <h4 style="color:var(--primary)"><i class="fas fa-carrot" style="color:#e67e22"></i> صحة المبدعين</h4>
                <p>نحرص هذا الأسبوع على تناول "الخضروات الورقية" لنمو سليم.</p>
            </div>
            <div class="info-card">
                <h4 style="color:var(--primary)"><i class="fas fa-star" style="color:var(--gold)"></i> إنجاز الأسبوع</h4>
                <p>تكريم الأطفال الملتزمين بالحضور المبكر في طابور الصباح.</p>
            </div>
        </div>
    </section>

    <section class="passport-section">
        <div class="section-title">
            <i class="fas fa-passport"></i> جواز السفر الذكي للمهارات
        </div>
        <div class="passport-grid">
            <div class="passport-item" onclick="openSkill('مهارة الاستقلال الذاتي', 'نعمل في الروضة على تمكين الطفل من الاعتماد على نفسه في احتياجاته الأساسية...')">
                <i class="fas fa-user-check"></i>
                <h3>الاستقلال الذاتي</h3>
            </div>
            <div class="passport-item" onclick="openSkill('الطلاقة اللغوية والتعبير', 'من خلال استراتيجيات الحوار والمناقشة...')">
                <i class="fas fa-comments"></i>
                <h3>الطلاقة اللغوية</h3>
            </div>
            <div class="passport-item" onclick="openSkill('الذكاء الوجداني والاجتماعي', 'نغرس في الطفل مهارة ضبط الانفعالات والتعاطف...')">
                <i class="fas fa-heartbeat"></i>
                <h3>الذكاء الوجداني</h3>
            </div>
            <div class="passport-item" onclick="openSkill('مهارات المستقبل (STEM)', 'نهيئ الطفل لعصر التقنية عبر ألعاب التفكير المنطقي...')">
                <i class="fas fa-rocket"></i>
                <h3>مهارات المستقبل</h3>
            </div>
        </div>
    </section>
</div>

<div class="chat-widget">
    <div class="chat-box" id="chatBox">
        <div class="chat-header">ضع سؤالك ولي الأمر وسنجيبك</div>
        <div class="chat-body">
            <textarea id="userQuestion" rows="4" placeholder="اكتب استفسارك هنا..."></textarea>
            <button class="send-btn" onclick="sendToWhatsApp()">
                إرسال عبر واتساب <i class="fab fa-whatsapp"></i>
            </button>
        </div>
    </div>
    <button class="chat-button" onclick="toggleChat()">
        <i class="fas fa-question-circle"></i>
    </button>
</div>

<footer>
    <p>بإشراف القائدة التربوية:</p>
    <p>نصنع الأثر.. ونبني الأجيال</p>
</footer>

<div class="overlay" id="overlay" onclick="closeSkill()"></div>
<div class="modal" id="modal">
    <div style="font-size: 3em; color: var(--gold); margin-bottom: 15px;"><i class="fas fa-award"></i></div>
    <h3 id="skillTitle" style="color:var(--primary); font-size: 1.5em; margin-bottom: 15px;"></h3>
    <p id="skillDesc" style="line-height:1.8; color:#555; text-align: justify;"></p>
    <button onclick="closeSkill()" style="background:var(--primary); color:white; border:none; padding:12px 30px; border-radius:15px; cursor:pointer; margin-top:20px; font-weight:bold;">العودة للمنصة</button>
</div>

<script>
    function toggleChat() {
        const chatBox = document.getElementById('chatBox');
        chatBox.style.display = (chatBox.style.display === 'block') ? 'none' : 'block';
    }

    function sendToWhatsApp() {
        const question = document.getElementById('userQuestion').value;
        if (!question.trim()) {
            alert("لطفاً اكتب سؤالك أولاً ✨");
            return;
        }
        const phoneNumber = "966175456910"; // رقمك
        const url = `https://wa.me/${phoneNumber}?text=${encodeURIComponent('سؤال من ولي أمر: ' + question)}`;
        window.open(url, '_blank');
        toggleChat(); // إغلاق الصندوق بعد الإرسال
    }

    function openSkill(title, desc) {
        document.getElementById('skillTitle').innerText = title;
        document.getElementById('skillDesc').innerText = desc;
        document.getElementById('modal').style.display = 'block';
        document.getElementById('overlay').style.display = 'block';
        document.body.style.overflow = 'hidden';
    }

    function closeSkill() {
        document.getElementById('modal').style.display = 'none';
        document.getElementById('overlay').style.display = 'none';
        document.body.style.overflow = 'auto';
    }
</script>

</body>
</html>
