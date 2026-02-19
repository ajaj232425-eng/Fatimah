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

        .collapse-item { background: white; margin-bottom: 12px; border-radius: 15px; border: 1px solid #eee; overflow: hidden; transition: 0.3s; }
        .collapse-header { padding: 18px; display: flex; align-items: center; justify-content: space-between; cursor: pointer; }
        .collapse-header i.main-icon { color: var(--gold); font-size: 1.3em; width: 35px; text-align: center; }
        .collapse-header h3 { margin: 0; font-size: 1.05em; color: var(--primary); }
        .collapse-content { max-height: 0; overflow: hidden; transition: 0.4s ease-out; background: #fafafa; }
        .collapse-item.active .collapse-content { max-height: 300px; border-top: 1px solid #eee; }
        .collapse-item.active .chevron { transform: rotate(180deg); }
        .chevron { transition: 0.3s; color: var(--gold); }

        /* أيقونة الأسئلة المرتبطة بقوقل فورمس */
        .qa-float { 
            position: fixed; bottom: 30px; left: 30px; background: var(--gold); color: white; 
            width: 65px; height: 65px; border-radius: 50%; display: flex; 
            justify-content: center; align-items: center; font-size: 25px; 
            cursor: pointer; z-index: 1000; box-shadow: 0 10px 25px rgba(212,175,55,0.5);
            text-decoration: none; transition: transform 0.3s ease;
        }
        .qa-float:hover { transform: scale(1.1); background: var(--primary); }

        footer { background: var(--primary); color: white; padding: 40px 20px; text-align: center; margin-top: 50px; border-top: 5px solid var(--gold); }
    </style>
</head>
<body>

    <header>
        <img src="https://upload.wikimedia.org/wikipedia/commons/1/11/Ministry_of_Education_Saudi_Arabia_Logo.svg" width="100" style="filter: brightness(0) invert(1); margin-bottom: 10px;">
        <h1>منصة الإنجاز والشفافية</h1>
        <p style="color: var(--gold); font-weight: bold;">فاطمه صالح آل بحري</p>
    </header>

    <div class="container">
        
        <div class="card-panel">
            <h2 style="color: var(--primary); margin-top: 0;"><i class="fas fa-eye"></i> الروضة الشفافة</h2>
            <div class="collapse-item">
                <div class="collapse-header" onclick="toggleItem(this)">
                    <div style="display:flex; align-items:center; gap:10px;"><i class="fas fa-star main-icon"></i> <h3>قيمة الأسبوع</h3></div>
                    <i class="fas fa-chevron-down chevron"></i>
                </div>
                <div class="collapse-content"><div style="padding:20px;">نغرس قيمنا الإسلامية والوطنية في نفوس صغارنا.</div></div>
            </div>
            <div class="collapse-item" style="border-right: 5px solid var(--primary);">
                <div class="collapse-header" onclick="toggleItem(this)">
                    <div style="display:flex; align-items:center; gap:10px;"><i class="fas fa-lightbulb main-icon"></i> <h3>المبادرة الأسبوعية</h3></div>
                    <i class="fas fa-chevron-down chevron"></i>
                </div>
                <div class="collapse-content"><div style="padding:20px;">مبادرة اجتماعية لتعزيز التواصل الإيجابي.</div></div>
            </div>
        </div>

        <div class="card-panel">
            <h2 style="color: var(--primary); margin-top: 0;"><i class="fas fa-passport"></i> جواز السفر الإلكتروني</h2>
            <div class="collapse-item"><div class="collapse-header" onclick="toggleItem(this)"><div style="display:flex; align-items:center; gap:10px;"><i class="fas fa-child main-icon"></i> <h3>الاستقلال الذاتي</h3></div><i class="fas fa-chevron-down chevron"></i></div><div class="collapse-content"><div style="padding:20px;">بناء طفل واثق ومستقل.</div></div></div>
            <div class="collapse-item"><div class="collapse-header" onclick="toggleItem(this)"><div style="display:flex; align-items:center; gap:10px;"><i class="fas fa-heart main-icon"></i> <h3>الذكاء الوجداني</h3></div><i class="fas fa-chevron-down chevron"></i></div><div class="collapse-content"><div style="padding:20px;">فهم المشاعر وبناء التعاطف.</div></div></div>
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
            document.querySelectorAll('.collapse-item').forEach(i => i.classList.remove('active'));
            if (!isActive) item.classList.add('active');
        }
    </script>
</body>
</html>
