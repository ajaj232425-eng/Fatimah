<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>منصة التميز التربوي | القائدة فاطمه آل بحري</title>
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

        /* الهيدر الفاخر */
        header {
            background: linear-gradient(45deg, var(--primary), #004d39);
            color: white;
            padding: 50px 20px;
            text-align: center;
            border-bottom: 8px solid var(--gold);
            border-bottom-left-radius: 100px;
        }

        .header-container img { width: 130px; margin-bottom: 15px; filter: brightness(0) invert(1); }
        .header-container h1 { font-size: 2.2em; margin: 10px 0; text-shadow: 2px 2px 4px rgba(0,0,0,0.3); }

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
            border-right: 6px solid var(--gold);
            box-shadow: 2px 2px 10px rgba(0,0,0,0.02);
        }

        .info-card h4 { margin: 0 0 10px 0; color: var(--primary); }
        .info-card p { margin: 0; font-size: 0.95em; color: #555; }

        /* قسم جواز السفر الذكي */
        .passport-section { margin-top: 50px; }

        .passport-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .passport-item {
            background: var(--white);
            padding: 25px;
            border-radius: 25px;
            text-align: center;
            transition: 0.4s;
            cursor: pointer;
            border: 2px solid transparent;
        }

        .passport-item:hover {
            border-color: var(--gold);
            transform: translateY(-10px);
            box-shadow: 0 15px 35px rgba(0,0,0,0.1);
        }

        .passport-item i { font-size: 40px; color: var(--primary); margin-bottom: 15px; }
        .passport-item h3 { font-size: 1.1em; margin-bottom: 10px; }

        /* التذييل */
        footer {
            margin-top: 60px;
            background: var(--primary);
            color: white;
            padding: 40px 20px;
            text-align: center;
        }

        .signature { font-size: 1.5em; font-weight: bold; color: var(--gold); margin-top: 10px; display: block; }

        /* Modal للتفاعل */
        .modal {
            display: none;
            position: fixed;
            top: 50%; left: 50%;
            transform: translate(-50%, -50%);
            background: white;
            padding: 30px;
            border-radius: 25px;
            box-shadow: 0 0 50px rgba(0,0,0,0.3);
            z-index: 1001;
            width: 85%; max-width: 450px;
            text-align: center;
        }
        .overlay { display: none; position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.6); z-index: 1000; }
    </style>
</head>
<body>

<header>
    <div class="header-container">
        <img src="https://upload.wikimedia.org/wikipedia/commons/1/11/Ministry_of_Education_Saudi_Arabia_Logo.svg" alt="وزارة التعليم">
        <h1>منصة الإنجاز والشفافية الرقمية</h1>
        <p>بوابة القائدة التربوية لتطوير جيل المستقبل</p>
    </div>
</header>

<div class="container">
    
    <section class="transparent-kindergarten">
        <div class="section-title">
            <i class="fas fa-eye"></i> الروضة الشفافة (تواصل أسبوعي)
        </div>
        <div class="transparency-grid">
            <div class="info-card">
                <h4><i class="fas fa-star" style="color:var(--gold)"></i> قيمة الأسبوع</h4>
                <p>"بِر الوالدين" - نزرع فيهم حب العائلة والتقدير.</p>
            </div>
            <div class="info-card">
                <h4><i class="fas fa-apple-alt" style="color:#e74c3c"></i> الطبق الصحي</h4>
                <p>هذا الأسبوع نركز على: "الفواكه الملونة" لطاقة أكبر.</p>
            </div>
            <div class="info-card">
                <h4><i class="fas fa-calendar-check" style="color:var(--secondary)"></i> نشاط الخميس</h4>
                <p>مهرجان "الألوان والمرح" في الساحة الخارجية.</p>
            </div>
        </div>
    </section>

    <section class="passport-section">
        <div class="section-title">
            <i class="fas fa-passport"></i> جواز السفر الذكي للمهارات
        </div>
        <p style="color:#666; margin-bottom:20px;">انقر على المهارة لمعرفة خطتنا في تطوير طفلك:</p>
        
        <div class="passport-grid">
            <div class="passport-item" onclick="openSkill('مهارة الاستقلال', 'ندرب الطفل على الاعتماد على نفسه في ارتداء ملابسه وتناول طعامه وترتيب أدواته، مما يبني شخصية واثقة.')">
                <i class="fas fa-child"></i>
                <h3>الاستقلال الذاتي</h3>
            </div>
            <div class="passport-item" onclick="openSkill('الطلاقة اللغوية', 'برامج مكثفة لإثراء حصيلة الطفل اللغوية من خلال القراءة القصصية والتعبير اليومي.')">
                <i class="fas fa-comments"></i>
                <h3>الطلاقة اللغوية</h3>
            </div>
            <div class="passport-item" onclick="openSkill('الذكاء الوجداني', 'تعليم الطفل كيف يفهم مشاعره ومشاعر الآخرين، وكيف يتعامل معها بذكاء وهدوء.')">
                <i class="fas fa-heart"></i>
                <h3>الذكاء الوجداني</h3>
            </div>
            <div class="passport-item" onclick="openSkill('مهارات المستقبل', 'مبادئ التفكير المنطقي وحل المشكلات البسيطة بأسلوب ترفيهي رقمي.')">
                <i class="fas fa-laptop-code"></i>
                <h3>مهارات المستقبل</h3>
            </div>
        </div>
    </section>

</div>

<footer>
    <p>هذه المنصة تعكس رؤية التطوير والشفافية لعام 2026</p>
    <p>تحت إشراف مديرة الروضة:</p>
    <span class="signature">فاطمه صالح آل بحري</span>
    <p style="margin-top:20px; font-size:0.8em; opacity:0.7;">إدارة تعليم نجران - المملكة العربية السعودية</p>
</footer>

<div class="overlay" id="overlay" onclick="closeSkill()"></div>
<div class="modal" id="modal">
    <h3 id="skillTitle" style="color:var(--primary);"></h3>
    <p id="skillDesc" style="line-height:1.7; color:#444;"></p>
    <button onclick="closeSkill()" style="background:var(--primary); color:white; border:none; padding:10px 25px; border-radius:12px; cursor:pointer; margin-top:15px;">شكراً لكم</button>
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
