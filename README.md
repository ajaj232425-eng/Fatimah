<! فكره أ/ فاطمه صالح نحو الاستدامه>
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
        
        /* --- تنسيق المنسدلات العام --- */
        .collapse-item { background: var(--white); margin-bottom: 12px; border-radius: 15px; border: 1px solid #eee; overflow: hidden; transition: 0.3s; box-shadow: 0 4px 10px rgba(0,0,0,0.03); }
        .collapse-header { padding: 18px; display: flex; align-items: center; justify-content: space-between; cursor: pointer; }
        .collapse-header .title-side { display: flex; align-items: center; gap: 12px; }
        .collapse-header i.main-icon { color: var(--gold); font-size: 1.3em; width: 30px; text-align: center; }
        .collapse-header h3 { margin: 0; font-size: 1.05em; color: var(--primary); }
        
        .collapse-content { max-height: 0; overflow: hidden; transition: 0.4s ease-out; background: #fafafa; }
        .collapse-item.active { border-color: var(--gold); }
        .collapse-item.active .collapse-content { max-height: 300px; border-top: 1px solid #eee; }
        .collapse-item.active .chevron { transform: rotate(180deg); }
        .chevron { transition: 0.3s; color: var(--gold); }
        .content-text { padding: 20px; color: #555; font-size: 0.95em; }

        /* أيقونة الأسئلة */
        #qa-modal { display: none; position: fixed; bottom: 100px; left: 30px; width: 300px; background: white; border-radius: 20px; box-shadow: 0 10px 30px rgba(0,0,0,0.2); z-index: 2000; flex-direction: column; border: 1px solid #eee; }
        .qa-header { background: var(--primary); color: white; padding: 15px; font-weight: bold; display: flex; justify-content: space-between; border-radius: 20px 20px 0 0; }
        .qa-body { padding: 15px; }
        .qa-body textarea { width: 100%; border: 1px solid #ddd; border-radius: 10px; padding: 10px; resize: none; font-family: inherit; box-sizing: border-box; }
        .qa-body button { background: var(--gold); color: white; border: none; width: 100%; padding: 10px; border-radius: 10px; margin-top: 10px; cursor: pointer; font-weight: bold; }

        .qa-float { position: fixed; bottom: 30px; left: 30px; background: var(--gold); color: white; width: 60px; height: 60px; border-radius: 50%; display: flex; justify-content: center; align-items: center; font-size: 25px; cursor: pointer; z-index: 1000; box-shadow: 0 8px 20px rgba(0,0,0,0.2); }
        
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
        
        <h2 style="color: var(--primary); text-align: center; font-size: 1.3em; margin-bottom: 20px;"><i class="fas fa-eye"></i> الروضة الشفافة</h2>
        
        <div class="collapse-item">
            <div class="collapse-header" onclick="toggleItem(this)">
                <div class="title-side"><i class="fas fa-star main-icon"></i> <h3>قيمة الأسبوع</h3></div>
                <i class="fas fa-chevron-down chevron"></i>
            </div>
            <div class="collapse-content"><div class="content-text">قيمة هذا الأسبوع هي "المواطنة المسؤولة"، نغرس في نفوس أطفالنا حب الوطن والمحافظة على ممتلكاته.</div></div>
        </div>

        <div class="collapse-item">
            <div class="collapse-header" onclick="toggleItem(this)">
                <div class="title-side"><i class="fas fa-apple-alt main-icon"></i> <h3>صحة المبدعين</h3></div>
                <i class="fas fa-chevron-down chevron"></i>
            </div>
            <div class="collapse-content"><div class="content-text">نهتم بتقديم وجبات صحية متوازنة، ونشجع أطفالنا على ممارسة الأنشطة الحركية الصباحية بانتظام.</div></div>
        </div>

        <div class="collapse-item" style="border-right: 6px solid var(--primary);">
            <div class="collapse-header" onclick="toggleItem(this)">
                <div class="title-side"><i class="fas fa-lightbulb main-icon" style="color: var(--primary);"></i> <h3>المبادرة الأسبوعية الاجتماعية</h3></div>
                <i class="fas fa-chevron-down chevron"></i>
            </div>
            <div class="collapse-content">
                <div class="content-text" style="background: #eef7f2;">
                    <strong>مبادرة (بصمتي الاجتماعية):</strong> <br>
                    مبادرة تهدف لتعزيز صلة الرحم، حيث نطلب من الطفل هذا الأسبوع إجراء اتصال مرئي بجدّه أو جدّته لتعزيز قيم الوفاء.
                </div>
            </div>
        </div>

        <h2 style="text-align: center; color: var(--primary); margin: 30px 0 20px 0;"><i class="fas fa-passport"></i> جواز السفر الإلكتروني للمهارات</h2>
        
        <div class="collapse-item">
            <div class="collapse-header" onclick="toggleItem(this)">
                <div class="title-side"><i class="fas fa-child main-icon"></i> <h3>الاستقلال الذاتي</h3></div>
                <i class="fas fa-chevron-down chevron"></i>
            </div>
            <div class="collapse-content"><div class="content-text">بناء شخصية الطفل ليعتمد على ذاته في اتخاذ قراراته اليومية الصغيرة بمسؤولية وثقة.</div></div>
        </div>

        <div class="collapse-item">
            <div class="collapse-header" onclick="toggleItem(this)">
                <div class="title-side"><i class="fas fa-comments main-icon"></i> <h3>الطلاقة اللغوية</h3></div>
                <i class="fas fa-chevron-down chevron"></i>
            </div>
            <div class="collapse-content"><div class="content-text">تمكين الطفل من مهارات الحوار والتعبير بوضوح، مما يعزز ثقته في الحديث أمام الآخرين.</div></div>
        </div>

        <div class="collapse-item">
            <div class="collapse-header" onclick="toggleItem(this)">
                <div class="title-side"><i class="fas fa-heart main-icon"></i> <h3>الذكاء الوجداني</h3></div>
                <i class="fas fa-chevron-down chevron"></i>
            </div>
            <div class="collapse-content"><div class="content-text">تنمية مهارات التعاطف وفهم المشاعر، لبناء جيل يقدر الآخرين ويتعامل معهم برقي.</div></div>
        </div>

        <div class="collapse-item">
            <div class="collapse-header" onclick="toggleItem(this)">
                <div class="title-side"><i class="fas fa-rocket main-icon"></i> <h3>مهارات المستقبل</h3></div>
                <i class="fas fa-chevron-down chevron"></i>
            </div>
            <div class="collapse-content"><div class="content-text">تأسيس مهارات التفكير الإبداعي والابتكار الرقمي لمواكبة متطلبات العصر الحديث.</div></div>
        </div>

    </div>

    <div id="qa-modal">
        <div class="qa-header"><span>اسأل القائدة</span><i class="fas fa-times" onclick="toggleQA()" style="cursor:pointer"></i></div>
        <div class="qa-body">
            <textarea id="userQ" rows="4" placeholder="اكتب سؤالكِ هنا..."></textarea>
            <button onclick="sendQ()">إرسال السؤال</button>
        </div>
    </div>

    <div class="qa-float" onclick="toggleQA()"><i class="fas fa-question"></i></div>

    <footer>
        <div class="footer-name">فاطمه صالح آل بحري</div>
        <p>القائدة التربوية الملهمة</p>
        <p>نحو تعليم مستدام يبني الإنسان ويحيي الأثر</p>
    </footer>

    <script>
        function toggleItem(el) {
            const item = el.parentElement;
            // إغلاق أي منسدلة أخرى مفتوحة لضمان الترتيب
            document.querySelectorAll('.collapse-item').forEach(i => {
                if (i !== item) i.classList.remove('active');
            });
            item.classList.toggle('active');
        }

        function toggleQA() {
            const m = document.getElementById('qa-modal');
            m.style.display = (m.style.display === 'flex') ? 'none' : 'flex';
        }

        function sendQ() {
            const q = document.getElementById('userQ').value;
            if(!q.trim()) return alert("يرجى كتابة السؤال");
            alert("تم إرسال سؤالكِ بنجاح أستاذة فاطمه، سيتم الرد قريباً.");
            document.getElementById('userQ').value = "";
            toggleQA();
        }
    </script>
</body>
</html>
