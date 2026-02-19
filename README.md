<! فكره أ/ فاطمه صالح نحو الاستدامه>
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>منصة الإنجاز والشفافية | فاطمه صالح آل بحري</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        :root { --primary: #006d51; --gold: #d4af37; --bg-overlay: rgba(248, 251, 249, 0.95); }
        
        body { 
            font-family: 'Segoe UI', Tahoma, sans-serif; margin: 0; 
            background-image: url('https://www.transparenttextures.com/patterns/arabesque.png'), linear-gradient(135deg, #f0f4f2 0%, #e6eee9 100%);
            background-attachment: fixed;
            color: #333; line-height: 1.6; 
        }
        
        header { 
            background: linear-gradient(135deg, var(--primary), #004d39); 
            color: white; padding: 40px 20px; text-align: center; 
            border-bottom: 6px solid var(--gold);
            border-bottom-left-radius: 50px; border-bottom-right-radius: 50px;
        }

        .container { max-width: 800px; margin: auto; padding: 20px; }
        
        .card-panel {
            background: var(--bg-overlay);
            backdrop-filter: blur(10px);
            padding: 25px; border-radius: 25px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.08);
            margin-bottom: 25px;
            border: 1px solid rgba(255,255,255,0.6);
        }

        h2 { color: var(--primary); font-size: 1.4em; border-bottom: 2px solid var(--gold); display: inline-block; margin-bottom: 20px; padding-bottom: 5px; }

        .collapse-item { background: white; margin-bottom: 12px; border-radius: 15px; border: 1px solid #eee; overflow: hidden; transition: 0.3s; }
        .collapse-header { padding: 18px; display: flex; align-items: center; justify-content: space-between; cursor: pointer; }
        .collapse-header i.main-icon { color: var(--gold); font-size: 1.3em; width: 35px; text-align: center; }
        .collapse-header h3 { margin: 0; font-size: 1.05em; color: var(--primary); }
        .collapse-content { max-height: 0; overflow: hidden; transition: 0.4s ease-out; background: #fafafa; }
        .collapse-item.active .collapse-content { max-height: 500px; border-top: 1px solid #eee; }
        .collapse-item.active .chevron { transform: rotate(180deg); }
        .chevron { transition: 0.3s; color: var(--gold); }
        .content-padding { padding: 20px; font-size: 0.95em; color: #555; }

        /* أيقونة الأسئلة المرتبطة بقوقل فورمس */
        .qa-float { 
            position: fixed; bottom: 30px; left: 30px; background: var(--gold); color: white; 
            width: 65px; height: 65px; border-radius: 50%; display: flex; 
            justify-content: center; align-items: center; font-size: 25px; 
            cursor: pointer; z-index: 1000; box-shadow: 0 10px 25px rgba(212,175,55,0.5);
            text-decoration: none; transition: 0.3s;
        }
        .qa-float:hover { transform: scale(1.1) rotate(10deg); background: var(--primary); }

        footer { background: var(--primary); color: white; padding: 40px 20px; text-align: center; margin-top: 50px; border-top: 5px solid var(--gold); }
    </style>
</head>
<body>

    <header>
        <img src="https://upload.wikimedia.org/wikipedia/commons/1/11/Ministry_of_Education_Saudi_Arabia_Logo.svg" width="100" style="filter: brightness(0) invert(1); margin-bottom: 10px;">
        <h1>منصة الإنجاز والشفافية</h1>
        <p style="color: var(--gold); font-weight: bold; font-size: 1.1em;">بوابة القائدة: فاطمه صالح آل بحري</p>
    </header>

    <div class="container">
        
        <div class="card-panel">
            <h2><i class="fas fa-bullhorn"></i> الروضة الشفافة</h2>
            
            <div class="collapse-item">
                <div class="collapse-header" onclick="toggleItem(this)">
                    <div style="display:flex; align-items:center; gap:10px;"><i class="fas fa-star main-icon"></i> <h3>القيم الأسبوعية</h3></div>
                    <i class="fas fa-chevron-down chevron"></i>
                </div>
                <div class="collapse-content"><div class="content-padding">نركز هذا الأسبوع على قيمة <b>"التعاون"</b>، حيث يتعلم الطفل أهمية العمل الجماعي ومساعدة الآخرين داخل الفصل وخارجه.</div></div>
            </div>

            <div class="collapse-item">
                <div class="collapse-header" onclick="toggleItem(this)">
                    <div style="display:flex; align-items:center; gap:10px;"><i class="fas fa-apple-alt main-icon"></i> <h3>الصحة والسلامة</h3></div>
                    <i class="fas fa-chevron-down chevron"></i>
                </div>
                <div class="collapse-content"><div class="content-padding">نحرص على تطبيق أعلى معايير السلامة، ونوصي أولياء الأمور بمتابعة النظام الغذائي المتوازن لتعزيز مناعة أطفالنا.</div></div>
            </div>

            <div class="collapse-item">
                <div class="collapse-header" onclick="toggleItem(this)">
                    <div style="display:flex; align-items:center; gap:10px;"><i class="fas fa-users main-icon"></i> <h3>الشراكة المجتمعية</h3></div>
                    <i class="fas fa-chevron-down chevron"></i>
                </div>
                <div class="collapse-content"><div class="content-padding">نفتح آفاق التواصل مع الأسرة والمجتمع لبناء بيئة تعليمية متكاملة تدعم نمو الطفل اجتماعياً ومعرفياً.</div></div>
            </div>

            <div class="collapse-item" style="border-right: 6px solid var(--primary);">
                <div class="collapse-header" onclick="toggleItem(this)">
                    <div style="display:flex; align-items:center; gap:10px;"><i class="fas fa-lightbulb main-icon" style="color:var(--primary)"></i> <h3>المبادرة الأسبوعية</h3></div>
                    <i class="fas fa-chevron-down chevron"></i>
                </div>
                <div class="collapse-content"><div class="content-padding" style="background:#eef7f2;"><b>مبادرة "أنا وأسرتي نغرس":</b> دعوة للأطفال لزراعة شتلة منزلية وتوثيق التجربة لتعزيز الوعي البيئي.</div></div>
            </div>
        </div>

        <div class="card-panel">
            <h2><i class="fas fa-passport"></i> جواز السفر الإلكتروني للمهارات</h2>
            
            <div class="collapse-item">
                <div class="collapse-header" onclick="toggleItem(this)">
                    <div style="display:flex; align-items:center; gap:10px;"><i class="fas fa-child main-icon"></i> <h3>الاستقلال الذاتي</h3></div>
                    <i class="fas fa-chevron-down chevron"></i>
                </div>
                <div class="collapse-content"><div class="content-padding">تمكين الطفل من مهارات العناية بالذات واتخاذ القرارات اليومية البسيطة بثقة.</div></div>
            </div>

            <div class="collapse-item">
                <div class="collapse-header" onclick="toggleItem(this)">
                    <div style="display:flex; align-items:center; gap:10px;"><i class="fas fa-comments main-icon"></i> <h3>الطلاقة اللغوية</h3></div>
                    <i class="fas fa-chevron-down chevron"></i>
                </div>
                <div class="collapse-content"><div class="content-padding">تطوير مهارات التحدث والاستماع، وبناء حصيلة لغوية تساعد الطفل على التعبير عن مشاعره بوضوح.</div></div>
            </div>

            <div class="collapse-item">
                <div class="collapse-header" onclick="toggleItem(this)">
                    <div style="display:flex; align-items:center; gap:10px;"><i class="fas fa-heart main-icon"></i> <h3>الذكاء الوجداني</h3></div>
                    <i class="fas fa-chevron-down chevron"></i>
                </div>
                <div class="collapse-content"><div class="content-padding">فهم المشاعر الذاتية وتعزيز التعاطف مع الأقران لبناء علاقات اجتماعية ناجحة.</div></div>
            </div>

            <div class="collapse-item">
                <div class="collapse-header" onclick="toggleItem(this)">
                    <div style="display:flex; align-items:center; gap:10px;"><i class="fas fa-puzzle-piece main-icon"></i> <h3>التفكير الإبداعي</h3></div>
                    <i class="fas fa-chevron-down chevron"></i>
                </div>
                <div class="collapse-content"><div class="content-padding">تحفيز الخيال لدى الطفل من خلال الأنشطة الفنية والحلول المبتكرة للمشكلات البسيطة.</div></div>
            </div>

            <div class="collapse-item">
                <div class="collapse-header" onclick="toggleItem(this)">
                    <div style="display:flex; align-items:center; gap:10px;"><i class="fas fa-users-cog main-icon"></i> <h3>العمل الجماعي</h3></div>
                    <i class="fas fa-chevron-down chevron"></i>
                </div>
                <div class="collapse-content"><div class="content-padding">غرس روح الفريق والمشاركة، وتعليم الطفل كيفية التفاعل الإيجابي مع المجموعة.</div></div>
            </div>

            <div class="collapse-item">
                <div class="collapse-header" onclick="toggleItem(this)">
                    <div style="display:flex; align-items:center; gap:10px;"><i class="fas fa-rocket main-icon"></i> <h3>مهارات المستقبل</h3></div>
                    <i class="fas fa-chevron-down chevron"></i>
                </div>
                <div class="collapse-content"><div class="content-padding">التعريف بمبادئ التقنية البسيطة والتفكير المنطقي لمواكبة تطلعات رؤية المملكة 2030.</div></div>
            </div>
        </div>

    </div>

    <a href="https://forms.google.com/ضع_رابط_نموذجك_هنا" target="_blank" class="qa-float" title="اسأل القائدة">
        <i class="fas fa-question"></i>
    </a>

    <footer>
        <h2 style="color:var(--gold); margin:0;">فاطمه صالح آل بحري</h2>
        <p>نصنع الأثر.. ونبني الأجيال | 2026</p>
    </footer>

    <script>
        function toggleItem(el) {
            const item = el.parentElement;
            const isActive = item.classList.contains('active');
            
            // إغلاق أي منسدلة أخرى مفتوحة
            document.querySelectorAll('.collapse-item').forEach(i => i.classList.remove('active'));
            
            // فتح المنسدلة الحالية إذا لم تكن مفتوحة
            if (!isActive) {
                item.classList.add('active');
            }
        }
    </script>
</body>
</html>
