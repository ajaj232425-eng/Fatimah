<! فكره أ/ فاطمه صالح نحو الاستدامه>
< rt<! >
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
            --bg: #f4f7f6;
        }

        body { font-family: 'Segoe UI', Tahoma, sans-serif; margin: 0; background-color: var(--bg); color: #333; overflow-x: hidden; }

        /* الهيدر */
        header {
            background: linear-gradient(135deg, var(--primary), #004d39);
            color: white; padding: 50px 20px; text-align: center; border-bottom: 8px solid var(--gold);
            border-bottom-left-radius: 60px;
        }

        .header-container img { width: 120px; filter: brightness(0) invert(1); margin-bottom: 10px; }

        .container { max-width: 1100px; margin: auto; padding: 20px; }

        /* --- قسم الروضة الشفافة --- */
        .transparency-section {
            background: white; padding: 25px; border-radius: 25px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.05);
            margin-top: -50px; margin-bottom: 40px; border: 1px solid #eee;
        }

        .section-title {
            color: var(--primary); font-size: 1.5em; margin-bottom: 20px;
            border-right: 5px solid var(--gold); padding-right: 15px; display: flex; align-items: center; gap: 10px;
        }

        .transparency-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; }
        .info-card { background: #fafafa; padding: 15px; border-radius: 15px; border-bottom: 3px solid var(--gold); }

        /* --- قسم جواز السفر --- */
        .passport-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 20px; }
        .passport-item {
            background: white; padding: 30px 15px; border-radius: 20px; text-align: center;
            cursor: pointer; border: 1px solid #eee; transition: 0.3s;
        }
        .passport-item i { font-size: 40px; color: var(--primary); margin-bottom: 15px; }

        /* --- الحل الجذري والنهائي للانبثاق للأمام --- */
        #fixed-overlay-layer {
            display: none;
            position: fixed;
            top: 0; left: 0;
            width: 100vw; height: 100vh;
            background: rgba(0, 0, 0, 0.85); /* تعتيم خلفية الموقع */
            z-index: 2147483647 !important; /* أعلى طبقة برمجية موجودة */
            justify-content: center; align-items: center;
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
        }

        .pop-card {
            background: white; width: 85%; max-width: 400px;
            padding: 35px; border-radius: 30px; text-align: center;
            border-top: 10px solid var(--gold);
            box-shadow: 0 25px 50px rgba(0,0,0,0.5);
            /* تأثير الانبثاق */
            animation: popForward 0.3s ease-out forwards;
            position: relative;
        }

        @keyframes popForward {
            from { transform: scale(0.7); opacity: 0; }
            to { transform: scale(1); opacity: 1; }
        }

        .close-btn {
            background: var(--primary); color: white; border: none;
            padding: 10px 35px; border-radius: 12px; cursor: pointer;
            margin-top: 20px; font-weight: bold; font-size: 1.1em;
        }

        /* تذييل الصفحة */
        footer {
            background: var(--primary); color: white; padding: 50px 20px;
            text-align: center; margin-top: 60px; border-top: 5px solid var(--gold);
        }
        .my-name { font-size: 2em; color: var(--gold); font-weight: bold; margin-bottom: 5px; }
    </style>
</head>
<body>

    <header>
        <div class="header-container">
            <img src="https://upload.wikimedia.org/wikipedia/commons/1/11/Ministry_of_Education_Saudi_Arabia_Logo.svg">
            <h1>منصة الإنجاز والشفافية</h1>
            <p style="color: var(--gold); font-weight: bold;">بوابة القائدة الملهمة</p>
        </div>
    </header>

    <div class="container">
        <section class="transparency-section">
            <div class="section-title"><i class="fas fa-bullhorn"></i> الروضة الشفافة</div>
            <div class="transparency-grid">
                <div class="info-card">
                    <h4 style="margin:0; color:var(--primary)">قيمة الأسبوع</h4>
                    <p style="font-size:0.9em">"التعاون والمشاركة" - نعزز روح الفريق بين الأطفال.</p>
                </div>
                <div class="info-card">
                    <h4 style="margin:0; color:var(--primary)">صحة المبدعين</h4>
                    <p style="font-size:0.9em">التركيز على شرب الماء وتناول الخضروات الورقية.</p>
                </div>
            </div>
        </section>

        <h2 style="text-align: center; color: var(--primary); margin-bottom: 30px;">جواز السفر الذكي للمهارات</h2>
        <div class="passport-grid">
            <div class="passport-item" onclick="showMe('الاستقلال الذاتي', 'تمكين الطفل من الاعتماد على نفسه وبناء شخصية مستقلة وواثقة.')">
                <i class="fas fa-user-check"></i>
                <h3>الاستقلال الذاتي</h3>
            </div>
            <div class="passport-item" onclick="showMe('الطلاقة اللغوية', 'تطوير مهارات التعبير وسرد القصص بأسلوب لغوي سليم.')">
                <i class="fas fa-comments"></i>
                <h3>الطلاقة اللغوية</h3>
            </div>
            <div class="passport-item" onclick="showMe('الذكاء الوجداني', 'فهم المشاعر وبناء علاقات اجتماعية إيجابية مع الأقران.')">
                <i class="fas fa-heart"></i>
                <h3>الذكاء الوجداني</h3>
            </div>
            <div class="passport-item" onclick="showMe('مهارات المستقبل', 'تنمية التفكير الإبداعي وحل المشكلات بوعي رقمي حديث.')">
                <i class="fas fa-rocket"></i>
                <h3>مهارات المستقبل</h3>
            </div>
        </div>
    </div>

    <div id="fixed-overlay-layer">
        <div class="pop-card">
            <div style="font-size: 50px; color: var(--gold); margin-bottom: 10px;"><i class="fas fa-certificate"></i></div>
            <h2 id="p-title" style="color: var(--primary); margin-bottom: 15px;"></h2>
            <p id="p-desc" style="line-height: 1.8; color: #444; font-size: 1.1em;"></p>
            <button class="close-btn" onclick="hideMe()">إغلاق</button>
        </div>
    </div>

    <footer>
        <div class="my-name">فاطمه صالح آل بحري</div>
        <p>القائدة التربوية الملهمة</p>
        <p>نصنع الأثر.. ونبني الأجيال</p>
    </footer>

    <script>
        function showMe(title, desc) {
            document.getElementById('p-title').innerText = title;
            document.getElementById('p-desc').innerText = desc;
            document.getElementById('fixed-overlay-layer').style.display = 'flex';
            document.body.style.overflow = 'hidden'; // تجميد الصفحة
        }

        function hideMe() {
            document.getElementById('fixed-overlay-layer').style.display = 'none';
            document.body.style.overflow = 'auto'; // إعادة الحركة
        }
    </script>
</body>
</html>
