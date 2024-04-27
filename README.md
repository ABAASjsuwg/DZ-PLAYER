<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Loading...</title>
<style>
  body {
    margin: 0;
    padding: 0;
    background-color: white;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    overflow: hidden;
  }
  .loader {
    border: 16px solid #f3f3f3; /* رمادي فاتح */
    border-top: 16px solid red; /* اللون الأحمر للدائرة */
    border-radius: 50%; /* جعل الحواف دائرية */
    width: 120px;
    height: 120px;
    animation: spin 2s linear infinite; /* تحريك الدائرة بشكل دائم */
  }
  .countdown {
    font-size: 24px;
    color: red;
    margin-top: 20px;
  }
  #content {
    display: none;
    max-width: 90%;
    text-align: center;
  }
  img {
    max-width: 100%;
    height: auto;
    margin-bottom: 10px;
  }
</style>
</head>
<body>
<div id="loader" class="loader"></div>
<div id="countdown" class="countdown" style="display: none;"></div>
<script>
  // عرض الشاشة البيضاء لمدة 2 ثانية
  setTimeout(function(){
    document.getElementById("loader").style.display = "none";
    document.getElementById("countdown").style.display = "block";
    document.body.style.overflow = "hidden"; // إخفاء التمرير
  }, 2000); // 2 ثانية
  
  // بدء العد التنازلي من 15 ثانية بعد عرض الشاشة البيضاء
  setTimeout(function(){
    var count = 15;
    var countdown = setInterval(function() {
      document.getElementById("countdown").innerHTML = count;
      count--;
      if (count === 0) {
        clearInterval(countdown);
        document.getElementById("countdown").style.display = "none";
        document.body.style.overflow = "auto"; // استعادة التمرير
        document.getElementById("content").style.display = "block"; // عرض الكود المطلوب
      }
    }, 1000); // كل ثانية واحدة
  }, 2000); // 2 ثانية
</script>
<div id="content">
  <img src="https://images-ext-1.discordapp.net/external/ke7FVWgC9oFz-ke0Pbir4nSKw0TCLaxAlUrChsNHlfs/https/play-lh.googleusercontent.com/f21s1gCAEwW9-NB40TGSjmDVnUnR-d4J8VG8h0QC88wPHVjrjb3Cl_EWlOJwig2vB-M" alt="Brain It On!">
  <h2>Brain It On!</h2>
  <a href="https://play.google.com/store/apps/details?id=com.orbital.brainiton&hl=ar&gl=US" class="download-btn">تحميل</a>
  <!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>اللعبة الجديدة</title>
<style>
  body {
    margin: 0;
    padding: 0;
    background-image: url('');
    background-size: cover;
    background-position: center;
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
  }
  .download-btn {
    background-color: red;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    font-size: 18px;
    cursor: pointer;
    margin-top: 20px;
  }
  img {
    width: 50%; /* تحديد عرض الصورة بنسبة 50% من عرض النافذة /
    height: auto; / السماح للارتفاع بالتعديل بشكل تلقائي حسب نسبة العرض /
    margin-bottom: 10px; / تباعد بسيط بين الصورة والزر /
  }
  h2 {
    background-color: lightgrey; / إضافة خلفية رمادية للعنوان /
    padding: 10px; / إضافة هامش داخلي لتحسين المظهر /
    border-radius: 5px; / تدوير الزوايا للمظهر الجميل */
  }
</style>
</head>
<body>
  <div>
    <h2> Free Fire </h2>
    <img src="https://media.discordapp.net/attachments/1233525263191769220/1233816071325094000/Z.png?ex=662e7842&is=662d26c2&hm=7370fafc5e0131db73de6f515bf9abe453e5bd8b41c59694390cdea9175bd317&=&format=webp&quality=lossless" alt="صورة اللعبة الجديدة">
    <a href="https://play.google.com/store/apps/details?id=com.dts.freefireth&hl=ar&gl=US" class="download-btn">تحميل</a>
  </div>
</body>
</html>
