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
            color: white; padding: 50px 20px; text-align: center; 
            border-bottom: 6px solid var(--gold);
            border-bottom-left-radius: 50px; border-bottom-right-radius: 50px;
        }

        .container { max-width: 800px; margin: auto; padding: 20px; position: relative; }
        
        .card-panel {
            background: var(--bg-overlay);
            backdrop-filter: blur(10px);
            padding: 25px; border-radius: 25px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.08);
            margin-bottom: 25px;
            border: 1px solid rgba(255,255,255,0.6);
        }

        /* المنسدلات للمهارات والروضة */
        .collapse-item { background: white; margin-bottom: 12px; border-radius: 15px; border: 1px solid #eee; overflow: hidden; transition: 0.3s; }
        .collapse-header { padding: 18px; display: flex; align-items: center; justify-content: space-between; cursor: pointer; }
        .collapse-header i.main-icon { color: var(--gold); font-size: 1.3em; width: 30px; text-align: center; }
        .collapse-header h3 { margin: 0; font-size: 1.05em; color: var(--primary); }
        .collapse-content { max-height: 0; overflow: hidden; transition: 0.4s ease-out; background: #fafafa; }
        .collapse-item.active .collapse-content { max-height: 300px; border-top: 1px solid #eee; }
        .collapse-item.active .chevron { transform: rotate(180deg); }
        .chevron { transition: 0.3s; color: var(--gold); }

        /* --- خاصية المنسدلة لايقونة الأسئلة --- */
        .qa-container {
            position: fixed; bottom: 30px; left: 30px; z-index: 1000;
            display: flex; flex-direction: column-reverse; align-items: flex-start;
        }

        .qa-dropdown {
            max-height: 0; width: 300px; background: white; border-radius: 20px;
            box-shadow: 0 15px 35px rgba(0,0,0,0.2);
            margin-bottom: 15px; overflow: hidden;
            transition: max-height 0.5s cubic-bezier(0.4, 0, 0.2, 1);
            border: 1px solid #eee;
        }

        .qa-container.active .qa-dropdown { max-height: 400px; }

        .qa-float { 
            background: var(--gold); color: white; 
            width: 65px; height: 65px; border-radius: 50%; display: flex; 
            justify-content: center; align-items: center; font-size: 30px; 
            cursor: pointer; box-shadow: 0 10px 25px rgba(212,175,55,0.5);
            transition: transform 0.3s ease;
        }
        .qa-container.active .qa-float { transform: rotate(45deg); background: #ff4d4d; }

        .qa-header-text { background: var(--primary); color: white; padding: 15px; text-align: center; font-weight: bold; }
        .qa-body-form { padding: 20px; }
        .qa-body-form textarea { width: 100%; border: 1px solid #ddd; border-radius: 12px; padding: 10px; resize: none; font-family: inherit; box-sizing: border-box; }
        .qa-body-form button { background: var(--primary); color: white; border: none; width: 100%; padding: 12px; border-radius: 12px; margin-top: 10px; cursor: pointer; font-weight: bold; }

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
                <div class="collapse-content"><div style="padding:20px; background:#f0f7f3;"><b>مبادرة بصمتي الاجتماعية:</b> تعزيز التواصل بين الطفل وأقرانه بالتقدير والشكر.</div></div>
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

    <div class="qa-container" id="qaContainer">
        <div class="qa-dropdown">
            <div class="qa-header-text">تواصل مباشر مع القائدة</div>
            <div class="qa-body-form" id="qaFormBody">
                <p style="font-size: 0.85em; color: #666; margin-bottom: 10px;">يسعدنا الرد على استفساراتكم التربوية أستاذة فاطمه.</p>
                <textarea id="userQuestion" rows="4" placeholder="اكتب سؤالكِ هنا..."></textarea>
                <button onclick="sendQuestion()">إرسال الاستفسار</button>
            </div>
        </div>
        <div class="qa-float" onclick="toggleQADropdown()">
            <i class="fas fa-question" id="qaIcon"></i>
        </div>
    </div>

    <footer>
        <h2 style="color:var(--gold); margin:0;">فاطمه صالح آل بحري</h2>
        <p>نصنع الأثر.. ونبني الأجيال</p>
    </footer>

    <script>
        // دالة المنسدلات العامة
        function toggleItem(el) {
            const item = el.parentElement;
            document.querySelectorAll('.collapse-item').forEach(i => { if (i !== item) i.classList.remove('active'); });
            item.classList.toggle('active');
        }

        // دالة المنسدلة لأيقونة الأسئلة
        function toggleQADropdown() {
            const container = document.getElementById('qaContainer');
            const icon = document.getElementById('qaIcon');
            container.classList.toggle('active');
            
            if(container.classList.contains('active')) {
                icon.className = 'fas fa-times'; // تغيير الأيقونة لإغلاق
            } else {
                icon.className = 'fas fa-question'; // إعادة الأيقونة لسؤال
            }
        }

        // دالة إرسال السؤال التفاعلية
        function sendQuestion() {
            const q = document.getElementById('userQuestion').value;
            if(!q.trim()) return alert("يرجى كتابة السؤال أولاً");
            
            const formBody = document.getElementById('qaFormBody');
            formBody.innerHTML = `
                <div style="text-align:center; padding:10px;">
                    <i class="fas fa-check-circle" style="color:var(--primary); font-size:2.5em; margin-bottom:10px;"></i>
                    <p style="font-weight:bold; color:var(--primary);">تم الإرسال بنجاح!</p>
                    <p style="font-size:0.8em;">شكرًا لكِ أستاذة فاطمه، تم استلام سؤالكِ.</p>
                    <button onclick="toggleQADropdown()" style="background:var(--gold); margin-top:10px;">إغلاق</button>
                </div>
            `;
            
            // إعادة ضبط النموذج بعد 5 ثوانٍ
            setTimeout(() => { location.reload(); }, 5000);
        }
    </script>
</body>
</html>
