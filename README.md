<! فكره الاستاذه فاطمه صالح لدوام الاستدامه>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>بوابة القائدة الملهمة | جواز السفر الذكي</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        :root {
            --primary: #006d51;
            --gold: #d4af37;
            --bg: #f8fbf9;
        }

        body {
            font-family: 'Segoe UI', Tahoma, sans-serif;
            margin: 0;
            background-color: var(--bg);
            color: #333;
        }

        header {
            background: linear-gradient(45deg, var(--primary), #004d39);
            color: white;
            padding: 40px 20px;
            text-align: center;
            border-bottom: 6px solid var(--gold);
        }

        .header-container img { width: 140px; filter: brightness(0) invert(1); }

        .container { max-width: 1000px; margin: auto; padding: 20px; }

        /* شبكة جواز السفر */
        .passport-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }

        .passport-item {
            background: white;
            padding: 30px;
            border-radius: 20px;
            text-align: center;
            cursor: pointer;
            border: 1px solid #eee;
            transition: 0.3s;
            position: relative;
            z-index: 1; /* طبقة عادية */
        }

        .passport-item:hover { transform: translateY(-5px); border-color: var(--gold); }
        .passport-item i { font-size: 40px; color: var(--primary); margin-bottom: 15px; }

        /* --- حل مشكلة الظهور (الطبقات العليا) --- */
        
        /* الستارة الخلفية */
        .overlay {
            display: none;
            position: fixed;
            top: 0; left: 0;
            width: 100%; height: 100%;
            background: rgba(0, 0, 0, 0.7); /* تعتيم قوي */
            z-index: 9998; /* تحت النافذة مباشرة */
            backdrop-filter: blur(8px); /* جعل الخلفية مغبشة */
        }

        /* النافذة المنبثقة */
        .modal {
            display: none;
            position: fixed;
            top: 50%; left: 50%;
            transform: translate(-50%, -50%);
            background: white;
            padding: 35px;
            border-radius: 25px;
            width: 85%;
            max-width: 450px;
            text-align: center;
            z-index: 9999; /* أعلى طبقة في الموقع كله */
            box-shadow: 0 25px 50px rgba(0,0,0,0.5);
            border-top: 8px solid var(--gold);
            animation: fadeIn 0.4s ease-out;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translate(-50%, -45%); }
            to { opacity: 1; transform: translate(-50%, -50%); }
        }

        .modal h3 { color: var(--primary); margin-bottom: 15px; font-size: 1.4em; }
        .modal p { line-height: 1.8; color: #444; text-align: justify; }

        .close-btn {
            background: var(--primary);
            color: white;
            border: none;
            padding: 10px 25px;
            border-radius: 10px;
            cursor: pointer;
            margin-top: 20px;
            font-weight: bold;
        }

        /* أيقونة اسألني التفاعلية */
        .qa-float {
            position: fixed;
            bottom: 25px;
            left: 25px;
            background: var(--gold);
            color: white;
            width: 60px; height: 60px;
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 24px;
            cursor: pointer;
            z-index: 9000;
            box-shadow: 0 10px 20px rgba(0,0,0,0.2);
        }
    </style>
</head>
<body>

<header>
    <div class="header-container">
        <img src="https://upload.wikimedia.org/wikipedia/commons/1/11/Ministry_of_Education_Saudi_Arabia_Logo.svg" alt="الشعار">
        <h1>منصة الإنجاز والشفافية</h1>
        <div style="color: var(--gold); font-weight: bold; margin-top: 10px;">بوابة القائدة الملهمة</div>
    </div>
</header>

<div class="container">
    <div class="passport-grid">
        <div class="passport-item" onclick="openPop('الاستقلال الذاتي', 'نركز في هذا المسار على بناء شخصية الطفل ليكون قادراً على إدارة شؤونه الخاصة، من تنظيم أدواته إلى اتخاذ قراراته البسيطة بثقة.')">
            <i class="fas fa-user-shield"></i>
            <h3>الاستقلال الذاتي</h3>
        </div>
        <div class="passport-item" onclick="openPop('الطلاقة اللغوية', 'برنامج إثرائي لتعزيز لغة الطفل وحصيلته اللغوية عبر القراءة التفاعلية وفنون الإلقاء أمام الأقران.')">
            <i class="fas fa-comment-dots"></i>
            <h3>الطلاقة اللغوية</h3>
        </div>
        <div class="passport-item" onclick="openPop('الذكاء الوجداني', 'تعليم الطفل مهارات التعاطف، وفهم المشاعر الذاتية، وبناء علاقات اجتماعية إيجابية وناجحة.')">
            <i class="fas fa-heart"></i>
            <h3>الذكاء الوجداني</h3>
        </div>
        <div class="passport-item" onclick="openPop('مهارات المستقبل', 'دمج التقنية بالتفكير المنطقي، لتهيئة طفل مبدع في حل المشكلات ومواكب لعصر التحول الرقمي.')">
            <i class="fas fa-laptop-code"></i>
            <h3>مهارات المستقبل</h3>
        </div>
    </div>
</div>

<div class="overlay" id="overlay" onclick="closePop()"></div>
<div class="modal" id="modal">
    <div style="font-size: 40px; color: var(--gold); margin-bottom: 10px;"><i class="fas fa-star"></i></div>
    <h3 id="mTitle"></h3>
    <p id="mDesc"></p>
    <button class="close-btn" onclick="closePop()">حسناً، فهمت</button>
</div>

<div class="qa-float" onclick="alert('سيتم فتح صندوق الأسئلة التفاعلي قريباً..')">
    <i class="fas fa-question"></i>
</div>

<script>
    function openPop(title, desc) {
        document.getElementById('mTitle').innerText = title;
        document.getElementById('mDesc').innerText = desc;
        document.getElementById('overlay').style.display = 'block';
        document.getElementById('modal').style.display = 'block';
        // منع تحرك الصفحة خلف النافذة
        document.body.style.overflow = 'hidden';
    }

    function closePop() {
        document.getElementById('overlay').style.display = 'none';
        document.getElementById('modal').style.display = 'none';
        document.body.style.overflow = 'auto';
    }
</script>

</body>
</html>
