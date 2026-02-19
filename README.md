<! فكره أ/ فاطمه صالح نحو الاستدامه>
< rt
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
            --bg: #f8fbf9;
            --white: #ffffff;
        }

        body { font-family: 'Segoe UI', Tahoma, sans-serif; margin: 0; background-color: var(--bg); color: #333; line-height: 1.6; }

        header {
            background: linear-gradient(135deg, var(--primary), #004d39);
            color: white; padding: 40px 20px; text-align: center; border-bottom: 6px solid var(--gold);
        }

        .container { max-width: 900px; margin: auto; padding: 20px; }

        /* --- الروضة الشفافة --- */
        .transparency-box {
            background: var(--white); padding: 20px; border-radius: 20px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05); margin-top: -40px; margin-bottom: 30px;
            border-right: 6px solid var(--gold);
        }

        /* --- شبكة المهارات بنظام القائمة المنسدلة --- */
        .skill-item {
            background: var(--white); margin-bottom: 15px; border-radius: 15px;
            overflow: hidden; border: 1px solid #eee; box-shadow: 0 2px 5px rgba(0,0,0,0.02);
        }

        .skill-header {
            padding: 20px; display: flex; align-items: center; justify-content: space-between;
            cursor: pointer; transition: background 0.3s;
        }

        .skill-header:hover { background: #f0f7f4; }

        .skill-header .title-side { display: flex; align-items: center; gap: 15px; }
        .skill-header i.main-icon { font-size: 28px; color: var(--primary); width: 40px; text-align: center; }
        .skill-header h3 { margin: 0; font-size: 1.1em; color: var(--primary); }

        .chevron { transition: transform 0.3s; color: var(--gold); }

        /* محتوى المنسدلة */
        .skill-content {
            max-height: 0; overflow: hidden; transition: max-height 0.4s ease-out;
            background: #fafafa; border-top: 1px solid #f0f0f0;
        }

        .skill-content .inner-text { padding: 20px; color: #555; font-size: 1em; }

        /* حالة الفتح */
        .skill-item.active .skill-content { max-height: 200px; }
        .skill-item.active .chevron { transform: rotate(180deg); }
        .skill-item.active { border-color: var(--gold); }

        /* تذييل الصفحة */
        footer {
            background: var(--primary); color: white; padding: 40px 20px;
            text-align: center; margin-top: 50px; border-top: 5px solid var(--gold);
        }
        .my-name { font-size: 1.8em; color: var(--gold); font-weight: bold; margin-bottom: 5px; }
    </style>
</head>
<body>

    <header>
        <img src="https://upload.wikimedia.org/wikipedia/commons/1/11/Ministry_of_Education_Saudi_Arabia_Logo.svg" width="100" style="filter: brightness(0) invert(1);">
        <h1>منصة الإنجاز والشفافية</h1>
        <p>بوابة القائدة الملهمة</p>
    </header>

    <div class="container">
        <div class="transparency-box">
            <h3 style="color: var(--primary); margin-top: 0;"><i class="fas fa-eye"></i> الروضة الشفافة</h3>
            <p>نحرص على اطلاعكم الأسبوعي حول القيم والأنشطة التربوية لضمان رحلة تعليمية شفافة ومثمرة لأطفالنا.</p>
        </div>

        <h2 style="text-align: center; color: var(--primary); margin-bottom: 25px;">جواز السفر الذكي للمهارات</h2>

        <div class="skill-item">
            <div class="skill-header" onclick="toggleSkill(this)">
                <div class="title-side">
                    <i class="fas fa-user-check main-icon"></i>
                    <h3>الاستقلال الذاتي</h3>
                </div>
                <i class="fas fa-chevron-down chevron"></i>
            </div>
            <div class="skill-content">
                <div class="inner-text">
                    نعمل من خلال هذا المسار على تعزيز قدرة الطفل على تدبير شؤونه الخاصة، من تنظيم أدواته إلى اتخاذ قراراته البسيطة، مما يبني لديه شخصية قيادية معتمدة على ذاتها.
                </div>
            </div>
        </div>

        <div class="skill-item">
            <div class="skill-header" onclick="toggleSkill(this)">
                <div class="title-side">
                    <i class="fas fa-comments main-icon"></i>
                    <h3>الطلاقة اللغوية</h3>
                </div>
                <i class="fas fa-chevron-down chevron"></i>
            </div>
            <div class="skill-content">
                <div class="inner-text">
                    برنامج مكثف لتنمية مهارات التعبير وسرد القصص والحوار الواثق، لتمكين الطفل من إيصال أفكاره ومشاعره بطلاقة ووضوح.
                </div>
            </div>
        </div>

        <div class="skill-item">
            <div class="skill-header" onclick="toggleSkill(this)">
                <div class="title-side">
                    <i class="fas fa-heart main-icon"></i>
                    <h3>الذكاء الوجداني</h3>
                </div>
                <i class="fas fa-chevron-down chevron"></i>
            </div>
            <div class="skill-content">
                <div class="inner-text">
                    فهم مشاعر الطفل لنفسه وللآخرين، وتعليمه مهارات التعاطف وبناء العلاقات الاجتماعية الإيجابية التي تضمن له بيئة نفسية متزنة.
                </div>
            </div>
        </div>

        <div class="skill-item">
            <div class="skill-header" onclick="toggleSkill(this)">
                <div class="title-side">
                    <i class="fas fa-rocket main-icon"></i>
                    <h3>مهارات المستقبل</h3>
                </div>
                <i class="fas fa-chevron-down chevron"></i>
            </div>
            <div class="skill-content">
                <div class="inner-text">
                    تأسيس مهارات التفكير المنطقي والابتكار الرقمي، لتهيئة جيل مبدع قادر على مواكبة المتغيرات التقنية الحديثة برؤية طموحة.
                </div>
            </div>
        </div>

    </div>

    <footer>
        <div class="my-name">فاطمه صالح آل بحري</div>
        <p>القائدة التربوية الملهمة</p>
        <p>نصنع الأثر.. ونبني الأجيال</p>
    </footer>

    <script>
        function toggleSkill(element) {
            // إغلاق أي مهارة أخرى مفتوحة (اختياري)
            const items = document.querySelectorAll('.skill-item');
            items.forEach(item => {
                if(item !== element.parentElement) {
                    item.classList.remove('active');
                }
            });

            // فتح أو إغلاق المهارة الحالية
            const parent = element.parentElement;
            parent.classList.toggle('active');
        }
    </script>
</body>
</html>
