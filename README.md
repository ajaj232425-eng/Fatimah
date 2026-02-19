<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>بوابة القائدة الملهمة | فاطمه آل بحري</title>
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
            line-height: 1.6;
        }

        /* الهيدر الفاخر */
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

        .header-container h1 { 
            font-size: 2.2em; 
            margin: 10px 0; 
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3); 
        }

        .inspirational-title {
            color: var(--gold);
            font-size: 1.4em;
            font-weight: bold;
            margin-top: 10px;
            letter-spacing: 1px;
        }

        .container { max-width: 1100px; margin: auto; padding: 20px; }

        /* قسم الروضة الشفافة */
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
            transition: 0.3s;
        }
        .info-card:hover { background: #fffdf5; }

        /* قسم جواز السفر الذكي */
        .passport-section { margin-top: 50px; }

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
            overflow: hidden;
        }

        .passport-item::before {
            content: "انقر للتفاصيل";
            position: absolute;
            top: 0; left: 0; width: 100%;
            background: var(--gold);
            color: white;
            font-size: 0.7em;
            padding: 2px 0;
            transform: translateY(-100%);
            transition: 0.3s;
        }

        .passport-item:hover::before { transform: translateY(0); }

        .passport-item:hover {
            border-color: var(--gold);
            transform: translateY(-10px);
            box-shadow: 0 15px 35px rgba(0,0,0,0.1);
        }

        .passport-item i { font-size: 45px; color: var(--primary); margin-bottom: 15px; }

        /* Modal للتفاعل */
        .modal {
            display: none;
            position: fixed;
            top: 50%; left: 50%;
            transform: translate(-50%, -50%);
            background: white;
            padding: 40px;
            border-radius: 30px;
            box-shadow: 0 0 50px rgba(0,0,0,0.4);
            z-index: 1001;
            width: 85%; max-width: 500px;
            text-align: center;
            border-top: 10px solid var(--gold);
        }
        .overlay { display: none; position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.7); z-index: 1000; }

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
        <div class="inspirational-title">بوابة القائدة الملهمة: فاطمه صالح آل بحري</div>
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
            <div class="passport-item" onclick="openSkill('مهارة الاستقلال الذاتي', 'نعمل في الروضة على تمكين الطفل من الاعتماد على نفسه في احتياجاته الأساسية مثل (ترتيب الحقيبة، غسل اليدين، وارتداء الحذاء) لتعزيز ثقته بنفسه كعضو فعال.')">
                <i class="fas fa-user-check"></i>
                <h3>الاستقلال الذاتي</h3>
            </div>

            <div class="passport-item" onclick="openSkill('الطلاقة اللغوية والتعبير', 'من خلال استراتيجيات الحوار والمناقشة، ننمي لدى الطفل القدرة على سرد القصص والتعبير عن مشاعره بوضوح، مع حفظ وتذوق الحروف والكلمات بأسلوب شيق.')">
                <i class="fas fa-comments"></i>
                <h3>الطلاقة اللغوية</h3>
            </div>

            <div class="passport-item" onclick="openSkill('الذكاء الوجداني والاجتماعي', 'نغرس في الطفل مهارة ضبط الانفعالات والتعاطف مع الأقران، وبناء صداقات إيجابية قائمة على الاحترام المتبادل وفهم المشاعر.')">
                <i class="fas fa-heartbeat"></i>
                <h3>الذكاء الوجداني</h3>
            </div>

            <div class="passport-item" onclick="openSkill('مهارات المستقبل (STEM)', 'نهيئ الطفل لعصر التقنية عبر ألعاب التفكير المنطقي، حل المشكلات البسيطة، والتعامل الذكي مع الأدوات الرقمية بوعي وإبداع.')">
                <i class="fas fa-rocket"></i>
                <h3>مهارات المستقبل</h3>
            </div>
        </div>
    </section>

</div>

<footer>
    <p>بإشراف القائدة التربوية:</p>
    <h2 style="color:var(--gold); margin: 5px 0;">فاطمه صالح آل بحري</h2>
    <p>نصنع الأثر.. ونبني الأجيال</p>
    <p style="margin-top:20px; font-size:0.8em; opacity:0.6;">إدارة تعليم نجران - المملكة العربية السعودية 2026</p>
</footer>

<div class="overlay" id="overlay" onclick="closeSkill()"></div>
<div class="modal" id="modal">
    <div style="font-size: 3em; color: var(--gold); margin-bottom: 15px;"><i class="fas fa-award"></i></div>
    <h3 id="skillTitle" style="color:var(--primary); font-size: 1.5em; margin-bottom: 15px;"></h3>
    <p id="skillDesc" style="line-height:1.8; color:#555; text-align: justify;"></p>
    <button onclick="closeSkill()" style="background:var(--primary); color:white; border:none; padding:12px 30px; border-radius:15px; cursor:pointer; margin-top:20px; font-weight:bold;">العودة للمنصة</button>
</div>

<script>
    function openSkill(title, desc) {
        document.getElementById('skillTitle').innerText = title;
        document.getElementById('skillDesc').innerText = desc;
        document.getElementById('modal').style.display = 'block';
        document.getElementById('overlay').style.display = 'block';
    }

    function closeSkill() {
        document.getElementById('modal').style.display = 'none';
        document.getElementById('overlay').style.display = 'none';
    }
</script>

</body>
</html>
