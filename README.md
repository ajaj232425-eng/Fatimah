<! فكره أ/ فاطمه صالح نحو الاستدامه>
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>منصة الإنجاز والشفافية | فاطمه صالح آل بحري</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        :root { --primary: #006d51; --gold: #d4af37; --bg-overlay: rgba(248, 251, 249, 0.92); }
        
        body { 
            font-family: 'Segoe UI', Tahoma, sans-serif; margin: 0; 
            /* خلفية تعليمية راقية بنمط ناعم */
            background-image: url('https://www.transparenttextures.com/patterns/arabesque.png'), linear-gradient(135deg, #f0f4f2 0%, #e6eee9 100%);
            background-attachment: fixed;
            color: #333; line-height: 1.6; 
        }
        
        header { 
            background: linear-gradient(135deg, var(--primary), #004d39); 
            color: white; padding: 50px 20px; text-align: center; 
            border-bottom: 6px solid var(--gold);
            box-shadow: 0 4px 15px rgba(0,0,0,0.15);
            border-bottom-left-radius: 50px; border-bottom-right-radius: 50px;
        }

        .container { max-width: 800px; margin: auto; padding: 20px; position: relative; z-index: 1; }
        
        /* البطاقات المنبثقة من الخلفية */
        .card-panel {
            background: var(--bg-overlay);
            backdrop-filter: blur(10px);
            padding: 25px; border-radius: 25px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.08);
            margin-bottom: 25px;
            border: 1px solid rgba(255,255,255,0.6);
        }

        /* المنسدلات */
        .collapse-item { background: white; margin-bottom: 12px; border-radius: 15px; border: 1px solid #eee; overflow: hidden; transition: 0.3s; }
        .collapse-header { padding: 18px; display: flex; align-items: center; justify-content: space-between; cursor: pointer; }
        .collapse-header i.main-icon { color: var(--gold); font-size: 1.3em; width: 30px; text-align: center; }
        .collapse-header h3 { margin: 0; font-size: 1.05em; color: var(--primary); }
        .collapse-content { max-height: 0; overflow: hidden; transition: 0.4s ease-out; background: #fafafa; }
        .collapse-item.active { border-color: var(--gold); transform: translateY(-3px); box-shadow: 0 5px 15px rgba(0,0,0,0.05); }
        .collapse-item.active .collapse-content { max-height: 300px; border-top: 1px solid #eee; }
        .collapse-item.active .chevron { transform: rotate(180deg); }
        .chevron { transition: 0.3s; color: var(--gold); }

        /* نظام الأسئلة */
        #qa-window {
            position: fixed; bottom: 100px; left: 20px; right: 20px; 
            max-width: 400px; background: white; border-radius: 25px; 
            box-shadow: 0 20px 50px rgba(0,0,0,0.3); z-index: 2001;
            display: none; overflow: hidden; animation: popIn 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }
        @keyframes popIn { from { transform: translateY(50px) scale(0.9); opacity: 0; } to { transform: translateY(0) scale(1); opacity: 1; } }
        
        .qa-header { background: var(--primary); color: white; padding: 20px; text-align: center; }
        .qa-float { 
            position: fixed; bottom: 30px; left: 30px; background: var(--gold); color: white; 
            width: 65px; height: 65px; border-radius: 50%; display: flex; 
            justify-content: center; align-items: center; font-size: 30px; 
            cursor: pointer; z-index: 1000; box-shadow: 0 10px 25px rgba(212,175,55,0.5);
        }

        footer { background: var(--primary); color: white; padding: 50px 20px; text-align: center; margin-top: 60px; border-top: 5px solid var(--gold); }
    </style>
</head>
<body>

    <header>
        <img src="https://upload.wikimedia.org/wikipedia/commons/1/11/Ministry_of_Education_Saudi_Arabia_Logo.svg" width="100" style="filter: brightness(0) invert(1); margin-bottom: 10px;">
        <h1>منصة الإنجاز والشفافية</h1>
        <p style="color: var(--gold); font-weight: bold; font-size: 1.2em;">فاطمه صالح آل بحري</p>
    </header>

    <div class="container">
        
        <div class="card-panel">
            <h2 style="color: var(--primary); margin-top: 0;"><i class="fas fa-eye"></i> الروضة الشفافة</h2>
            
            <div class="collapse-item">
                <div class="collapse-header" onclick="toggleItem(this)">
                    <div style="display:flex; align-items:center; gap:10px;"><i class="fas fa-star main-icon"></i> <h3>قيمة الأسبوع</h3></div>
                    <i class="fas fa-chevron-down chevron"></i>
                </div>
                <div class="collapse-content"><div style="padding:20px;">نغرس اليوم بذرة "الاحترام" لنجني غداً مجتمعاً متماسكاً.</div></div>
            </div>

            <div class="collapse-item">
                <div class="collapse-header" onclick="toggleItem(this)">
                    <div style="display:flex; align-items:center; gap:10px;"><i class="fas fa-lightbulb main-icon"></i> <h3>المبادرة الأسبوعية</h3></div>
                    <i class="fas fa-chevron-down chevron"></i>
                </div>
                <div class="collapse-content"><div style="padding:20px; background:#f0f7f3;"><b>مبادرة بصمتي الاجتماعية:</b> تشجيع الطفل على مساعدة أقرانه في الروضة.</div></div>
            </div>
        </div>

        <div class="card-panel">
            <h2 style="color: var(--primary); margin-top: 0;"><i class="fas fa-passport"></i> جواز السفر الإلكتروني</h2>
            
            <div class="collapse-item">
                <div class="collapse-header" onclick="toggleItem(this)">
                    <div style="display:flex; align-items:center; gap:10px;"><i class="fas fa-child main-icon"></i> <h3>الاستقلال الذاتي</h3></div>
                    <i class="fas fa-chevron-down chevron"></i>
                </div>
                <div class="collapse-content"><div style="padding:20px;">بناء طفل يثق بقدراته ويتحمل مسؤولية قراراته الصغيرة.</div></div>
            </div>

            <div class="collapse-item">
                <div class="collapse-header" onclick="toggleItem(this)">
                    <div style="display:flex; align-items:center; gap:10px;"><i class="fas fa-heart main-icon"></i> <h3>الذكاء الوجداني</h3></div>
                    <i class="fas fa-chevron-down chevron"></i>
                </div>
                <div class="collapse-content"><div style="padding:20px;">تطوير مهارات التعاطف وفهم الذات لبناء توازن نفسي مستدام.</div></div>
            </div>
        </div>

    </div>

    <div id="qa-window">
        <div class="qa-header"><h4><i class="fas fa-comment-dots"></i> اسأل القائدة</h4></div>
        <div style="padding: 20px;" id="qa-form">
            <textarea id="userQ" rows="4" style="width:100%; border:1px solid #ddd; border-radius:10px; padding:10px;" placeholder="اكتب سؤالكِ هنا..."></textarea>
            <button onclick="sendQ()" style="background:var(--primary); color:white; border:none; width:100%; padding:12px; border-radius:10px; margin-top:10px; cursor:pointer; font-weight:bold;">إرسال الآن</button>
        </div>
    </div>

    <div class="qa-float" onclick="toggleQA()"><i class="fas fa-question"></i></div>

    <footer>
        <h2 style="color:var(--gold); margin:0;">فاطمه صالح آل بحري</h2>
        <p>نصنع الأثر.. ونبني الأجيال</p>
    </footer>

    <script>
        function toggleItem(el) {
            const item = el.parentElement;
            document.querySelectorAll('.collapse-item').forEach(i => { if (i !== item) i.classList.remove('active'); });
            item.classList.toggle('active');
        }

        function toggleQA() {
            const win = document.getElementById('qa-window');
            win.style.display = (win.style.display === 'block') ? 'none' : 'block';
        }

        function sendQ() {
            const q = document.getElementById('userQ').value;
            if(!q.trim()) return alert("يرجى كتابة السؤال أولاً");
            document.getElementById('qa-form').innerHTML = `<div style="text-align:center; padding:20px;"><i class="fas fa-check-circle" style="color:var(--primary); font-size:3em;"></i><p>شكرًا لكِ أستاذة فاطمه، تم استلام سؤالكِ بنجاح.</p></div>`;
            setTimeout(() => { toggleQA(); location.reload(); }, 3000);
        }
    </script>
</body>
</html>
