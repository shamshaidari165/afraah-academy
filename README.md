<!DOCTYPE html>
<html lang="fa">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Afraah Academy</title>
    <style>
        body {
            font-family: 'Tahoma', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f2f5;
            color: #333;
        }

        header {
            background: linear-gradient(135deg, #1abc9c, #16a085);
            color: white;
            padding: 50px 20px;
            text-align: center;
        }

        header h1 {
            font-size: 3em;
            margin: 0;
        }

        header p {
            font-size: 1.2em;
            margin-top: 10px;
        }

        nav {
            display: flex;
            justify-content: center;
            background-color: #34495e;
        }

        nav a {
            color: white;
            padding: 15px 25px;
            text-decoration: none;
            transition: 0.3s;
        }

        nav a:hover {
            background-color: #1abc9c;
            color: white;
        }

        section {
            padding: 60px 20px;
            max-width: 1100px;
            margin: auto;
        }

        h2 {
            text-align: center;
            margin-bottom: 40px;
            color: #2c3e50;
        }

        .about p, .about ul {
            max-width: 800px;
            margin: auto;
            font-size: 1.1em;
            line-height: 1.8;
        }

        .about ul {
            list-style: disc;
            padding-left: 20px;
        }

        .courses-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
        }

        .course-card {
            background-color: white;
            border-radius: 12px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.1);
            overflow: hidden;
            width: 300px;
            transition: transform 0.3s;
        }

        .course-card:hover {
            transform: translateY(-10px);
        }

        .course-card img {
            width: 100%;
            height: 180px;
            object-fit: cover;
        }

        .course-card .content {
            padding: 20px;
        }

        .course-card h3 {
            margin-top: 0;
            color: #1abc9c;
        }

        .course-card p {
            margin: 10px 0;
            line-height: 1.5;
        }

        .contact-info {
            text-align: center;
            margin-bottom: 30px;
        }

        form {
            max-width: 600px;
            margin: auto;
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        form input, form textarea {
            padding: 12px;
            border-radius: 6px;
            border: 1px solid #ccc;
            font-size: 1em;
        }

        form button {
            padding: 12px;
            border: none;
            background-color: #1abc9c;
            color: white;
            font-size: 1em;
            cursor: pointer;
            border-radius: 6px;
            transition: background 0.3s;
        }

        form button:hover {
            background-color: #16a085;
        }

        footer {
            text-align: center;
            background-color: #34495e;
            color: white;
            padding: 20px 0;
            margin-top: 40px;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .courses-container {
                flex-direction: column;
                align-items: center;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Afraah Academy</h1>
        <p>یادگیری حرفه‌ای گرافیک دیزاین و توسعه وب</p>
    </header>

    <nav>
        <a href="#about">درباره ما</a>
        <a href="#courses">کورس‌ها</a>
        <a href="#contact">تماس با ما</a>
    </nav>

    <section id="about" class="about">
        <h2>درباره ما</h2>
        <p>Afraah Academy یک آکادمی آموزشی است که در زمینه‌های <strong>طراحی گرافیک (Graphic Design)</strong> و <strong>توسعه وب (Web Development)</strong> دوره‌های حرفه‌ای ارائه می‌دهد.</p>
        <p><strong>هدف و ماموریت:</strong></p>
        <ul>
            <li>آموزش مهارت‌های عملی و به‌روز در زمینه گرافیک و وب</li>
            <li>آماده‌سازی دانشجویان برای بازار کار حرفه‌ای</li>
            <li>ایجاد محیط آموزشی دوستانه و خلاق</li>
        </ul>
    </section>

    <section id="courses">
        <h2>کورس‌ها</h2>
        <div class="courses-container">
            <div class="course-card">
                <img src="https://images.unsplash.com/photo-1581091215369-8f8c3d1d3e43?fit=crop&w=400&h=180" alt="Graphic Design">
                <div class="content">
                    <h3>گرافیک دیزاین</h3>
                    <p>آموزش طراحی لوگو، بنر، کارت ویزیت و دیگر مهارت‌های گرافیکی.</p>
                    <p>مدت زمان: ۷ صبح تا ۶ عصر</p>
                </div>
            </div>
            <div class="course-card">
                <img src="https://images.unsplash.com/photo-1521791136064-7986c2920216?fit=crop&w=400&h=180" alt="Web Development">
                <div class="content">
                    <h3>Web Development</h3>
                    <p>آموزش HTML, CSS, JavaScript و فریمورک‌های وب برای ساخت سایت‌های حرفه‌ای.</p>
                    <p>مدت زمان: ۷ صبح تا ۶ عصر</p>
                </div>
            </div>
        </div>
    </section>

    <section id="contact">
        <h2>تماس با ما</h2>
        <div class="contact-info">
            <p>شماره تماس: 0702290730</p>
            <p>ایمیل: afraahacademy@gmail.com</p>
        </div>
        <form>
            <input type="text" placeholder="نام شما" required>
            <input type="email" placeholder="ایمیل شما" required>
            <textarea rows="5" placeholder="پیام شما" required></textarea>
            <button type="submit">ارسال پیام</button>
        </form>
    </section>

    <footer>
        <p>© 2025 Afraah Academy. همه حقوق محفوظ است.</p>
    </footer>
</body>
</html>
