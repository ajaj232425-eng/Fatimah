<! فكره أ/ فاطمه صالح نحو الاستدامه>
< rt>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>منصة الإنجاز والشفافية | فاطمه آل بحري</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        :root {
            --primary: #006d51;
            --gold: #d4af37;
            --white: #ffffff;
            --bg: #f4f7f6;
        }

        body { font-family: 'Segoe UI', Tahoma, sans-serif; margin: 0; background-color: var(--bg); color: #333; overflow-x: hidden; }

        /* الهيدر */
        header {
            background: linear-gradient(135deg, var(--primary), #004d39);
            color: white; padding: 50px 20px; text-align: center; border-bottom: 8px solid var(--gold);
            border-bottom-left-radius: 80px;
        }

        .header-container img { width: 130px; filter: brightness(0) invert(1); margin-bottom: 15px; }

        .container { max-width: 1100px; margin: auto; padding: 20px; position: relative; z-index: 1; }

        /* --- قسم الروضة الشفافة --- */
        .transparency-section {
            background: var(--white);
            padding: 30px;
            border-radius: 30px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.05);
            margin-top: -60px;
            margin-bottom: 40px;
            border: 1px solid #eee;
        }

        .section-title {
            color: var(--primary); font-size: 1.6em; margin-bottom: 25px;
            display: flex; align-items: center; gap: 12px;
            border-right: 6px solid var(--gold); padding-right: 15px;
        }

        .transparency-grid {
            display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 20px;
        }

        .info-card {
            background: #fafafa; padding: 20px; border-radius: 20px;
            border-bottom: 4px solid var(--gold); transition: 0.3s;
        }

        /* --- قسم جواز السفر الذكي --- */
        .passport-grid {
            display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 20px;
        }

        .passport-item {
            background: white; padding: 35px 20px; border-radius: 25px; text-align: center;
            cursor: pointer; border: 1px solid #eee; transition: 0.3s;
        }

        /* --- الحل النهائي للظهور في الأمام (الانبثاق المطلق) --- */
        #exclusive-modal-layer {
            display: none;
            position: fixed;
            top: 0; left: 0;
            width: 100%; height: 100%;
            background: rgba(0, 0, 0, 0.9); /* تعتيم خلفية الموقع بالكامل */
            z-index: 2147483647 !important; /* أعلى قيمة برمجية لضمان الظهور فوق الأيقونات */
            justify-content: center; align-items: center;
            backdrop-filter: blur(15px);
        }

        .modal-card {
            background: white; width: 85%; max-width: 450px;
            padding: 40px; border-radius: 35px; text-align: center;
            box-shadow: 0 30px 60px rgba(0,0,0,0.5);
            border-top: 12px solid var(--gold);
            animation: popUp 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }

        @keyframes popUp {
            from { transform: scale(0.5); opacity: 0; }
            to { transform: scale(1); opacity: 1; }
        }

        .btn-close {
            background: var(--primary); color: white; border: none;
            padding: 12px 40px; border-radius: 15px; cursor: pointer;
            margin-top: 25px; font-weight: bold;
        }

        /* تذييل الصفحة بالاسم */
        footer {
            background: var(--primary); color: white; padding: 60px 20px;
            text-align: center; margin-top: 60px; border-top: 6px solid var(--gold);
        }

        .footer-name { font-size: 2.2em; color: var(--gold); font-weight: bold; margin-bottom: 5px; }
    </style>
</head>
<body>

<div id="wrapper">
    <header>
        <div class="header-container">
            <img src="https://upload.wikimedia.org/wikipedia/commons/1/11/Ministry_of_Education_Saudi_Arabia_Logo.svg" alt="وزارة التعليم">
            <h1>منصة الإنجاز والشفافية الرقمية</h1>
            <p style="color: var(--gold); font-weight: bold; font-size: 1.2em;">بوابة القائدة الملهمة</p>
        </div>
    </header>

    <div class="container">
        
        <section class="transparency-section">
            <div class="section-title">
                <i class="fas fa-bullhorn"></i> الروضة الشفافة (تواصلنا الأسبوعي)
            </div>
            <div class="transparency-grid">
                <div class="info-card">
                    <h4><i class="fas fa-star" style="color:var(--gold)"></i> قيمة الأسبوع</h4>
                    <p>"التعاون والمشاركة" - نعلم أطفالنا متعة العمل الجماعي وروح الفريق الواحد.</p>
                </div>
                <div class="info-card">
                    <h4><i class="fas fa-apple-alt" style="color:#e67e22"></i> صحة المبدعين</h4>
                    <p>نحرص هذا الأسبوع على تناول "الخضروات الورقية" لتقوية مناعة أبطالنا الصغار.</p>
                </div>
                <div class="info-card">
                    <h4><i class="fas fa-calendar-check" style="color:#3498db"></i> إعلان هام</h4>
                    <p>يسرنا دعوتكم لحضور "اليوم المفتوح للابتكار" يوم الخميس القادم بإذن الله.</p>
                </div>
            </div>
        </section>

        <h2 style="text-align: center; color: var(--primary); font-size: 1.8em; margin-bottom: 30px;">جواز السفر الذكي للمهارات</h2>
        <div class="passport-grid">
            <div class="passport-item" onclick="openBox('الاستقلال الذاتي', 'بناء شخصية الطفل ليكون قادراً على إدارة شؤونه الخاصة بثقة تامة وشعور بالمسؤولية.')">
                <i class="fas fa-user-check"></i>
                <h3>الاستقلال الذاتي</h3>
            </div>
            <div class="passport-item" onclick="openBox('الطلاقة اللغوية', 'تطوير مهارات الحوار، التعبير، والقدرة على سرد القصص بأسلوب لغوي رصين وواثق.')">
                <i class="fas fa-comments"></i>
                <h3>الطلاقة اللغوية</h3>
            </div>
            <div class="passport-item" onclick="openBox('الذكاء الوجداني', 'فهم المشاعر الذاتية ومشاعر الآخرين، وبناء جسور من التواصل الاجتماعي القائم على الاحترام.')">
                <i class="fas fa-heart"></i>
                <h3>الذكاء الوجداني</h3>
            </div>
            <div class="passport-item" onclick="openBox('مهارات المستقبل', 'تنمية مهارات التفكير الناقد وحل المشكلات البسيطة بوعي رقمي وابتكار يواكب الرؤية.')">
                <i class="fas fa-rocket"></i>
                <h3>مهارات المستقبل</h3>
            </div>
        </div>
    </div>

    <footer>
        <div class="footer-name">فاطمه صالح آل بحري</div>
        <p>القائدة التربوية الملهمة</p>
        <p>نصنع الأثر.. ونبني الأجيال</p>
        <p style="margin-top: 25px; font-size: 0.8em; opacity: 0.7;">جميع الحقوق محفوظة © 2026</p>
    </footer>
</div>

<div id="exclusive-modal-layer">
    <div class="modal-card">
        <div style="font-size: 60px; color: var(--gold); margin-bottom: 15px;"><i class="fas fa-certificate"></i></div>
        <h2 id="m-title" style="color: var(--primary); margin-bottom: 15px;"></h2>
        <p id="m-desc" style="line-height: 1.8; color: #444; font-size: 1.1em;"></p>
        <button class="btn-close" onclick="closeBox()">إغلاق</button>
    </div>
</div>

<script>
    function openBox(title, desc) {
        document.getElementById('m-title').innerText = title;
        document.getElementById('m-desc').innerText = desc;
        document.getElementById('exclusive-modal-layer').style.display = 'flex';
        // تجميد التفاعل في الخلفية تماماً
        document.getElementById('wrapper').style.filter = 'blur(5px)';
        document.body.style.overflow = 'hidden';
    }

    function closeBox() {
        document.getElementById('exclusive-modal-layer').style.display = 'none';
        document.getElementById('wrapper').style.filter = 'none';
        document.body.style.overflow = 'auto';
    }
</script>

</body>
</html>
