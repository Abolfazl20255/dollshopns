<!DOCTYPE html>
<html lang="fa">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DollShopNS - عروسک‌های بافتنی</title>
    <style>
        body {
            background: url('https://i.postimg.cc/KY9hB65x/1000029365-LE-upscale-balanced-x4.jpg') no-repeat center center fixed;
            background-size: cover;
            font-family: Arial, sans-serif;
            text-align: center;
            color: white;
            margin: 0;
            padding: 0;
            height: 100vh;
        }
        .container {
            max-width: 100%;
            margin: 30px auto;
            background: rgba(0, 0, 0, 0.6);
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.3);
            width: 90%;
            overflow: hidden;
        }
        h1 {
            font-size: 28px;
        }
        .desc {
            font-size: 18px;
            margin-bottom: 20px;
        }
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 10px;
        }
        .gallery img {
            width: 100%;
            border-radius: 10px;
            transition: transform 0.3s, box-shadow 0.3s;
            cursor: pointer;
        }
        .gallery img:hover {
            transform: scale(1.05);
            box-shadow: 0 0 15px rgba(255, 255, 255, 0.7);
        }
        .buttons {
            margin-top: 20px;
        }
        .btn {
            display: inline-block;
            padding: 10px 20px;
            margin: 10px;
            font-size: 18px;
            color: white;
            background: #ff007f;
            text-decoration: none;
            border-radius: 5px;
            transition: background 0.3s;
        }
        .btn:hover {
            background: #ff3399;
        }
        /* پاپ‌آپ */
        .popup {
            display: none;
            position: fixed;
            z-index: 999;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
        }
        .popup img {
            margin: auto;
            display: block;
            max-width: 90%;
            max-height: 90%;
            border-radius: 10px;
        }
        .popup .close {
            position: absolute;
            top: 10px;
            right: 10px;
            color: white;
            font-size: 30px;
            cursor: pointer;
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>به dollshopns دنیای عروسک های بافتنی خوش آمدید</h1>
        <p class="desc">ما بهترین و جذاب ترین عروسک های بافتنی را برای شما آماده کرده ایم. با عشق خرید کنید</p>

        <div class="gallery">
            <img src="https://i.postimg.cc/jjsssL0b/472547649-1788734578632034-8514592903985262509-n-webp.jpg" alt="عروسک بافتنی 1" onclick="openPopup(this.src)">
            <img src="https://i.postimg.cc/Z5Pbt6QH/469974566-3783615805231373-2231633653268564379-n-webp.jpg" alt="عروسک بافتنی 2" onclick="openPopup(this.src)">
            <img src="https://i.postimg.cc/zXgD7sS9/472534078-1140629154133772-5353844971935112429-n-webp.jpg" alt="عروسک بافتنی 3" onclick="openPopup(this.src)">
            <img src="https://i.imgur.com/LFj322G.jpeg" alt="عروسک بافتنی 4" onclick="openPopup(this.src)">
        </div>

        <div class="buttons">
            <a class="btn" href="https://www.instagram.com/dollshopns" target="_blank">مشاهده در اینستاگرام</a>
        </div>
    </div>

    <!-- پاپ‌آپ نمایش تصویر -->
    <div id="popup" class="popup">
        <span class="close" onclick="closePopup()">×</span>
        <img id="popup-img" src="" alt="Popup Image">
    </div>

    <script>
        function openPopup(src) {
            document.getElementById('popup-img').src = src;
            document.getElementById('popup').style.display = 'block';
        }

        function closePopup() {
            document.getElementById('popup').style.display = 'none';
        }
    </script>
</body>
</html>
