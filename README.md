<! فكره أ/ فاطمه صالح نحو الاستدامه>
< rt
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>منصة الإنجاز والشفافية | فاطمه آل بحري</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        :root { --primary: #006d51; --gold: #d4af37; --bg: #f8fbf9; --white: #ffffff; }
        body { font-family: 'Segoe UI', Tahoma, sans-serif; margin: 0; background-color: var(--bg); color: #333; line-height: 1.6; }
        header { background: linear-gradient(135deg, var(--primary), #004d39); color: white; padding: 50px 20px; text-align: center; border-bottom: 6px solid var(--gold); }
        .container { max-width: 900px; margin: auto; padding: 20px; }
        
        /* الروضة الشفافة */
        .transparency-box { background: var(--white); padding: 25px; border-radius: 20px; box-shadow: 0 10px 25px rgba(0,0,0,0.05); margin-top: -50px; margin-bottom: 30px; border-right: 8px solid var(--gold); }
        
        /* القائمة المنسدلة */
        .skill-item { background: var(--white); margin-bottom: 12px; border-radius: 15px; border: 1px solid #eee; overflow: hidden; }
        .skill-header { padding: 18px; display: flex; align-items: center; justify-content: space-between; cursor: pointer; }
        .skill-content { max-height: 0; overflow: hidden; transition: 0.3s ease-out; background: #fafafa; }
        .skill-item.active .skill-content { max-height: 200px; }
        .skill-item.active .chevron { transform: rotate(180deg); }

        /* أيقونة الأسئلة */
        .qa-float { position: fixed; bottom: 30px; left: 30px; background: var(--gold); color: white; width: 60px; height: 60px; border-radius: 50%; display: flex; justify-content: center; align-items: center; font-size: 25px; cursor: pointer; z-index: 1000; box-shadow: 0 8px 20px rgba(0,0,0,0.2); }
        
        footer { background: var(--primary); color: white; padding: 40px 20px; text-align: center; margin-top: 50px; border-top: 5px solid var(--gold); }
    </style>
</head>
<body>

    <header>
        <h1>منصة الإنجاز والشفافية</h1>
        <p style="color: var(--gold); font-weight: bold;">بوابة القائدة الملهمة: فاطمه صالح آل بحري</p>
    </header>

    <div class="container">
        
        <div class="transparency-box">
            <h3><i class="fas fa-bullhorn"></i> الروضة الشفافة</h3>
            <p>قيمنا هذا الأسبوع: <strong>"الاستدامة والرفق بالبيئة"</strong></p>
        </div>

        <h2 style="text-align: center; color: var(--primary);">جواز السفر الذكي للمهارات</h2>
        
        <div class="skill-item">
            <div class="skill-header" onclick="toggle(this)">
                <span><i class="fas fa-child"></i> الاستقلال الذاتي</span>
                <i class="fas fa-chevron-down chevron"></i>
            </div>
            <div class="skill-content"><p>تعليم الطفل مهارات الحياة اليومية ليكون قائداً مستقلاً في منزله ومجتمعه.</p></div>
        </div>

        <div style="background: #eef7f2; padding: 25px; border-radius: 20px; border: 2px dashed var(--primary); margin-top: 40px; text-align: center;">
            <h3 style="color: var(--primary);"><i class="fas fa-leaf"></i> مبادرة غرس الاستدامة</h3>
            <p><strong>تحدي الأسبوع:</strong> ساعد طفلك على زراعة بذرة صغيرة في وعاء بالمنزل وراقبا نموها معاً.</p>
        </div>

    </div>

    <div class="qa-float" onclick="alert('يسعدنا تواصلكم قريباً!')">
        <i class="fas fa-question"></i>
    </div>

    <footer>
        <h2 style="color: var(--gold);">فاطمه صالح آل بحري</h2>
        <p>نحو تعليم مستدام يواكب رؤية المملكة 2030</p>
    </footer>

    <script>
        function toggle(el) {
            el.parentElement.classList.toggle('active');
        }
    </script>
</body>
</html>
