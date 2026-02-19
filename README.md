<! فكره أ/ فاطمه صالح لدوام الاستدامه>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>منصة الإنجاز والشفافية | القائدة الملهمة</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        :root {
            --primary: #006d51;
            --gold: #d4af37;
            --light-bg: #f8fbf9;
            --white: #ffffff;
        }

        body {
            font-family: 'Segoe UI', Tahoma, sans-serif;
            margin: 0;
            background-color: var(--light-bg);
            color: #333;
        }

        /* الهيدر */
        header {
            background: linear-gradient(45deg, var(--primary), #004d39);
            color: white;
            padding: 50px 20px;
            text-align: center;
            border-bottom: 8px solid var(--gold);
            border-bottom-left-radius: 100px;
        }

        .container { max-width: 1100px; margin: auto; padding: 20px; }

        /* قسم الأسئلة والأجوبة الجديد */
        .qa-section {
            margin-top: 50px;
            background: white;
            padding: 30px;
            border-radius: 30px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.05);
        }

        .question-form {
            background: #f9f9f9;
            padding: 20px;
            border-radius: 20px;
            margin-bottom: 30px;
            border: 2px dashed var(--gold);
        }

        textarea {
            width: 100%;
            padding: 15px;
            border-radius: 15px;
            border: 1px solid #ddd;
            margin-bottom: 10px;
            resize: none;
            box-sizing: border-box;
        }

        .submit-btn {
            background: var(--primary);
            color: white;
            border: none;
            padding: 10px 25px;
            border-radius: 10px;
            cursor: pointer;
            font-weight: bold;
        }

        /* عرض الأسئلة */
        .questions-list {
            display: grid;
            gap: 15px;
        }

        .qa-card {
            background: #fff;
            border-right: 5px solid var(--gold);
            padding: 15px;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.05);
        }

        .qa-card .user-q { font-weight: bold; color: var(--primary); margin-bottom: 5px; }
        .qa-card .admin-a { 
            background: #f0f7f4; 
            padding: 10px; 
            border-radius: 8px; 
            font-size: 0.9em; 
            margin-top: 10px;
            color: #444;
        }

        /* أيقونة منبثقة عائمة */
        .floating-qa-btn {
            position: fixed;
            bottom: 30px;
            left: 30px;
            background: var(--gold);
            color: white;
            width: 65px;
            height: 65px;
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 25px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.2);
            cursor: pointer;
            z-index: 999;
        }

        /* النافذة المنبثقة للأسئلة */
        .qa-popup {
            display: none;
            position: fixed;
            bottom: 110px;
            left: 30px;
            width: 350px;
            max-height: 500px;
            background: white;
            border-radius: 20px;
            box-shadow: 0 10px 40px rgba(0,0,0,0.2);
            z-index: 1000;
            overflow-y: auto;
            padding: 20px;
            animation: slideIn 0.3s ease;
        }

        @keyframes slideIn { from { transform: translateY(20px); opacity: 0; } to { transform: translateY(0); opacity: 1; } }

        .close-qa { float: left; cursor: pointer; color: #999; }
    </style>
</head>
<body>

<header>
    <img src="https://upload.wikimedia.org/wikipedia/commons/1/11/Ministry_of_Education_Saudi_Arabia_Logo.svg" width="150" alt="وزارة التعليم">
    <h1>منصة الإنجاز والشفافية الرقمية</h1>
    <div style="color: var(--gold); font-weight: bold; font-size: 1.2em;">بوابة القائدة الملهمة</div>
</header>

<div class="container">
    <p style="text-align: center;">مرحباً بكم في منصتنا التربوية التفاعلية</p>
</div>

<div class="floating-qa-btn" onclick="toggleQA()">
    <i class="fas fa-comments"></i>
</div>

<div class="qa-popup" id="qaPopup">
    <span class="close-qa" onclick="toggleQA()"><i class="fas fa-times"></i></span>
    <h3 style="color: var(--primary); margin-top: 0;">اسأل القائدة وسنجيبك ✨</h3>
    
    <div class="question-form">
        <textarea id="qInput" placeholder="اكتب سؤالك هنا بوضوح..."></textarea>
        <button class="submit-btn" onclick="addQuestion()">إرسال السؤال</button>
    </div>

    <div class="questions-list" id="qList">
        <div class="qa-card">
            <div class="user-q">ولي أمر: ما هي مواعيد الزيارة الرسمية؟</div>
            <div class="admin-a"><strong>رد القائدة:</strong> نسعد باستقبالكم يومي الاثنين والأربعاء من الساعة 10 صباحاً.</div>
        </div>
        <div class="qa-card">
            <div class="user-q">ولي أمر: هل يوجد رحلات ميدانية قريباً؟</div>
            <div class="admin-a"><strong>رد القائدة:</strong> نعم، سيتم الإعلان عن رحلة "عالم الاستكشاف" الأسبوع القادم بإذن الله.</div>
        </div>
    </div>
</div>

<script>
    function toggleQA() {
        const popup = document.getElementById('qaPopup');
        popup.style.display = (popup.style.display === 'block') ? 'none' : 'block';
    }

    function addQuestion() {
        const input = document.getElementById('qInput');
        if (input.value.trim() === "") return;

        const list = document.getElementById('qList');
        const newQA = document.createElement('div');
        newQA.className = 'qa-card';
        newQA.innerHTML = `
            <div class="user-q">ولي أمر: ${input.value}</div>
            <div class="admin-a" style="color: #d4af37;"><em>قيد المراجعة.. سيتم الرد قريباً</em></div>
        `;
        
        list.prepend(newQA); // وضع السؤال الجديد في الأعلى
        input.value = "";
        alert("تم استلام سؤالك، وسيظهر الرد هنا فور اعتماد القائدة له ✅");
    }
</script>

</body>
</html>
