# 💕 موقع حب لـ نور

## وصف المشروع

هذا مشروع ويب رومانسي متكامل مصمم خصيصاً لإعلان حبك لـ "نور". يتضمن الموقع تصميماً أنيقاً ورومانسياً مع تأثيرات حركية جميلة ورسائل شخصية يمكن تخصيصها.

---

## هيكل الملفات

```
nour-love-site/
├── index.html
├── style.css
└── script.js
```

---

## 1. ملف HTML الرئيسي (index.html)

```html
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>لـ نور 💕</title>
    <link rel="stylesheet" href="style.css">
    <link href="https://fonts.googleapis.com/css2?family=Amiri:wght@400;700&family=Tajawal:wght@300;400;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
</head>
<body>
    <!-- خلفية القلوب المتحركة -->
    <div class="hearts-container" id="heartsContainer"></div>

    <!-- القسم الرئيسي -->
    <header class="hero-section">
        <div class="hero-content">
            <div class="photo-frame">
                <img src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?w=400&h=400&fit=crop" alt="نور" class="main-photo">
                <div class="frame-decoration"></div>
            </div>
            <h1 class="title">لحبي الوحيد</h1>
            <h2 class="subtitle">نور 💕</h2>
            <p class="intro-text">هذا الموقع هو طريقة صغيرة لأقول لكِ...</p>
            <button class="start-btn" onclick="startJourney()">
                <i class="fas fa-heart"></i>
                اضغطي هنا يا حياتي
            </button>
        </div>
    </header>

    <!-- قسم رسالة الحب -->
    <section class="love-message" id="loveMessage">
        <div class="container">
            <div class="message-card">
                <div class="message-header">
                    <i class="fas fa-heart heart-icon"></i>
                    <h2>رسالة من القلب</h2>
                </div>
                <div class="message-body">
                    <p class="arabic-text">
                        نُوْرِيْ عُمْرِيْ،<br><br>
                        لَمْ أَجِدْ كَلِمَاتٍ تَسْتَطِيعُ أَنْ تَصِفَ مَشَاعِرِيْ نَحْوَكِ. 
                        أَنْتِ السَّبَبُ فِيْ ابْتِسَامَتِيْ كُلَّ يَوْمٍ، وَالنُّورُ الَّذِيْ يُضِيءُ حَيَاتِيْ.
                        مَعَكِ أَشْعُرُ أَنَّ كُلَّ شَيْءٍ مُمْكِنٌ، وَأَنَّ الحُبَّ الحَقِيقِيَّ وُجِدَ لِيَكُونَ بَيْنَنَا.<br><br>
                        أَحْبُبُكِ بِكُلِّ قَلْبِيْ 💕
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- قسم لماذا أحبها -->
    <section class="reasons-section" id="reasonsSection">
        <div class="container">
            <h2 class="section-title">
                <i class="fas fa-star"></i>
                لِمَاذَا أَحْبَبْتُكِ؟
                <i class="fas fa-star"></i>
            </h2>
            <div class="reasons-grid">
                <div class="reason-card">
                    <div class="reason-icon">
                        <i class="fas fa-smile"></i>
                    </div>
                    <h3>ابتسامتكِ</h3>
                    <p>ابتسامتكِ تُنير عالمي وتُذيب قلبي كل مرة</p>
                </div>
                <div class="reason-card">
                    <div class="reason-icon">
                        <i class="fas fa-heart"></i>
                    </div>
                    <h3>قلبكِ الطيب</h3>
                    <p>قلبكِ الطاهر والجميل هو أجمل ما عرفت</p>
                </div>
                <div class="reason-card">
                    <div class="reason-icon">
                        <i class="fas fa-eye"></i>
                    </div>
                    <h3>عيناكِ</h3>
                    <p>عيناكِ الساحرتان تخبرانني بكل شيء</p>
                </div>
                <div class="reason-card">
                    <div class="reason-icon">
                        <i class="fas fa-brain"></i>
                    </div>
                    <h3>عقلكِ</h3>
                    <p>ذكاؤكِ وروحكِ المرحة تسحرانني</p>
                </div>
                <div class="reason-card">
                    <div class="reason-icon">
                        <i class="fas fa-hands"></i>
                    </div>
                    <h3>حنانكِ</h3>
                    <p>حنانكِ يُشعرني بالأمان والسكينة</p>
                </div>
                <div class="reason-card">
                    <div class="reason-icon">
                        <i class="fas fa-gem"></i>
                    </div>
                    <h3>أنتِ أنتِ</h3>
                    <p>لأنكِ مجرد أنتِ... وهذا يكفي</p>
                </div>
            </div>
        </div>
    </section>

    <!-- قسم العد التنازلي -->
    <section class="countdown-section" id="countdownSection">
        <div class="container">
            <h2 class="section-title">
                <i class="fas fa-clock"></i>
                منذ لحظة لقائي بكِ
            </h2>
            <div class="countdown-container">
                <div class="countdown-box">
                    <span class="countdown-number" id="years">0</span>
                    <span class="countdown-label">سنوات</span>
                </div>
                <div class="countdown-box">
                    <span class="countdown-number" id="months">0</span>
                    <span class="countdown-label">شهور</span>
                </div>
                <div class="countdown-box">
                    <span class="countdown-number" id="days">0</span>
                    <span class="countdown-label">أيام</span>
                </div>
                <div class="countdown-box">
                    <span class="countdown-number" id="hours">0</span>
                    <span class="countdown-label">ساعات</span>
                </div>
            </div>
            <p class="countdown-note">أجمل لحظات حياتي كانت معكِ</p>
        </div>
    </section>

    <!-- قسم الذكريات -->
    <section class="memories-section" id="memoriesSection">
        <div class="container">
            <h2 class="section-title">
                <i class="fas fa-camera"></i>
                ذكرياتنا الجميلة
            </h2>
            <div class="memories-gallery">
                <div class="memory-item">
                    <img src="https://images.unsplash.com/photo-1529333166437-7750a6dd5a70?w=300&h=300&fit=crop" alt="ذكرى 1">
                    <div class="memory-overlay">
                        <p>أول لقاء 💕</p>
                    </div>
                </div>
                <div class="memory-item">
                    <img src="https://images.unsplash.com/photo-1516589178581-6cd7833ae3b2?w=300&h=300&fit=crop" alt="ذكرى 2">
                    <div class="memory-overlay">
                        <p>ضحكتنا Together 😍</p>
                    </div>
                </div>
                <div class="memory-item">
                    <img src="https://images.unsplash.com/photo-1518199266791-5375a83190b7?w=300&h=300&fit=crop" alt="ذكرى 3">
                    <div class="memory-overlay">
                        <p>أجمل الذكريات 🌟</p>
                    </div>
                </div>
                <div class="memory-item">
                    <img src="https://images.unsplash.com/photo-1529634806980-85c3dd6d34ac?w=300&h=300&fit=crop" alt="ذكرى 4">
                    <div class="memory-overlay">
                        <p>حبيبي نور 💖</p>
                    </div>
                </div>
                <div class="memory-item">
                    <img src="https://images.unsplash.com/photo-1491438590914-bc09fcaaf77a?w=300&h=300&fit=crop" alt="ذكرى 5">
                    <div class="memory-overlay">
                        <p>نور عيني 🌺</p>
                    </div>
                </div>
                <div class="memory-item">
                    <img src="https://images.unsplash.com/photo-1485217988980-11786ced9454?w=300&h=300&fit=crop" alt="ذكرى 6">
                    <div class="memory-overlay">
                        <p>حب العمر 💝</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- قسم الرسالة الأخيرة -->
    <section class="final-message" id="finalMessage">
        <div class="container">
            <div class="final-card">
                <div class="final-content">
                    <h2>أخيراً...</h2>
                    <p class="final-text">
                        نُوْرِيْ،<br><br>
                        لَوْ كَانَ الحُبُّ كَلِمَةً، لَكَانَتْ كَلِمَتُكِ الأَوَّلَ وَالأَخِيرَ.<br>
                        لَوْ كَانَ الحُبُّ نَجْمَةً، لَكَانَتْ أَلْمَعَ نَجْمَةٍ فِي السَّمَاء.<br><br>
                        أَنتِ حُبِّي، أَنتِ مَستَقبَلي، أَنتِ كُلُّ شَيْءٍ.<br><br>
                        أُحِبُّكِ بِكُلِّ مَا فِيَّ 💕
                    </p>
                    <div class="signature">
                        <p>إلى الأبد،</p>
                        <p class="lover-name">حبيبكِ الذي أحبكِ</p>
                    </div>
                </div>
                <div class="floating-hearts">
                    <span>💕</span>
                    <span>💖</span>
                    <span>💗</span>
                    <span>💓</span>
                    <span>💕</span>
                </div>
            </div>
        </div>
    </section>

    <!-- التذييل -->
    <footer class="site-footer">
        <div class="container">
            <p>صُنع بكل حب 💕</p>
            <p>لأجمل فتاة في العالم - نور</p>
        </div>
    </footer>

    <script src="script.js"></script>
</body>
</html>
```

---

## 2. ملف التنسيق (style.css)

```css
/* إعدادات عامة */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

:root {
    --primary-color: #e91e63;
    --secondary-color: #ff6b9d;
    --accent-color: #ffc1e3;
    --text-dark: #2d3436;
    --text-light: #636e72;
    --bg-light: #fff5f8;
    --bg-white: #ffffff;
    --shadow: 0 10px 40px rgba(233, 30, 99, 0.15);
    --shadow-hover: 0 20px 60px rgba(233, 30, 99, 0.25);
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: 'Tajawal', 'Amiri', sans-serif;
    background: linear-gradient(135deg, #fff5f8 0%, #ffeef4 50%, #fff5f8 100%);
    color: var(--text-dark);
    line-height: 1.8;
    overflow-x: hidden;
}

/* خلفية القلوب المتحركة */
.hearts-container {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    pointer-events: none;
    z-index: 1000;
    overflow: hidden;
}

.heart-float {
    position: absolute;
    font-size: 20px;
    color: var(--primary-color);
    opacity: 0.3;
    animation: floatHeart 8s linear infinite;
}

@keyframes floatHeart {
    0% {
        transform: translateY(100vh) rotate(0deg);
        opacity: 0;
    }
    10% {
        opacity: 0.3;
    }
    90% {
        opacity: 0.3;
    }
    100% {
        transform: translateY(-100px) rotate(360deg);
        opacity: 0;
    }
}

/* الحاوية العامة */
.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

/* القسم الرئيسي */
.hero-section {
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 100px 20px;
    background: linear-gradient(180deg, rgba(255,255,255,0) 0%, rgba(255,245,248,0.5) 100%);
    position: relative;
}

.hero-content {
    animation: fadeInUp 1s ease-out;
}

@keyframes fadeInUp {
    from {
        opacity: 0;
        transform: translateY(30px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

/* إطار الصورة */
.photo-frame {
    position: relative;
    width: 200px;
    height: 200px;
    margin: 0 auto 30px;
}

.main-photo {
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 50%;
    border: 5px solid var(--bg-white);
    box-shadow: var(--shadow);
    transition: transform 0.3s ease;
}

.main-photo:hover {
    transform: scale(1.05);
}

.frame-decoration {
    position: absolute;
    top: -10px;
    left: -10px;
    right: -10px;
    bottom: -10px;
    border: 3px solid var(--primary-color);
    border-radius: 50%;
    animation: pulse 2s ease-in-out infinite;
}

@keyframes pulse {
    0%, 100% {
        transform: scale(1);
        opacity: 1;
    }
    50% {
        transform: scale(1.05);
        opacity: 0.5;
    }
}

/* العناوين */
.title {
    font-family: 'Amiri', serif;
    font-size: 2.5rem;
    color: var(--primary-color);
    margin-bottom: 10px;
    text-shadow: 2px 2px 4px rgba(233, 30, 99, 0.1);
}

.subtitle {
    font-family: 'Amiri', serif;
    font-size: 3rem;
    color: var(--text-dark);
    margin-bottom: 20px;
    background: linear-gradient(45deg, var(--primary-color), var(--secondary-color));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}

.intro-text {
    font-size: 1.2rem;
    color: var(--text-light);
    margin-bottom: 30px;
}

/* زر البداية */
.start-btn {
    background: linear-gradient(45deg, var(--primary-color), var(--secondary-color));
    color: white;
    border: none;
    padding: 15px 40px;
    font-size: 1.2rem;
    font-family: 'Tajawal', sans-serif;
    border-radius: 50px;
    cursor: pointer;
    transition: all 0.3s ease;
    box-shadow: var(--shadow);
}

.start-btn:hover {
    transform: translateY(-3px);
    box-shadow: var(--shadow-hover);
}

.start-btn i {
    margin-left: 10px;
}

/* قسم رسالة الحب */
.love-message {
    padding: 100px 0; my-websitent-
