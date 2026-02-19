<! فكره أ/ فاطمه صالح نحو الاستدامه>
< rt
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>منصة الإنجاز والشفافية | فاطمه صالح آل بحري</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        :root { --primary: #006d51; --gold: #d4af37; --bg: #f8fbf9; --white: #ffffff; }
        body { font-family: 'Segoe UI', Tahoma, sans-serif; margin: 0; background-color: var(--bg); color: #333; line-height: 1.6; }
        
        header { 
            background: linear-gradient(135deg, var(--primary), #004d39); 
            color: white; padding: 40px 20px; text-align: center; 
            border-bottom: 6px solid var(--gold);
            border-bottom-left-radius: 40px; border-bottom-right-radius: 40px;
        }

        .container { max-width: 900px; margin: auto; padding: 20px; }
        
        /* الروضة الشفافة */
        .transparency-box { 
            background: var(--white); padding: 20px; border-radius: 20px; 
            box-shadow: 0 10px 25px rgba(0,0,0,0.05); 
            margin-top: -50px; margin-bottom: 30px; 
            border-right: 8px solid var(--gold); 
        }

        /* جواز السفر الإلكتروني - المنسدلة */
        .passport-section { margin-top: 20px; }
        .skill-item { background: var(--white); margin-bottom: 12px; border-radius: 15px; border: 1px solid #eee; overflow: hidden; transition: 0.3s; }
        .skill-header { padding: 18px; display: flex; align-items: center; justify-content: space-between; cursor: pointer; font-weight: bold; color: var(--primary); }
        .skill-header i.main-icon { margin-left: 10px; color: var(--gold); font-size: 1.2em; }
        .skill-content { max-height: 0; overflow: hidden; transition: 0.4s ease-out; background: #fafafa; }
        .skill-item.active { border-color: var(--gold); box-shadow: 0 5px 15px rgba(0,0,0,0.05); }
        .skill-item.active .skill-content { max-height: 500px; border-top: 1px solid #eee; }
        .skill-item.active .chevron { transform: rotate(180deg); }
        .chevron { transition: 0.3s; color: var(--gold); }

        /* مبادرة الاستدامة */
        .social-impact-box {
            background: linear-gradient(135deg, #eef7f2, #ffffff);
            padding: 20px; border-radius: 20px; border: 2px solid var(--primary); 
            margin-top: 30px; text-align: center;
        }

        /* نافذة الأسئلة التفاعلية */
        #qa-modal {
            display: none; position: fixed; bottom: 100px; left: 30px;
            width: 300px; background: white; border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2); z-index: 2000;
            flex-direction: column; overflow: hidden; border: 1px solid #eee;
            animation: slideUp 0.3s ease-out;
        }
        @keyframes slideUp { from { transform: translateY(20px); opacity: 0; } to { transform: translateY(0); opacity: 1; } }
        .qa-header { background: var(--primary); color: white; padding: 15px; font-weight: bold; display: flex; justify-content: space-between; }
        .qa-body { padding: 15px; }
        .qa-body textarea { width: 100%; border: 1px solid #ddd; border-radius: 10px; padding: 10px; resize: none; font-family: inherit; }
        .qa-body button { background: var(--gold); color: white; border: none; width: 100%; padding: 10px; border-radius: 10px; margin-top: 10px; cursor: pointer; font-weight: bold; }

        /* أيقونة الأسئلة العائمة */
        .qa-float { 
            position: fixed; bottom: 30px; left: 30px; 
            background: var(--gold); color: white; 
            width: 60px; height: 60px; border-radius: 50%; 
            display: flex; justify-content: center; align-items: center; 
            font-size: 25px; cursor: pointer; z-index: 1000; 
            box-shadow: 0 8px 20px rgba(0,0,0,0.2); 
        }
        
        footer { background: var(--primary); color: white; padding: 40px 20px; text-align: center; margin-top: 50px; border-top: 5px solid var(--gold); }
        .footer-name { font-size: 1.8em; color: var(--gold); font-weight: bold; }
    </style>
</head>
<body>

    <header>
        <img src="https://upload.wikimedia.org/wikipedia/commons/1/11/Ministry_of_Education_Saudi_Arabia_Logo.svg" width="100" style="filter: brightness(0) invert(1); margin-bottom: 10px;">
        <h1>منصة الإنجاز والشفافية</h1>
        <p>بوابة القائدة الملهمة: فاطمه صالح آل بحري</p>
    </header>

    <div class="container">
        
        <div class="transparency-box">
            <h3 style="color: var(--primary); margin: 0 0 10px 0;"><i class="fas fa-bullhorn"></i> الروضة الشفافة</h3>
            <p>نشارككم بكل شفافية قيمنا الأسبوعية لبناء جيل واعي ومسؤول.</p>
        </div>

        <h2 style="text-align: center; color: var(--primary);"><i class="fas fa-passport"></i> جواز السفر الإلكتروني للمهارات</h2>
        
        <div class="passport-section">
            <div class="skill-item">
                <div class="skill-header" onclick="toggleSkill(this)">
                    <span><i class="fas fa-child main-icon"></i> الاستقلال الذاتي</span>
                    <i class="fas fa-chevron-down chevron"></i>
                </div>
                <div class="skill-content">
                    <p style="padding: 20px;"><strong>الهدف الاجتماعي:</strong> تمكين الطفل من الاعتماد على نفسه ليكون عنصراً فعالاً ومستقلاً في أسرته ومجتمعه الصغير.</p>
                </div>
            </div>

            <div class="skill-item">
                <div class="skill-header" onclick="toggleSkill(this)">
                    <span><i class="fas fa-comments main-icon"></i> الطلاقة اللغوية</span>
                    <i class="fas fa-chevron-down chevron"></i>
                </div>
                <div class="skill-content">
                    <p style="padding: 20px;"><strong>الهدف الاجتماعي:</strong> تطوير قدرة الطفل على التواصل والحوار البنّاء، مما يعزز مهارات الإقناع والتفاعل الاجتماعي الإيجابي.</p>
                </div>
            </div>

            <div class="skill-item">
                <div class="skill-header" onclick="toggleSkill(this)">
                    <span><i class="fas fa-heart main-icon"></i> الذكاء الوجداني</span>
                    <i class="fas fa-chevron-down chevron"></i>
                </div>
                <div class="skill-content">
                    <p style="padding: 20px;"><strong>الهدف الاجتماعي:</strong> غرس قيم التعاطف وفهم مشاعر الآخرين لبناء مجتمع تعليمي متماسك يسوده الاحترام المتبادل.</p>
                </div>
            </div>
        </div>

        <div class="social-impact-box">
            <h3 style="color: var(--primary);"><i class="fas fa-seedling"></i> مبادرة غرس الاستدامة الاجتماعية</h3>
            <p><strong>تحدي الأسبوع:</strong> ساعد طفلك على القيام بعمل تطوعي بسيط في المنزل وحدثه عن أثر العطاء.</p>
        </div>

    </div>

    <div id="qa-modal">
        <div class="qa-header">
            <span>اسأل القائدة</span>
            <i class="fas fa-times" style="cursor:pointer" onclick="toggleQA()"></i>
        </div>
        <div class="qa-body">
            <textarea id="userQuestion" rows="4" placeholder="اكتب استفسارك هنا..."></textarea>
            <button onclick="sendQuestion()">إرسال الاستفسار</button>
        </div>
    </div>

    <div class="qa-float" onclick="toggleQA()">
        <i class="fas fa-question"></i>
    </div>

    <footer>
        <div class="footer-name">فاطمه صالح آل بحري</div>
        <p>القائدة التربوية الملهمة</p>
        <p>نحو تعليم مستدام يبني الإنسان ويحيي الأثر</p>
    </footer>

    <script>
        // دالة المنسدلة
        function toggleSkill(el) {
            const item = el.parentElement;
            document.querySelectorAll('.skill-item').forEach(i => {
                if (i !== item) i.classList.remove('active');
            });
            item.classList.toggle('active');
        }

        // دالة إظهار/إخفاء صندوق الأسئلة
        function toggleQA() {
            const modal = document.getElementById('qa-modal');
            modal.style.display = (modal.style.display === 'flex') ? 'none' : 'flex';
        }

        // دالة إرسال السؤال (تفاعلية)
        function sendQuestion() {
            const question = document.getElementById('userQuestion').value;
            if (question.trim() === "") {
                alert("يرجى كتابة السؤال أولاً");
                return;
            }
            alert("شكرًا لكِ أستاذة فاطمه، تم استلام السؤال بنجاح وسيتم الرد قريباً.");
            document.getElementById('userQuestion').value = "";
            toggleQA();
        }
    </script>
</body>
</html>
