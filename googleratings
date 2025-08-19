# Googleratings
واجهة تحتوي على ايقونات لتقييم جوجل لعدة فروع
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8 ">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>نفوذ الغربية </title>
    <link rel="stylesheet" href="   ">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #fdf0f1, #f8d7da, #fdf0f1);
            background-size: 400% 400%;
            animation: gradientBG 15s ease infinite;
            min-height: 100vh;
            padding: 20px;
            color: #781f19;
            direction: rtl;
        }
        
        @keyframes gradientBG {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        
        .container {
            max-width: 1400px;
            margin: 0 auto;
        }
        
        header {
            text-align: center;
            padding: 30px 0;
            margin-bottom: 30px;
        }
        
        h1 {
            font-size: 2.8rem;
            margin-bottom: 10px;
            text-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: relative;
            display: inline-block;
            color: #781f19;
        }
        
        h1::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 70%;
            height: 3px;
            background: linear-gradient(to right, transparent, #781f19, transparent);
        }
        
        .subtitle {
            font-size: 1.2rem;
            opacity: 0.9;
            max-width: 600px;
            margin: 0 auto;
            line-height: 1.6;
            color: #781f19;
        }
        
        .brands-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
            gap: 25px;
            margin-top: 40px;
        }
        
        .brand-card {
            background: rgba(255, 255, 255, 0.7);
            backdrop-filter: blur(10px);
            border-radius: 15px;
            padding: 20px;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 8px 25px rgba(120, 31, 25, 0.1);
            border: 1px solid rgba(120, 31, 25, 0.1);
            position: relative;
            overflow: hidden;
        }
        
        .brand-card:hover {
            transform: translateY(-10px);
            background: rgba(255, 255, 255, 0.9);
            box-shadow: 0 15px 35px rgba(120, 31, 25, 0.15);
        }
        
        .brand-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 5px;
            background: #781f19;
            transform: scaleX(0);
            transform-origin: left;
            transition: transform 0.3s ease;
        }
        
        .brand-card:hover::before {
            transform: scaleX(1);
        }
        
        .brand-icon {
            width: 80px;
            height: 80px;
            margin: 0 auto 15px;
            background: #781f19;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2.5rem;
            color: #fdf0f1;
            box-shadow: 0 5px 15px rgba(120, 31, 25, 0.2);
        }
        
        .brand-name {
            font-size: 1.2rem;
            font-weight: 700;
            margin-bottom: 5px;
            color: #781f19;
        }
        
        .brand-location {
            font-size: 1rem;
            font-weight: 600;
            color: #c0554d;
            margin-top: 8px;
            padding: 5px 10px;
            background: rgba(120, 31, 25, 0.05);
            border-radius: 20px;
            display: inline-block;
        }
        
        .brand-desc {
            font-size: 0.85rem;
            opacity: 0.8;
            color: #781f19;
            margin-top: 10px;
        }
        
        .branch-filter {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 10px;
            margin: 30px 0;
        }
        
        .filter-btn {
            padding: 8px 20px;
            background: rgba(120, 31, 25, 0.1);
            border: 1px solid rgba(120, 31, 25, 0.2);
            border-radius: 30px;
            color: #781f19;
            cursor: pointer;
            transition: all 0.3s;
            font-weight: 500;
        }
        
        .filter-btn:hover, .filter-btn.active {
            background: #781f19;
            color: #fdf0f1;
        }
        
        /* Modal Styles */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            z-index: 1000;
            align-items: center;
            justify-content: center;
            backdrop-filter: blur(5px);
        }
        
        .modal-content {
            background: linear-gradient(145deg, #fdf0f1, #f8d7da);
            width: 90%;
            max-width: 500px;
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 25px 50px rgba(120, 31, 25, 0.2);
            position: relative;
            animation: modalAppear 0.4s ease-out;
            border: 2px solid #781f19;
        }
        
        @keyframes modalAppear {
            from { opacity: 0; transform: translateY(50px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .modal-header {
            padding: 20px;
            background: rgba(120, 31, 25, 0.9);
            display: flex;
            align-items: center;
        }
        
        .modal-icon {
            width: 50px;
            height: 50px;
            background: #fdf0f1;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            color: #781f19;
            margin-left: 15px;
        }
        
        .modal-title {
            font-size: 1.5rem;
            font-weight: 700;
            color: #fdf0f1;
        }
        
        .close-btn {
            position: absolute;
            top: 20px;
            left: 20px;
            font-size: 1.5rem;
            cursor: pointer;
            background: rgba(253, 240, 241, 0.2);
            width: 40px;
            height: 40px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s;
            color: #fdf0f1;
        }
        
        .close-btn:hover {
            background: rgba(253, 240, 241, 0.3);
            transform: rotate(90deg);
        }
        
        .modal-body {
            padding: 30px;
        }
        
        .info-section {
            margin-bottom: 25px;
        }
        
        .info-title {
            display: flex;
            align-items: center;
            margin-bottom: 15px;
            font-size: 1.1rem;
            color: #781f19;
            font-weight: 600;
        }
        
        .info-title i {
            margin-left: 10px;
        }
        
        .website-link {
            display: block;
            background: rgba(120, 31, 25, 0.05);
            padding: 12px 20px;
            border-radius: 10px;
            color: #781f19;
            text-decoration: none;
            transition: all 0.3s;
            word-break: break-all;
            font-size: 0.95rem;
            border: 1px solid rgba(120, 31, 25, 0.1);
        }
        
        .website-link:hover {
            background: rgba(120, 31, 25, 0.1);
            transform: translateX(-5px);
        }
        
        .qrcode-container {
            text-align: center;
            padding: 15px;
            background: rgba(120, 31, 25, 0.05);
            border-radius: 15px;
            margin-top: 20px;
            border: 1px solid rgba(120, 31, 25, 0.1);
        }
        
        .qrcode-img {
            max-width: 200px;
            width: 100%;
            height: auto;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            border: 1px solid #e0c8c9;
        }
        
        .qrcode-label {
            display: block;
            margin-top: 10px;
            font-size: 0.9rem;
            opacity: 0.8;
            color: #781f19;
        }
        
        .instructions {
            background: rgba(120, 31, 25, 0.05);
            padding: 20px;
            border-radius: 15px;
            margin-top: 20px;
            font-size: 0.9rem;
            line-height: 1.6;
            color: #781f19;
            border: 1px solid rgba(120, 31, 25, 0.1);
        }
        
        .instructions h3 {
            margin-bottom: 10px;
            color: #781f19;
            display: flex;
            align-items: center;
        }
        
        .instructions h3 i {
            margin-left: 8px;
        }
        
        .instructions ul {
            padding-right: 20px;
        }
        
        .instructions li {
            margin-bottom: 8px;
        }
        
        /* Footer */
        footer {
            text-align: center;
            padding: 30px 0;
            margin-top: 40px;
            font-size: 0.9rem;
            opacity: 0.8;
            border-top: 1px solid rgba(120, 31, 25, 0.1);
            color: #781f19;
        }
        
        /* New Styles for Back Button */
        .back-button {
            position: fixed;
            top: 20px;
            right: 20px;
            padding: 10px 20px;
            background-color: #781f19;
            color: #fdf0f1;
            border: none;
            border-radius: 30px;
            font-size: 1rem;
            cursor: pointer;
            z-index: 999;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
            transition: all 0.3s ease;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .back-button:hover {
            background-color: #a43a34;
            transform: translateY(-2px);
        }

        .back-button i {
            transform: scaleX(-1);
        }

        /* Responsive */
        @media (max-width: 768px) {
            .brands-container {
                grid-template-columns: repeat(auto-fill, minmax(160px, 1fr));
                gap: 15px;
            }
            
            h1 {
                font-size: 2.2rem;
            }
            
            .brand-icon {
                width: 65px;
                height: 65px;
                font-size: 2rem;
            }
            
            .modal-content {
                width: 95%;
            }
        }
        
        @media (max-width: 480px) {
            .brands-container {
                grid-template-columns: repeat(auto-fill, minmax(140px, 1fr));
            }
            
            .brand-card {
                padding: 15px 10px;
            }
            
            .brand-icon {
                width: 55px;
                height: 55px;
                font-size: 1.7rem;
            }
            
            .brand-name {
                font-size: 1rem;
            }
        }
    </style>
</head>
<body>
    <button class="back-button" onclick="goBack()" style="display:none;"><i class="fas fa-arrow-right"></i> رجوع</button>

    <div class="container">
        <header id="main-header">
            <h1><i class="fas fa-store-alt"></i> نفوذ الغربية </h1>
            <p class="subtitle">متابعة تقييمات الفروع في جوجل </p>
        </header>
        
        <div id="brands-section">
            <div class="branch-filter">
                <button class="filter-btn active" data-location="all">جميع الفروع</button>
                <button class="filter-btn" data-location="النعيم">النعيم</button>
                <button class="filter-btn" data-location="الحمدانية">الحمدانية</button>
                <button class="filter-btn" data-location="السامر">السامر</button>
                <button class="filter-btn" data-location="النسيم">النسيم</button>
                <button class="filter-btn" data-location="الصفا">الصفا</button>
                <button class="filter-btn" data-location="السنابل">السنابل</button>
                <button class="filter-btn" data-location="أبحر">أبحر</button>
                <button class="filter-btn" data-location="الشوقية">الشوقية</button>
                <button class="filter-btn" data-location="الجال">الجال</button>
            </div>
            
            <div class="brands-container">
                <div class="brand-card" data-location="النعيم" onclick="openModal('مامولا', 'مامولا - النعيم', 'https://maps.app.goo.gl/JXPxpX4S93iXcYcJ8?g_st=ac', 'النعيم')">
                    <div class="brand-icon">
                        <i class="fas fa-crown"></i>
                    </div>
                    <div class="brand-name">مامولا</div>
                    <div class="brand-location">النعيم</div>
                    <div class="brand-desc">منتجات فاخرة </div>
                </div>
                
                <div class="brand-card" data-location="النعيم" onclick="openModal('عنبة', 'عنبة - النعيم', 'https://maps.app.goo.gl/Ad7uBieJqnEkk9nJ7?g_st=awb', 'النعيم')">
                    <div class="brand-icon">
                        <i class="fas fa-wine-bottle"></i>
                    </div>
                    <div class="brand-name">عنبة</div>
                    <div class="brand-location">النعيم</div>
                    <div class="brand-desc">عصائر طبيعية ومنعشة</div>
                </div>
                
                <div class="brand-card" data-location="النعيم" onclick="openModal('لقمة وردية', 'لقمة وردية - النعيم', 'https://maps.app.goo.gl/F4w2bUpcdbQkgBwf7?g_st=ac', 'النعيم')">
                    <div class="brand-icon">
                        <i class="fas fa-utensils"></i>
                    </div>
                    <div class="brand-name">لقمة وردية</div>
                    <div class="brand-location">النعيم</div>
                    <div class="brand-desc">أطباق مميزة ولذيذة</div>
                </div>
                
                <div class="brand-card" data-location="النعيم" onclick="openModal('قشطية', 'قشطية - النعيم', 'https://maps.app.goo.gl/NuwS3Kv5BNkDicfK8?g_st=ac', 'النعيم')">
                    <div class="brand-icon">
                        <i class="fas fa-ice-cream"></i>
                    </div>
                    <div class="brand-name">قشطية</div>
                    <div class="brand-location">النعيم</div>
                    <div class="brand-desc">حلويات شرقية بلمسة عصرية</div>
                </div>
                
                <div class="brand-card" data-location="الحمدانية" onclick="openModal('مامولا', 'مامولا - الحمدانية', 'https://maps.app.goo.gl/YpTg5qS2NJzSsiDG8?g_st=ac', 'الحمدانية')">
                    <div class="brand-icon">
                        <i class="fas fa-crown"></i>
                    </div>
                    <div class="brand-name">مامولا</div>
                    <div class="brand-location">الحمدانية</div>
                    <div class="brand-desc">منتجات فاخرة </div>
                </div>
                
                <div class="brand-card" data-location="الحمدانية" onclick="openModal('عنبة', 'عنبة - الحمدانية', 'https://maps.app.goo.gl/P5XbBgZRsJH1rc18A?g_st=ac', 'الحمدانية')">
                    <div class="brand-icon">
                        <i class="fas fa-wine-bottle"></i>
                    </div>
                    <div class="brand-name">عنبة</div>
                    <div class="brand-location">الحمدانية</div>
                    <div class="brand-desc">عصائر طبيعية ومنعشة</div>
                </div>
                
                <div class="brand-card" data-location="السامر" onclick="openModal('مامولا', 'مامولا - السامر', 'https://maps.app.goo.gl/upnceUw8K6SmsEUW9?g_st=ac', 'السامر')">
                    <div class="brand-icon">
                        <i class="fas fa-crown"></i>
                    </div>
                    <div class="brand-name">مامولا</div>
                    <div class="brand-location">السامر</div>
                    <div class="brand-desc">منتجات فاخرة </div>
                </div>
                
                <div class="brand-card" data-location="السامر" onclick="openModal('عنبة', 'عنبة - السامر', 'https://maps.app.goo.gl/WuuNvaPQzPi8ci7E7?g_st=ac', 'السامر')">
                    <div class="brand-icon">
                        <i class="fas fa-wine-bottle"></i>
                    </div>
                    <div class="brand-name">عنبة</div>
                    <div class="brand-location">السامر</div>
                    <div class="brand-desc">عصائر طبيعية ومنعشة</div>
                </div>
                
                <div class="brand-card" data-location="النسيم" onclick="openModal('مامولا', 'مامولا - النسيم', 'https://maps.app.goo.gl/qBA9yTd6mQGUVsfbA?g_st=ac', 'النسيم')">
                    <div class="brand-icon">
                        <i class="fas fa-crown"></i>
                    </div>
                    <div class="brand-name">مامولا</div>
                    <div class="brand-location">النسيم</div>
                    <div class="brand-desc">منتجات فاخرة </div>
                </div>
                
                <div class="brand-card" data-location="النسيم" onclick="openModal('عنبة', 'عنبة - النسيم', 'https://maps.app.goo.gl/oekjGoLYD1hTLB5F9?g_st=ac', 'النسيم')">
                    <div class="brand-icon">
                        <i class="fas fa-wine-bottle"></i>
                    </div>
                    <div class="brand-name">عنبة</div>
                    <div class="brand-location">النسيم</div>
                    <div class="brand-desc">عصائر طبيعية ومنعشة</div>
                </div>
                
                <div class="brand-card" data-location="الصفا" onclick="openModal('مامولا', 'مامولا - الصفا', 'https://maps.app.goo.gl/Ro1mAUogMH8vhY9Z8?g_st=ac', 'الصفا')">
                    <div class="brand-icon">
                        <i class="fas fa-crown"></i>
                    </div>
                    <div class="brand-name">مامولا</div>
                    <div class="brand-location">الصفا</div>
                    <div class="brand-desc">منتجات فاخرة </div>
                </div>
                
                <div class="brand-card" data-location="الصفا" onclick="openModal('عنبة', 'عنبة - الصفا', 'https://maps.app.goo.gl/viLGDu2m11XjR1pM7?g_st=ac', 'الصفا')">
                    <div class="brand-icon">
                        <i class="fas fa-wine-bottle"></i>
                    </div>
                    <div class="brand-name">عنبة</div>
                    <div class="brand-location">الصفا</div>
                    <div class="brand-desc">عصائر طبيعية ومنعشة</div>
                </div>
                
                <div class="brand-card" data-location="السنابل" onclick="openModal('مامولا', 'مامولا - السنابل', 'https://maps.app.goo.gl/7uVospEVDU6DJRiP6?g_st=ac', 'السنابل')">
                    <div class="brand-icon">
                        <i class="fas fa-crown"></i>
                    </div>
                    <div class="brand-name">مامولا</div>
                    <div class="brand-location">السنابل</div>
                    <div class="brand-desc">منتجات فاخرة </div>
                </div>
                
                <div class="brand-card" data-location="السنابل" onclick="openModal('عنبة', 'عنبة - السنابل', 'https://maps.app.goo.gl/TqX9QfyJuWMqpxfd6?g_st=ac', 'السنابل')">
                    <div class="brand-icon">
                        <i class="fas fa-wine-bottle"></i>
                    </div>
                    <div class="brand-name">عنبة</div>
                    <div class="brand-location">السنابل</div>
                    <div class="brand-desc">عصائر طبيعية ومنعشة</div>
                </div>
                
                <div class="brand-card" data-location="أبحر" onclick="openModal('مامولا', 'مامولا - أبحر', 'https://maps.app.goo.gl/2dhzA2KiSyeWYoF68?g_st=ac', 'أبحر')">
                    <div class="brand-icon">
                        <i class="fas fa-crown"></i>
                    </div>
                    <div class="brand-name">مامولا</div>
                    <div class="brand-location">أبحر</div>
                    <div class="brand-desc">منتجات فاخرة </div>
                </div>
                
                <div class="brand-card" data-location="أبحر" onclick="openModal('عنبة', 'عنبة - أبحر', 'https://maps.app.goo.gl/ZZMPsBLhQ3J5F3eb7?g_st=ac', 'أبحر')">
                    <div class="brand-icon">
                        <i class="fas fa-wine-bottle"></i>
                    </div>
                    <div class="brand-name">عنبة</div>
                    <div class="brand-location">أبحر</div>
                    <div class="brand-desc">عصائر طبيعية ومنعشة</div>
                </div>
                
                <div class="brand-card" data-location="الشوقية" onclick="openModal('مامولا', 'مامولا - الشوقية', 'https://maps.app.goo.gl/8HQSiFMSSe7iT9ZM9?g_st=ac', 'الشوقية')">
                    <div class="brand-icon">
                        <i class="fas fa-crown"></i>
                    </div>
                    <div class="brand-name">مامولا</div>
                    <div class="brand-location">الشوقية</div>
                    <div class="brand-desc">منتجات فاخرة </div>
                </div>
                
                <div class="brand-card" data-location="الشوقية" onclick="openModal('عنبة', 'عنبة - الشوقية', 'https://maps.app.goo.gl/Ex5eqcNhqXvzQqbj9?g_st=ac', 'الشوقية')">
                    <div class="brand-icon">
                        <i class="fas fa-wine-bottle"></i>
                    </div>
                    <div class="brand-name">عنبة</div>
                    <div class="brand-location">الشوقية</div>
                    <div class="brand-desc">عصائر طبيعية ومنعشة</div>
                </div>
                
                <div class="brand-card" data-location="الجال" onclick="openModal('مامولا', 'مامولا - الجال', 'https://maps.app.goo.gl/7g8mGFiu7CM8J9UG9?g_st=ac', 'الجال')">
                    <div class="brand-icon">
                        <i class="fas fa-crown"></i>
                    </div>
                    <div class="brand-name">مامولا</div>
                    <div class="brand-location">الجال</div>
                    <div class="brand-desc">منتجات فاخرة </div>
                </div>
                
                <div class="brand-card" data-location="الجال" onclick="openModal('عنبة', 'عنبة - الجال', 'https://maps.app.goo.gl/E4roDsAhBP2otUn89?g_st=ac', 'الجال')">
                    <div class="brand-icon">
                        <i class="fas fa-wine-bottle"></i>
                    </div>
                    <div class="brand-name">عنبة</div>
                    <div class="brand-location">الجال</div>
                    <div class="brand-desc">عصائر طبيعية ومنعشة</div>
                </div>
            </div>
        </div>
        
        <div id="brandModal" class="modal">
            <div class="modal-content">
                <div class="close-btn" onclick="closeModal()">
                    <i class="fas fa-times"></i>
                </div>
                <div class="modal-header">
                    <div class="modal-icon" id="modalIcon">
                        <i class="fas fa-store-alt"></i>
                    </div>
                    <h2 class="modal-title" id="modalTitle">مامولا - النعيم</h2>
                </div>
                <div class="modal-body">
                    <div class="info-section">
                        <div class="info-title">
                            <i class="fas fa-link"></i>
                            <span>الموقع الرسمي</span>
                        </div>
                        <a href="#" class="website-link" id="websiteLink" target="_blank">https://www.mamola.com/naim</a>
                    </div>
                    
                    <div class="info-section">
                        <div class="info-title">
                            <i class="fas fa-map-marker-alt"></i>
                            <span>الموقع</span>
                        </div>
                        <div class="website-link" id="locationName">النعيم</div>
                    </div>
                    
                    <div class="info-section">
                        <div class="info-title">
                            <i class="fas fa-qrcode"></i>
                            <span>مسح الباركود للوصول إلى تعليقات جوجل</span>
                        </div>
                        <div class="qrcode-container">
                            <img src="https://api.qrserver.com/v1/create-qr-code/?size=200x200&data=https://google.com" alt="باركود تعليقات جوجل" class="qrcode-img" id="qrcodeImage">
                            <span class="qrcode-label">مسح الباركود للوصول إلى التقييمات والتعليقات</span>
                        </div>
                    </div>
                    
                    <div class="instructions">
                        <h3><i class="fas fa-info-circle"></i> كيفية استخدام الباركود</h3>
                        <ul>
                            <li>افتح تطبيق الكاميرا على هاتفك</li>
                            <li>وجّه الكاميرا نحو صورة الباركود</li>
                            <li>انقر على الرابط الذي سيظهر على شاشتك</li>
                            <li>ستتم إعادة توجيهك مباشرة إلى صفحة تعليقات جوجل الخاصة بهذا الفرع</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        
        <footer>
            <p>نظام نفوذ الغربية </p>
            <p>انقر على أيقونة الفرع لرؤية التفاصيل والوصول إلى تعليقات جوجل</p>
        </footer>
    </div>
    
    <script>
        // Function to open modal with brand info
        function openModal(brandName, fullName, websiteUrl, location) {
            const modal = document.getElementById('brandModal');
            const modalTitle = document.getElementById('modalTitle');
            const websiteLink = document.getElementById('websiteLink');
            const modalIcon = document.getElementById('modalIcon');
            const qrcodeImage = document.getElementById('qrcodeImage');
            const locationElement = document.getElementById('locationName');
            
            // Hide main content and show back button
            document.getElementById('main-header').style.display = 'none';
            document.getElementById('brands-section').style.display = 'none';
            document.querySelector('.back-button').style.display = 'flex';
            
            // Set modal content
            modalTitle.textContent = fullName;
            websiteLink.textContent = websiteUrl;
            websiteLink.href = websiteUrl;
            locationElement.textContent = location;
            
            // Generate Google reviews URL for QR code
            const googleReviewsUrl = `https://search.google.com/local/writereview?placeid=${brandName}-${location}`;
            qrcodeImage.src = `https://api.qrserver.com/v1/create-qr-code/?size=200x200&data=${encodeURIComponent(googleReviewsUrl)}`;
            
            // Set icon based on brand
            modalIcon.innerHTML = '';
            const icon = document.createElement('i');
            
            switch(brandName) {
                case 'مامولا':
                    icon.className = 'fas fa-crown';
                    break;
                case 'عنبة':
                    icon.className = 'fas fa-wine-bottle';
                    break;
                case 'لقمة وردية':
                    icon.className = 'fas fa-utensils';
                    break;
                case 'قشطية':
                    icon.className = 'fas fa-ice-cream';
                    break;
                default:
                    icon.className = 'fas fa-store-alt';
            }
            
            modalIcon.appendChild(icon);
            
            // Display modal
            modal.style.display = 'flex';
        }
        
        // Function to close modal
        function closeModal() {
            document.getElementById('brandModal').style.display = 'none';
            
            // Show main content again and hide back button
            document.getElementById('main-header').style.display = 'block';
            document.getElementById('brands-section').style.display = 'block';
            document.querySelector('.back-button').style.display = 'none';
        }

        // Function to go back to main page
        function goBack() {
            closeModal();
        }
        
        // Close modal when clicking outside
        window.onclick = function(event) {
            const modal = document.getElementById('brandModal');
            if (event.target === modal) {
                closeModal();
            }
        }
        
        // Filter functionality
        document.querySelectorAll('.filter-btn').forEach(button => {
            button.addEventListener('click', () => {
                // Remove active class from all buttons
                document.querySelectorAll('.filter-btn').forEach(btn => {
                    btn.classList.remove('active');
                });
                
                // Add active class to clicked button
                button.classList.add('active');
                
                const location = button.getAttribute('data-location');
                const cards = document.querySelectorAll('.brand-card');
                
                cards.forEach(card => {
                    if (location === 'all' || card.getAttribute('data-location') === location) {
                        card.style.display = 'block';
                    } else {
                        card.style.display = 'none';
                    }
                });
            });
        });
    </script>
</body>
</html>
