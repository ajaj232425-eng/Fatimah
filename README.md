<! فكره أ/ فاطمه صالح نحو الاستدامه>
<!l>
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
            --white: #ffffff;
            --bg: #f8fbf9;
        }

        body { font-family: 'Segoe UI', Tahoma, sans-serif; margin: 0; background-color: var(--bg); overflow-x: hidden; }

        /* الهيدر */
        header {
            background: linear-gradient(135deg, var(--primary), #004d39);
            color: white; padding: 50px 20px; text-align: center; border-bottom: 8px solid var(--gold);
        }

        .container { max-width: 1000px; margin: auto; padding: 20px; position: relative; z-index: 1; }

        /* كروت المهارات */
        .passport-grid {
            display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 20px; margin-top: 30px;
        }

        .passport-item {
            background: white; padding: 30px; border-radius: 25px; text-align: center;
            cursor: pointer; border: 1px solid #eee; transition: 0.3s;
            position: relative; z-index: 5; /* طبقة منخفضة مقارنة بالنافذة */
        }

        .passport-item i { font-size: 45px; color: var(--primary); margin-bottom: 15px; }

        /* الحل الجذري: النافذة المنبثقة للأمام */
        #exclusive-layer {
            display: none;
            position: fixed;
            top: 0; left: 0;
            width: 100%; height: 100%;
            background: rgba(0, 0, 0, 0.9); /* تعتيم كلي للخلفية */
            z-index: 1000000 !important; /* طبقة مليون لضمان الانبثاق للأمام */
            justify-content: center;
            align-items: center;
            backdrop-filter: blur(15px); /* غبش قوي جداً للأيقونات بالخلف */
        }

        .modal-card {
            background: white;
            width: 85%; max-width: 450px;
            padding: 40px;
            border-radius: 35px;
            text-align: center;
            position: relative;
            box-shadow: 0 30px 60px rgba(0,0,0,0.5);
            border-top: 12px solid var(--gold);
            transform: scale(0.7); /* تبدأ صغيرة لتنبثق */
            animation: popForward 0.4s forwards cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }

        @keyframes popForward {
            to { transform: scale(1); } /* تنبثق للأمام */
        }

        .btn-close {
            background: var(--primary); color: white; border: none;
            padding: 12px 40px; border-radius: 15px; cursor: pointer;
            margin-top: 25px; font-weight: bold; font-size: 1.1em;
        }

        /* تذييل الصفحة */
        footer {
            background: var(--primary); color: white; padding: 60px 20px;
            text-align: center; margin-top: 50px; border-top: 5px solid var(--gold);
        }

        .footer-name { font-size: 2em; color: var(--gold); font-weight: bold; margin-bottom: 10px; }
    </style>
</head>
<body>

<div id="main-content">
    <header>
        <img src="https://upload.wikimedia.org/wikipedia/commons/1/11/Ministry_of_Education_Saudi_Arabia_Logo.svg" width="130" style="filter: brightness(0) invert(1);">
        <h1>منصة الإنجاز والشفافية</h1>
        <p>بوابة القائدة الملهمة</p>
    </header>

    <div class="container">
        <h2 style="text-align: center; color: var(--primary); font-size: 1.8em;">جواز السفر الذكي للمهارات</h2>
        
        <div class="passport-grid">
            <div class="passport-item" onclick="showModal('الاستقلال الذاتي', 'تمكين الطفل من الاعتماد على نفسه في مهاراته الحياتية وبناء شخصية مستقلة.')">
                <i class="fas fa-user-check"></i>
                <h3>الاستقلال الذاتي</h3>
            </div>
            <div class="passport-item" onclick="showModal('الطلاقة اللغوية', 'تعزيز القدرة على التعبير اللغوي وسرد القصص والحوار الواثق.')">
                <i class="fas fa-comments"></i>
                <h3>الطلاقة اللغوية</h3>
            </div>
            <div class="passport-item" onclick="showModal('الذكاء الوجداني', 'تنمية فهم المشاعر وبناء علاقات اجتماعية إيجابية مع الأقران.')">
                <i class="fas fa-heart"></i>
                <h3>الذكاء الوجداني</h3>
            </div>
            <div class="passport-item" onclick="showModal('مهارات المستقبل', 'تنمية مهارات التفكير المنطقي والابتكار الرقمي لمواكبة المستقبل.')">
                <i class="fas fa-rocket"></i>
                <h3>مهارات المستقبل</h3>
            </div>
        </div>
    </div>

    <footer>
        <div class="footer-name">فاطمه صالح آل بحري</div>
        <p>القائدة التربوية الملهمة</p>
        <p>نصنع الأثر.. ونبني الأجيال</p>
        <p style="margin-top: 20px; font-size: 0.8em; opacity: 0.7;">جميع الحقوق محفوظة © 2026</p>
    </footer>
</div>

<div id="exclusive-layer">
    <div class="modal-card">
        <div style="font-size: 60px; color: var(--gold); margin-bottom: 20px;"><i class="fas fa-award"></i></div>
        <h2 id="modal-title" style="color: var(--primary); font-size: 1.6em;"></h2>
        <p id="modal-desc" style="line-height: 1.8; color: #444; font-size: 1.1em;"></p>
        <button class="btn-close" onclick="hideModal()">إغلاق</button>
    </div>
</div>

<script>
    function showModal(title, desc) {
        document.getElementById('modal-title').innerText = title;
        document.getElementById('modal-desc').innerText = desc;
        document.getElementById('exclusive-layer').style.display = 'flex';
        // منع التمرير في الخلفية
        document.body.style.overflow = 'hidden';
    }

    function hideModal() {
        document.getElementById('exclusive-layer').style.display = 'none';
        document.body.style.overflow = 'auto';
    }
</script>

</body>
</html>
