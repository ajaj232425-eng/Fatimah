# Fatimah<!DOCTYPE html><!DOCTYPE html>
<html lang="ar">
<head>
<meta charset="UTF-8">
<title>حساب عمر الطفل للروضة</title>

<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@600&display=swap" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/hijri-date/lib/safe.js"></script>

<style>
body{
    margin:0;
    font-family:'Cairo',sans-serif;
    direction:rtl;
    text-align:center;
    color:#333;

    /* صورة خلفية طفل كرتوني */
    background:url("https://cdn.pixabay.com/photo/2017/01/31/13/14/back-to-school-2022464_1280.png") no-repeat center center fixed;
    background-size:cover;
}

/* طبقة شفافة لراحة العين */
.overlay{
    position:fixed;
    top:0;
    left:0;
    width:100%;
    height:100%;
    background:rgba(255,255,255,0.65);
}

.container{
    position:relative;
    background:white;
    width:50%;
    margin:60px auto;
    padding:40px;
    border-radius:25px;
    box-shadow:0 10px 25px rgba(0,0,0,0.15);
    z-index:1;
}

h1{
    font-size:36px;
}

input,button{
    padding:14px;
    margin:10px;
    font-size:20px;
    border-radius:10px;
    border:1px solid #ccc;
}

button{
    background:#ff7aa2;
    color:white;
    border:none;
    cursor:pointer;
}

button:hover{
    background:#ff4d85;
}

.result{
    margin-top:20px;
    font-size:24px;
    line-height:1.8;
}

.footer{
    margin-top:30px;
    font-size:16px;
    color:#666;
}
</style>
</head>

<body>

<div class="overlay"></div>

<div class="container">
<h1>حساب عمر الطفل للروضة</h1>

<input type="date" id="birthdate">
<br>
<button onclick="calculateAge()">احسب العمر</button>

<div class="result" id="result"></div>

<div class="footer">
مديرة الروضة ومصممة الموقع :<br>
<strong>فاطمه صالح ال بحري</strong>
</div>
</div>

<script>
function calculateAge(){
    let birthdate=document.getElementById("birthdate").value;
    if(!birthdate){
        alert("ادخلي تاريخ الميلاد");
        return;
    }

    let birth=new Date(birthdate);
    let today=new Date();

    let years=today.getFullYear()-birth.getFullYear();
    let months=today.getMonth()-birth.getMonth();
    let days=today.getDate()-birth.getDate();

    if(days<0){
        months--;
        days+=30;
    }
    if(months<0){
        years--;
        months+=12;
    }

    let hijri=new HijriDate(today);

    let eligibility="";
    if(years>=3 && years<=6){
        eligibility="✅ العمر مناسب للروضة";
    }else if(years<3){
        eligibility="❌ أصغر من سن القبول";
    }else{
        eligibility="❌ أكبر من سن القبول";
    }

    document.getElementById("result").innerHTML=
    `
    العمر: ${years} سنة و ${months} شهر و ${days} يوم <br><br>
    📅 التاريخ الميلادي: ${today.toLocaleDateString()} <br>
    🌙 التاريخ الهجري: ${hijri.getDate()} / ${hijri.getMonth()+1} / ${hijri.getFullYear()} هـ <br><br>
    <strong>${eligibility}</strong>
    `;
}
</script>

</body>
</html>
