
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Qasem | My Portfolio</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
}

body {
    font-family: Tahoma, Arial, sans-serif;
    background: #080808;
    color: white;
}

/* شاشة البداية */

#intro {
    position: fixed;
    inset: 0;
    z-index: 1000;
    background:
        radial-gradient(circle at center, #29200c, #080808 65%);
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    transition: opacity 1s, visibility 1s;
}

.intro-content {
    padding: 25px;
}

.intro-content .line {
    width: 75px;
    height: 3px;
    background: #d4af37;
    margin: 0 auto 25px;
}

.intro-content h1 {
    font-size: clamp(35px, 7vw, 65px);
    margin-bottom: 15px;
}

.intro-content h1 span {
    color: #d4af37;
}

.intro-content p {
    color: #ccc;
    font-size: 17px;
    margin-bottom: 35px;
}

.explore-btn {
    padding: 15px 45px;
    background: #d4af37;
    color: #080808;
    border: none;
    border-radius: 5px;
    font-size: 18px;
    font-weight: bold;
    cursor: pointer;
    transition: .3s;
}

.explore-btn:hover {
    background: white;
    transform: scale(1.06);
}

.intro-hidden {
    opacity: 0;
    visibility: hidden;
    pointer-events: none;
}

/* الموقع الرئيسي */

header {
    background: #101010;
    border-bottom: 1px solid #d4af37;
    padding: 22px 8%;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    color: #d4af37;
    font-size: 23px;
    font-weight: bold;
}

nav a {
    color: white;
    text-decoration: none;
    margin-right: 18px;
}

nav a:hover {
    color: #d4af37;
}

.hero {
    text-align: center;
    padding: 90px 20px;
    background: linear-gradient(135deg, #171717, #080808);
}

.hero h2 {
    font-size: 38px;
    margin-bottom: 15px;
}

.hero h2 span {
    color: #d4af37;
}

.hero p {
    color: #bbb;
    font-size: 17px;
    line-height: 2;
}

.section {
    padding: 70px 8%;
}

.title {
    text-align: center;
    margin-bottom: 40px;
}

.title h2 {
    color: #d4af37;
    font-size: 32px;
}

.title p {
    color: #aaa;
    margin-top: 10px;
}

.projects {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(270px, 1fr));
    gap: 25px;
}

.card {
    background: #151515;
    border: 1px solid #333;
    border-radius: 10px;
    overflow: hidden;
    transition: .4s;
}

.card:hover {
    transform: translateY(-8px);
    border-color: #d4af37;
}

.card img {
    width: 100%;
    height: 220px;
    object-fit: cover;
    display: block;
    transition: .4s;
}

.card:hover img {
    transform: scale(1.04);
}

.card-content {
    padding: 22px;
}

.card h3 {
    color: #d4af37;
    font-size: 23px;
    margin-bottom: 12px;
}

.card p {
    color: #bbb;
    line-height: 1.9;
    margin-bottom: 20px;
}

.card a {
    display: inline-block;
    background: #d4af37;
    color: #080808;
    text-decoration: none;
    padding: 10px 20px;
    border-radius: 5px;
    font-weight: bold;
}

.card a:hover {
    background: white;
}

.about {
    background: #111;
    text-align: center;
}

.about h2 {
    color: #d4af37;
    margin-bottom: 20px;
}

.about p {
    max-width: 700px;
    margin: auto;
    color: #ccc;
    line-height: 2;
}

footer {
    background: #050505;
    text-align: center;
    padding: 30px;
    color: #aaa;
}

@media(max-width:600px) {
    header {
        flex-direction: column;
        gap: 15px;
    }

    .hero h2 {
        font-size: 29px;
    }
}
</style>
</head>

<body>

<!-- واجهة الدخول -->

<div id="intro">

    <div class="intro-content">

        <div class="line"></div>

        <h1>
            مرحباً بك في عالم
            <span>قاسم</span>
        </h1>

        <p>
            معرض أعمالي ومشاريعي الرقمية
        </p>

        <button class="explore-btn" onclick="enterSite()">
            استكشف أعمالي
        </button>

    </div>

</div>

<!-- الموقع -->

<header>

    <div class="logo">QASEM.</div>

    <nav>
        <a href="#home">الرئيسية</a>
        <a href="#projects">مشاريعي</a>
        <a href="#about">من أنا</a>
    </nav>

</header>

<section class="hero" id="home">

    <h2>
        أنا <span>قاسم حسن قاسم</span>
    </h2>

    <p>
        أهلاً بك في معرض مشاريعي وأعمالي.
        هنا تجد المواقع التي قمت بتصميمها وتطويرها.
    </p>

</section>

<section class="section" id="projects">

    <div class="title">
        <h2>مشاريعي وأعمالي</h2>
        <p>استعرض مشاريعي الرقمية واكتشف أعمالي</p>
    </div>

    <div class="projects">

        <div class="card">

            <a href="https://hss06301-maker.github.io/-6/"
               target="_blank">

                <img
                src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?w=900"
                alt="السيرة الذاتية">

            </a>

            <div class="card-content">

                <h3>السيرة الذاتية</h3>

                <p>
                    موقعي الشخصي للتعريف بي
                    واستعراض معلوماتي ومهاراتي.
                </p>

                <a href="https://hss06301-maker.github.io/-6/"
                   target="_blank">
                    استكشف المشروع
                </a>

            </div>

        </div>

        <div class="card">

            <a href="https://hss06301-maker.github.io/New-shop/"
               target="_blank">

                <img
                src="https://images.unsplash.com/photo-1552728089-57bdde30beb3?w=900"
                alt="عالم الطيور">

            </a>

            <div class="card-content">

                <h3>متجر عالم الطيور</h3>

                <p>
                    متجر إلكتروني لعرض الطيور
                    وطيور الزينة.
                </p>

                <a href="https://hss06301-maker.github.io/New-shop/"
                   target="_blank">
                    استكشف المشروع
                </a>

            </div>

        </div>

    </div>

</section>

<section class="section about" id="about">

    <h2>من أنا؟</h2>

    <p>
        أنا قاسم حسن قاسم، مهتم بالتقنية
        وتصميم وتطوير المواقع الإلكترونية
        وإنشاء المشاريع الرقمية.
    </p>

</section>

<footer>
    <p>QASEM HASSAN QASEM</p>
    <p>© 2026 جميع الحقوق محفوظة</p>
</footer>

<script>

function enterSite() {

    document.getElementById("intro")
    .classList.add("intro-hidden");

    window.scrollTo({
        top: 0,
        behavior: "smooth"
    });

}

</script>

</body>
</html>
