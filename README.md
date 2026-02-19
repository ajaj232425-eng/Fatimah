<! فكره أ/ فاطمه صالح نحو الاستدامه>
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
            --bg: #f4f7f6;
            --white: #ffffff;
        }

        body {
            font-family: 'Segoe UI', Tahoma, sans-serif;
            margin: 0;
            background-color: var(--bg);
            color: #333;
        }

        /* الهيدر */
        header {
            background: linear-gradient(135deg, var(--primary), #004d39);
            color: white;
            padding: 50px 20px;
            text-align: center;
            border-bottom: 6px solid var(--gold);
            border-bottom-left-radius: 80px;
        }

        .header-container img { width: 150px; filter: brightness(0) invert(1); margin-bottom: 15px; }
        .inspirational-title { color: var(--gold); font-size: 1.4em; font-weight: bold; margin-top: 5px; }

        .container { max-width: 1100px; margin: auto; padding: 20px; position: relative; z-index: 1; }

        /* قسم الروضة الشفافة */
        .transparency-section {
            background: var(--white);
            padding: 30px;
            border-radius: 30px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.05);
            margin-top: -50px;
            border: 1px solid #eee;
            margin-bottom: 40px;
        }

        .section-title {
            color: var(--primary);
            font-size: 1.6em;
            margin-bottom: 25px;
            display: flex;
            align-items: center;
            gap: 12px;
            border-right: 5px solid var(--gold);
            padding-right: 15px;
        }

        .transparency-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
        }

        .info-card {
            background: #fafafa;
            padding: 20px;
            border-radius: 20px;
            border-right: 4px solid var(--gold);
        }

        /* قسم جواز السفر */
        .passport-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 20px;
        }

        .passport-item {
            background: var(--white);
            padding: 35px 20px;
            border-radius: 25px;
            text-align: center;
            cursor: pointer;
            border: 1px solid #eee;
            transition: 0.3s;
        }

        .passport-item:hover { transform: translateY(-5px); border-color: var(--gold); }
        .passport-item i { font-size: 45px; color: var(--primary); margin-bottom: 15px; }

        /* الحل النهائي لمشكلة الظهور بالخلف */
        #fixed-modal-overlay {
            display: none;
            position: fixed;
            top: 0; left: 0;
            width: 100vw; height: 100vh;
            background: rgba(0, 0, 0, 0.9); /* تعتيم شبه كامل */
            z-index: 999999 !important; /* أعلى طبقة ممكنة فوق كل الأيقونات */
            backdrop-filter: blur(10px);
        }

        .modal-box {
            position: absolute;
            top: 50%; left: 50%;
            transform: translate(-50%, -50%);
            background: white;
            width: 85%; max-width: 450px;
            padding: 40px;
            border-radius: 30px;
            text-align: center;
            border-top: 10px solid var(--gold);
            box-shadow: 0 0 50px rgba(0,0,0,0.8);
        }

        .btn-close {
            background: var(--primary);
            color: white;
            border: none;
            padding: 12px 40px;
            border-radius: 15px;
            cursor: pointer;
            margin-top: 25px;
            font-weight: bold;
        }

        .qa-float {
            position: fixed;
            bottom: 30px; left: 30px;
            background: var(--gold);
            color: white;
            width: 65px; height: 65px;
            border-radius: 50%;
            display: flex;
            justify-content: center; align-items: center;
            font-size: 28px;
            cursor: pointer;
            z-index: 1000;
        }

        /* تذييل الصفحة مع الاسم */
        footer {
            background: var(--primary);
            color: white;
            padding: 50px 20px;
            text-align: center;
            margin-top: 60px;
            border-top: 5px solid var(--gold);
        }

        .footer-name {
            font-size: 1.8em;
            color: var(--gold);
            margin-bottom: 10px;
            font-weight: bold;
        }
    </style>
</head>
<body>

<header>
    <img src="https://upload.wikimedia.org/wikipedia/commons/1/11/Ministry_of_Education_Saudi_Arabia_Logo.svg" alt="وزارة التعليم">
    <h1>منصة الإنجاز والشفافية الرقمية</h1>
    <div class="inspirational-title">بوابة القائدة الملهمة</div>
</header>

<div class="container">
    
    <section class="transparency-section">
        <div class="section-title"><i class="fas fa-eye"></i> الروضة الشفافة</div>
        <div class="transparency-grid">
            <div class="info-card">
                <h4><i class="fas fa-star"></i> قيمة الأسبوع</h4>
                <p>"أنا طفل مسؤول" - تعزيز مهارة الاعتماد على النفس.</p>
            </div>
            <div class="info-card">
                <h4><i class="fas fa-apple-alt"></i> وجبتي الصحية</h4>
                <p>التركيز على شرب الماء وتناول الفواكه الطازجة.</p>
            </div>
        </div>
    </section>

    <h2 style="text-align: center; color: var(--primary);">جواز السفر الذكي للمهارات</h2>
    <div class="passport-grid">
        <div class="passport-item" onclick="openMe('الاستقلال الذاتي', 'بناء شخصية الطفل ليكون قادراً على إدارة شؤونه الخاصة بثقة تامة.')">
            <i class="fas fa-user-check"></i>
            <h3>الاستقلال الذاتي</h3>
        </div>
        <div class="passport-item" onclick="openMe('الطلاقة اللغوية', 'تطوير مهارات الحوار والتحدث بطلاقة وثقة أمام الجمهور.')">
            <i class="fas fa-comments"></i>
            <h3>الطلاقة اللغوية</h3>
        </div>
        <div class="passport-item" onclick="openMe('الذكاء الوجداني', 'فهم المشاعر والتعامل مع الأقران بروح اجتماعية إيجابية.')">
            <i class="fas fa-heart"></i>
            <h3>الذكاء الوجداني</h3>
        </div>
        <div class="passport-item" onclick="openMe('مهارات المستقبل', 'تنمية مهارات التفكير الرقمي والابتكار لمواكبة رؤية الوطن.')">
            <i class="fas fa-rocket"></i>
            <h3>مهارات المستقبل</h3>
        </div>
    </div>
</div>

<div id="fixed-modal-overlay">
    <div class="modal-box">
        <div style="font-size: 50px; color: var(--gold); margin-bottom: 10px;"><i class="fas fa-award"></i></div>
        <h2 id="m-title" style="color: var(--primary);"></h2>
        <p id="m-desc" style="font-size: 1.1em; line-height: 1.6;"></p>
        <button class="btn-close" onclick="closeMe()">إغلاق</button>
    </div>
</div>

<div class="qa-float" onclick="alert('سيتم فتح نظام الأسئلة قريباً')"><i class="fas fa-question-circle"></i></div>

<footer>
    <div class="footer-name">فاطمه صالح آل بحري</div>
    <p>القائدة الملهمة للمنصة الرقمية</p>
    <p>نصنع الأثر.. ونبني الأجيال</p>
    <p style="margin-top:20px; font-size: 0.8em; opacity: 0.7;">حقوق التصميم محفوظة © 2026</p>
</footer>

<script>
    function openMe(t, d) {
        document.getElementById('m-title').innerText = t;
        document.getElementById('m-desc').innerText = d;
        document.getElementById('fixed-modal-overlay').style.display = 'block';
        document.body.style.overflow = 'hidden';
    }
    function closeMe() {
        document.getElementById('fixed-modal-overlay').style.display = 'none';
        document.body.style.overflow = 'auto';
    }
</script>

</body>
</html>
