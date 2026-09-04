<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>رایان افزار | فروشگاه تخصصی کامپیوتر</title>

<meta name="description"
      content="رایان افزار، فروشگاه کامپیوتر و تجهیزات دیجیتال">

<style>

/* =====================================================
   RESET
===================================================== */

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    font-family:
        Tahoma,
        Arial,
        sans-serif;

    color:var(--text);

    background:
        radial-gradient(
            circle at 10% 5%,
            rgba(124,60,255,.18),
            transparent 25%
        ),
        radial-gradient(
            circle at 90% 12%,
            rgba(0,217,255,.12),
            transparent 25%
        ),
        radial-gradient(
            circle at 50% 85%,
            rgba(255,43,214,.08),
            transparent 28%
        ),
        linear-gradient(
            135deg,
            var(--bg),
            var(--bg2)
        );

    background-attachment:fixed;

    overflow-x:hidden;

    transition:.4s;
}


/* =====================================================
   VARIABLES
===================================================== */

:root{

    --bg:#05060b;
    --bg2:#090b14;

    --card:rgba(16,18,30,.68);

    --text:#f6f7ff;

    --muted:#9ca3b8;

    --primary:#7c3cff;

    --secondary:#00d9ff;

    --accent:#ff2bd6;

    --green:#00f5a0;

    --border:
        rgba(255,255,255,.10);

    --shadow:
        0 25px 80px rgba(0,0,0,.42);
}


/* =====================================================
   BACKGROUND GRID
===================================================== */

body::before{

    content:"";

    position:fixed;

    inset:0;

    pointer-events:none;

    z-index:-1;

    background-image:

        linear-gradient(
            rgba(255,255,255,.018) 1px,
            transparent 1px
        ),

        linear-gradient(
            90deg,
            rgba(255,255,255,.018) 1px,
            transparent 1px
        );

    background-size:50px 50px;

    mask-image:
        linear-gradient(
            to bottom,
            black,
            transparent 90%
        );
}


/* =====================================================
   HEADER
===================================================== */

header{

    position:sticky;

    top:14px;

    z-index:999;

    width:min(1180px,92%);

    margin:14px auto 0;

    padding:13px 18px;

    display:flex;

    align-items:center;

    justify-content:space-between;

    gap:20px;

    background:
        rgba(9,11,20,.68);

    border:
        1px solid var(--border);

    border-radius:22px;

    backdrop-filter:
        blur(22px);

    -webkit-backdrop-filter:
        blur(22px);

    box-shadow:
        var(--shadow),
        inset 0 1px rgba(255,255,255,.06);
}


.logo{

    font-size:24px;

    font-weight:900;

    white-space:nowrap;

    background:
        linear-gradient(
            90deg,
            #fff,
            var(--secondary),
            var(--primary)
        );

    -webkit-background-clip:text;

    background-clip:text;

    color:transparent;
}


nav{

    display:flex;

    align-items:center;

    justify-content:center;

    gap:6px;

    flex-wrap:wrap;
}


nav a{

    color:#cfd3e3;

    text-decoration:none;

    font-size:13px;

    padding:10px 13px;

    border-radius:12px;

    transition:.25s;
}


nav a:hover{

    color:#fff;

    background:
        rgba(255,255,255,.07);

    box-shadow:
        0 0 18px
        rgba(124,60,255,.12);
}


.theme-btn{

    width:42px;

    height:42px;

    border-radius:13px;

    cursor:pointer;

    border:
        1px solid var(--border);

    background:
        rgba(255,255,255,.06);

    color:#fff;

    font-size:19px;

    transition:.25s;
}


.theme-btn:hover{

    transform:
        rotate(12deg)
        scale(1.06);

    border-color:
        rgba(0,217,255,.45);
}


/* =====================================================
   HERO
===================================================== */

.hero{

    min-height:720px;

    display:flex;

    align-items:center;

    justify-content:center;

    text-align:center;

    padding:
        110px
        20px
        90px;

    position:relative;

    isolation:isolate;
}


.hero::before,
.hero::after{

    content:"";

    position:absolute;

    border-radius:50%;

    pointer-events:none;

    z-index:-1;

    filter:blur(3px);
}


.hero::before{

    width:380px;

    height:380px;

    background:
        rgba(124,60,255,.16);

    top:8%;

    left:4%;

    box-shadow:
        0 0 160px
        rgba(124,60,255,.25);
}


.hero::after{

    width:300px;

    height:300px;

    background:
        rgba(0,217,255,.11);

    bottom:8%;

    right:5%;

    box-shadow:
        0 0 150px
        rgba(0,217,255,.2);
}


.hero-content{

    max-width:920px;
}


.badge{

    display:inline-flex;

    align-items:center;

    gap:8px;

    padding:
        10px 17px;

    margin-bottom:22px;

    border-radius:999px;

    color:#d9d3ff;

    background:
        rgba(124,60,255,.10);

    border:
        1px solid
        rgba(124,60,255,.35);

    font-size:13px;
}


.hero h1{

    font-size:
        clamp(40px,7vw,76px);

    line-height:1.18;

    margin-bottom:22px;

    font-weight:950;

    letter-spacing:-2px;
}


.hero h1 span{

    background:
        linear-gradient(
            90deg,
            var(--secondary),
            #fff,
            var(--accent),
            var(--primary)
        );

    background-size:
        250% auto;

    -webkit-background-clip:text;

    background-clip:text;

    color:transparent;

    animation:
        gradientMove 5s linear infinite;
}


@keyframes gradientMove{

    to{
        background-position:
            250% center;
    }

}


.hero p{

    color:#aeb5c9;

    font-size:17px;

    line-height:2;

    max-width:700px;

    margin:auto;
}


.hero-buttons{

    margin-top:34px;

    display:flex;

    justify-content:center;

    gap:12px;

    flex-wrap:wrap;
}


.main-btn,
.second-btn,
.installment-btn{

    display:inline-flex;

    align-items:center;

    justify-content:center;

    gap:8px;

    border-radius:14px;

    padding:
        14px 24px;

    font-weight:800;

    text-decoration:none;

    transition:.28s;

    cursor:pointer;
}


.main-btn{

    border:
        1px solid
        rgba(255,255,255,.12);

    background:
        linear-gradient(
            110deg,
            var(--primary),
            #5b2cff,
            var(--secondary)
        );

    color:#fff;

    box-shadow:
        0 12px 35px
        rgba(91,44,255,.30);
}


.main-btn:hover{

    transform:
        translateY(-4px);

    box-shadow:
        0 18px 50px
        rgba(0,217,255,.22);
}


.second-btn{

    background:
        rgba(255,255,255,.055);

    color:#fff;

    border:
        1px solid var(--border);

    backdrop-filter:
        blur(14px);
}


.second-btn:hover{

    transform:
        translateY(-4px);

    border-color:
        rgba(0,217,255,.4);

    background:
        rgba(0,217,255,.07);
}


/* =====================================================
   INSTALLMENT
===================================================== */

.installment{

    width:min(1180px,88%);

    margin:
        0 auto 30px;

    padding:32px;

    border-radius:26px;

    display:flex;

    align-items:center;

    justify-content:space-between;

    gap:25px;

    flex-wrap:wrap;

    background:
        linear-gradient(
            115deg,
            rgba(124,60,255,.22),
            rgba(0,217,255,.12),
            rgba(255,43,214,.10)
        );

    border:
        1px solid
        rgba(255,255,255,.12);

    box-shadow:
        var(--shadow),
        0 0 70px
        rgba(124,60,255,.10);

    backdrop-filter:
        blur(18px);
}


.installment h2{

    font-size:26px;

    margin-bottom:9px;
}


.installment p{

    line-height:2;

    color:#c0c5d6;
}


.installment-btn{

    background:#fff;

    color:#10121c;

    position:relative;

    z-index:2;
}


.installment-btn:hover{

    transform:
        translateY(-3px);

    box-shadow:
        0 12px 30px
        rgba(255,255,255,.15);
}


/* =====================================================
   GENERAL SECTION
===================================================== */

.section{

    padding:
        90px 6%;
}


.section-title{

    text-align:center;

    margin-bottom:44px;
}


.section-title h2{

    font-size:32px;

    margin-bottom:11px;
}


.section-title p{

    color:var(--muted);
}


/* =====================================================
   3D COVERFLOW
===================================================== */

.coverflow-section{

    padding:
        80px 5% 55px;

    position:relative;

    overflow:hidden;
}


.coverflow-section::before{

    content:"";

    position:absolute;

    width:700px;

    height:400px;

    left:50%;

    top:50%;

    transform:
        translate(-50%,-50%);

    background:
        radial-gradient(
            ellipse,
            rgba(124,60,255,.22),
            transparent 70%
        );

    filter:blur(20px);

    pointer-events:none;
}


.coverflow-wrap{

    width:min(1250px,100%);

    margin:auto;

    position:relative;
}


.coverflow{

    height:510px;

    position:relative;

    perspective:1800px;

    transform-style:preserve-3d;

    touch-action:pan-y;

    user-select:none;

    cursor:grab;
}


.coverflow:active{

    cursor:grabbing;
}


.coverflow-card{

    position:absolute;

    left:50%;

    top:50%;

    width:min(350px,74vw);

    height:405px;

    transform-style:preserve-3d;

    border-radius:32px;

    overflow:hidden;

    padding:27px;

    display:flex;

    flex-direction:column;

    justify-content:flex-end;

    background:
        linear-gradient(
            145deg,
            rgba(25,29,52,.98),
            rgba(4,6,14,.99)
        );

    border:
        1px solid
        rgba(255,255,255,.14);

    box-shadow:
        0 40px 100px
        rgba(0,0,0,.65),
        inset 0 1px
        rgba(255,255,255,.1);

    transition:
        transform .75s
        cubic-bezier(.16,.86,.22,1),
        opacity .5s,
        filter .5s,
        box-shadow .5s;

    will-change:transform;

    isolation:isolate;

    cursor:pointer;
}


.coverflow-card::before{

    content:"";

    position:absolute;

    inset:-2px;

    border-radius:inherit;

    background:
        conic-gradient(
            from 180deg,
            transparent,
            #00d9ff,
            #ff2bd6,
            #7c3cff,
            transparent
        );

    opacity:0;

    transition:.5s;

    z-index:-3;
}


.coverflow-card::after{

    content:"";

    position:absolute;

    inset:0;

    z-index:-1;

    background:
        radial-gradient(
            circle at 50% 25%,
            rgba(0,217,255,.2),
            transparent 35%
        ),
        linear-gradient(
            to top,
            rgba(2,3,9,.99),
            rgba(2,3,9,.35) 60%,
            transparent
        );
}


.coverflow-card.active{

    border-color:
        rgba(0,217,255,.6);

    box-shadow:
        0 50px 120px
        rgba(0,0,0,.72),
        0 0 70px
        rgba(0,217,255,.18),
        0 0 25px
        rgba(124,60,255,.2),
        inset 0 1px
        rgba(255,255,255,.15);
}


.coverflow-card.active::before{

    opacity:.5;
}


.cf-icon{

    position:absolute;

    top:25px;

    left:25px;

    right:25px;

    height:245px;

    display:grid;

    place-items:center;

    font-size:115px;

    border-radius:25px;

    background:
        radial-gradient(
            circle,
            rgba(0,217,255,.2),
            transparent 45%
        ),
        radial-gradient(
            circle,
            rgba(124,60,255,.15),
            transparent 70%
        );

    border:
        1px solid
        rgba(255,255,255,.06);

    text-shadow:
        0 0 25px
        rgba(0,217,255,.4),
        0 0 60px
        rgba(124,60,255,.25);

    transform:
        translateZ(30px);
}


.coverflow-card h3{

    font-size:25px;

    margin-bottom:10px;

    transform:
        translateZ(20px);
}


.coverflow-card p{

    color:#aeb5c9;

    font-size:13px;

    line-height:1.9;

    transform:
        translateZ(15px);
}


.cf-tag{

    width:max-content;

    margin-bottom:12px;

    padding:
        6px 13px;

    border-radius:999px;

    font-size:10px;

    letter-spacing:1.5px;

    color:#e9fcff;

    background:
        rgba(0,217,255,.08);

    border:
        1px solid
        rgba(0,217,255,.25);
}


.cf-controls{

    display:flex;

    justify-content:center;

    align-items:center;

    gap:15px;

    position:relative;

    z-index:50;
}


.cf-arrow{

    width:53px;

    height:53px;

    border-radius:17px;

    border:
        1px solid
        rgba(255,255,255,.11);

    background:
        rgba(255,255,255,.065);

    color:white;

    font-size:23px;

    cursor:pointer;

    transition:.28s;

    backdrop-filter:
        blur(16px);
}


.cf-arrow:hover{

    transform:
        translateY(-4px)
        scale(1.08);

    border-color:
        rgba(0,217,255,.5);

    box-shadow:
        0 0 30px
        rgba(0,217,255,.18);
}


.cf-dots{

    display:flex;

    align-items:center;

    gap:8px;
}


.cf-dot{

    width:7px;

    height:7px;

    border:0;

    border-radius:50%;

    background:
        rgba(255,255,255,.23);

    cursor:pointer;

    transition:.35s;
}


.cf-dot.active{

    width:30px;

    background:
        var(--secondary);

    box-shadow:
        0 0 18px
        rgba(0,217,255,.6);
}


.coverflow-hint{

    text-align:center;

    color:#70788d;

    font-size:12px;

    margin-top:14px;
}


/* =====================================================
   SPECIAL OFFER
===================================================== */

.special{

    max-width:1180px;

    margin:auto;

    display:grid;

    grid-template-columns:
        1fr 1fr;

    gap:30px;

    align-items:center;

    padding:30px;

    border-radius:27px;

    background:
        rgba(15,18,31,.62);

    border:
        1px solid var(--border);

    box-shadow:
        var(--shadow);

    backdrop-filter:
        blur(18px);
}


.special-icon{

    min-height:240px;

    display:flex;

    justify-content:center;

    align-items:center;

    font-size:115px;

    border-radius:22px;

    background:
        radial-gradient(
            circle,
            rgba(255,43,214,.13),
            transparent 58%
        ),
        linear-gradient(
            135deg,
            rgba(124,60,255,.12),
            rgba(0,217,255,.08)
        );

    border:
        1px solid
        rgba(255,255,255,.07);
}


.special h2{

    color:#dcd5ff;

    margin-bottom:15px;
}


.special p{

    color:var(--muted);

    line-height:2;
}


.special-price{

    margin:20px 0;

    font-size:24px;

    color:var(--green);

    font-weight:900;
}


/* =====================================================
   FEATURES
===================================================== */

.features{

    display:grid;

    grid-template-columns:
        repeat(
            auto-fit,
            minmax(200px,1fr)
        );

    gap:18px;

    max-width:1180px;

    margin:auto;
}


.feature{

    text-align:center;

    padding:27px;

    border-radius:21px;

    background:
        rgba(14,17,29,.58);

    border:
        1px solid var(--border);

    box-shadow:
        var(--shadow);

    backdrop-filter:
        blur(16px);

    transition:.3s;
}


.feature:hover{

    transform:
        translateY(-6px);

    border-color:
        rgba(124,60,255,.35);
}


.feature-icon{

    font-size:38px;

    margin-bottom:12px;
}


.feature h3{

    margin-bottom:10px;
}


.feature p{

    color:var(--muted);

    font-size:14px;

    line-height:1.8;
}


/* =====================================================
   CART
===================================================== */

.cart{

    max-width:1180px;

    margin:auto;

    padding:30px;

    border-radius:25px;

    background:
        rgba(14,17,29,.62);

    border:
        1px solid var(--border);

    box-shadow:
        var(--shadow);

    backdrop-filter:
        blur(18px);
}


.cart h2{

    color:#ddd6ff;

    margin-bottom:20px;
}


#cartItems{

    color:var(--muted);

    line-height:2.4;
}


.total{

    margin-top:20px;

    padding-top:20px;

    border-top:
        1px solid
        var(--border);

    color:var(--green);

    font-size:19px;

    font-weight:900;
}


/* =====================================================
   SOCIAL
===================================================== */

.social-grid{

    max-width:1180px;

    margin:auto;

    display:grid;

    grid-template-columns:
        repeat(3,1fr);

    gap:16px;
}


.social-card{

    min-height:92px;

    display:flex;

    align-items:center;

    gap:15px;

    padding:18px;

    border-radius:21px;

    text-decoration:none;

    color:#fff;

    background:
        linear-gradient(
            145deg,
            rgba(19,22,37,.82),
            rgba(8,10,18,.72)
        );

    border:
        1px solid var(--border);

    box-shadow:
        var(--shadow);

    backdrop-filter:
        blur(16px);

    transition:.3s;
}


.social-card:hover{

    transform:
        translateY(-6px)
        scale(1.015);

    border-color:
        rgba(0,217,255,.42);

    box-shadow:
        0 25px 65px
        rgba(0,0,0,.45);
}


.social-icon{

    width:52px;

    height:52px;

    min-width:52px;

    display:grid;

    place-items:center;

    border-radius:16px;

    font-size:25px;

    background:
        rgba(255,255,255,.06);

    border:
        1px solid
        rgba(255,255,255,.09);
}


.social-card strong{

    display:block;

    font-size:16px;

    margin-bottom:5px;
}


.social-card small{

    display:block;

    color:#9ca3b8;

    line-height:1.6;

    font-size:12px;

    direction:ltr;

    text-align:right;
}


.service-strip{

    max-width:1180px;

    margin:
        24px auto 0;

    display:flex;

    justify-content:center;

    flex-wrap:wrap;

    gap:10px;
}


.service-strip span{

    padding:
        10px 13px;

    border-radius:999px;

    color:#cbd1e2;

    background:
        rgba(255,255,255,.045);

    border:
        1px solid
        rgba(255,255,255,.08);

    font-size:12px;
}


/* =====================================================
   CONTACT
===================================================== */

.contact{

    text-align:center;

    padding:
        95px 20px;

    background:
        radial-gradient(
            circle at center,
            rgba(124,60,255,.12),
            transparent 45%
        );
}


.contact h2{

    font-size:32px;

    margin-bottom:18px;
}


.contact p{

    color:var(--muted);

    line-height:2.4;
}


.phone{

    display:inline-block;

    margin-top:20px;

    color:var(--secondary);

    font-size:25px;

    font-weight:900;

    text-decoration:none;
}


.address{

    margin:
        25px auto;

    max-width:550px;

    background:
        rgba(255,255,255,.04);

    border:
        1px solid var(--border);

    padding:20px;

    border-radius:17px;

    line-height:2;

    color:#e8eaf2;

    backdrop-filter:
        blur(14px);
}


/* =====================================================
   FOOTER
===================================================== */

footer{

    background:#03040a;

    color:#747b8f;

    text-align:center;

    padding:
        38px 20px;

    line-height:2;

    border-top:
        1px solid
        rgba(255,255,255,.07);
}


footer strong{

    color:var(--secondary);

    font-size:20px;
}


/* =====================================================
   ANIMATIONS
===================================================== */

.hero-content,
.installment,
.special,
.feature,
.cart,
.social-card{

    animation:
        riseIn .8s ease both;
}


@keyframes riseIn{

    from{

        opacity:0;

        transform:
            translateY(18px);
    }

    to{

        opacity:1;

        transform:
            translateY(0);
    }
}


/* =====================================================
   LIGHT MODE
===================================================== */

body:not(.dark){

    --bg:#eef1f8;

    --bg2:#f7f8fc;

    --text:#151827;

    --muted:#687086;

    --border:
        rgba(20,30,60,.10);
}


body:not(.dark) header{

    background:
        rgba(255,255,255,.76);
}


body:not(.dark)
.installment{

    color:#151827;
}


body:not(.dark)
nav a{

    color:#343a4b;
}


body:not(.dark)
.hero p{

    color:#5d6578;
}


body:not(.dark)
.special,
body:not(.dark)
.feature,
body:not(.dark)
.cart{

    background:
        rgba(255,255,255,.72);
}


/* =====================================================
   MOBILE
===================================================== */

@media(max-width:850px){

    .social-grid{

        grid-template-columns:
            repeat(2,1fr);
    }

}


@media(max-width:700px){

    header{

        top:8px;

        width:94%;

        margin-top:8px;

        flex-direction:column;

        gap:9px;

        padding:12px;
    }


    nav{

        justify-content:center;
    }


    nav a{

        padding:
            8px 9px;

        font-size:12px;
    }


    .hero{

        min-height:620px;

        padding:
            90px
            16px
            65px;
    }


    .hero h1{

        font-size:40px;

        letter-spacing:-1px;
    }


    .hero p{

        font-size:15px;
    }


    .installment{

        width:92%;

        padding:25px;
    }


    .section{

        padding:
            65px 15px;
    }


    .special{

        grid-template-columns:1fr;

        padding:20px;
    }


    .special-icon{

        min-height:180px;

        font-size:90px;
    }


    .section-title h2{

        font-size:27px;
    }


    .coverflow-section{

        padding:
            65px 8px 35px;
    }


    .coverflow{

        height:435px;
    }


    .coverflow-card{

        width:min(292px,77vw);

        height:360px;

        padding:21px;
    }


    .cf-icon{

        height:205px;

        font-size:88px;
    }


    .coverflow-card h3{

        font-size:20px;
    }


    .social-grid{

        grid-template-columns:1fr;
    }

}


@media(prefers-reduced-motion:reduce){

    *,
    *::before,
    *::after{

        animation-duration:.01ms !important;

        animation-iteration-count:1 !important;

        scroll-behavior:auto !important;

        transition-duration:.01ms !important;
    }

}

</style>
</head>


<body>


<!-- =====================================================
     HEADER
===================================================== -->

<header>

    <div class="logo">
        ⚡ رایان افزار
    </div>

    <nav>

        <a href="#home">
            خانه
        </a>

        <a href="#showcase">
            محصولات
        </a>

        <a href="#installment">
            اقساط
        </a>

        <a href="#social">
            📲 ارتباط
        </a>

        <a href="#contact">
            تماس
        </a>

        <a href="#cart">
            🛒 سبد
        </a>

        <button
            class="theme-btn"
            id="themeButton"
            onclick="changeTheme()">

            🌙

        </button>

    </nav>

</header>


<!-- =====================================================
     HERO
===================================================== -->

<section
    class="hero"
    id="home">

    <div class="hero-content">

        <div class="badge">

            ✨ فروشگاه رایان افزار سمنان

        </div>


        <h1>

            تکنولوژی بهتر،

            <span>
                انتخاب بهتر
            </span>

            🚀

        </h1>


        <p>

            در رایان افزار تلاش می‌کنیم
            خرید تجهیزات کامپیوتری را
            ساده، مطمئن و لذت‌بخش کنیم.

        </p>


        <div class="hero-buttons">

            <button
                class="main-btn"
                onclick="goProducts()">

                🔥 مشاهده محصولات

            </button>


            <a
                class="second-btn"
                href="tel:09129582157">

                📞 تماس با ما

            </a>

        </div>

    </div>

</section>


<!-- =====================================================
     INSTALLMENT
===================================================== -->

<section
    class="installment"
    id="installment">

    <div>

        <h2>
            💳 خرید اقساطی بدون بهره
        </h2>

        <p>

            خرید راحت‌تر،
            پرداخت آسان‌تر.

            برای اطلاع از شرایط اقساط
            با فروشگاه تماس بگیرید.

        </p>

    </div>


    <a
        class="installment-btn"
        href="tel:09129582157">

        📞 استعلام شرایط اقساط

    </a>

</section>


<!-- =====================================================
     3D SHOWCASE
===================================================== -->

<section
    class="coverflow-section"
    id="showcase">


    <div class="section-title">

        <h2>
            🚀 ویترین سه‌بعدی رایان افزار
        </h2>

        <p>
            ویترین را بچرخان و محصولات را تماشا کن
        </p>

    </div>


    <div class="coverflow-wrap">

        <div
            class="coverflow"
            id="coverflow">


            <!-- 1 -->

            <article class="coverflow-card">

                <div class="cf-icon">
                    💻
                </div>

                <span class="cf-tag">
                    LAPTOP
                </span>

                <h3>
                    لپ‌تاپ
                </h3>

                <p>
                    لپ‌تاپ‌های متنوع برای
                    کار، دانشگاه، طراحی،
                    برنامه‌نویسی و استفاده روزمره.
                </p>

            </article>


            <!-- 2 -->

            <article class="coverflow-card">

                <div class="cf-icon">
                    🖥️
                </div>

                <span class="cf-tag">
                    DISPLAY
                </span>

                <h3>
                    مانیتورهای حرفه‌ای
                </h3>

                <p>
                    انتخاب مناسب برای گیم،
                    کار، طراحی و استفاده روزمره.
                </p>

            </article>


            <!-- 3 -->

            <article class="coverflow-card">

                <div class="cf-icon">
                    🎮
                </div>

                <span class="cf-tag">
                    GAMING
                </span>

                <h3>
                    تجهیزات گیمینگ
                </h3>

                <p>
                    تجهیزات مناسب برای ساخت
                    یک ست گیمینگ کامل.
                </p>

            </article>


            <!-- 4 -->

            <article class="coverflow-card">

                <div class="cf-icon">
                    🧩
                </div>

                <span class="cf-tag">
                    HARDWARE
                </span>

                <h3>
                    قطعات کامپیوتر
                </h3>

                <p>
                    قطعات و لوازم مورد نیاز
                    برای ارتقا و اسمبل سیستم.
                </p>

            </article>


            <!-- 5 -->

            <article class="coverflow-card">

                <div class="cf-icon">
                    🎧
                </div>

                <span class="cf-tag">
                    AUDIO
                </span>

                <h3>
                    هدفون و هدست
                </h3>

                <p>
                    تجهیزات صوتی برای
                    موسیقی، بازی و کار.
                </p>

            </article>


            <!-- 6 -->

            <article class="coverflow-card">

                <div class="cf-icon">
                    ⭐
                </div>

                <span class="cf-tag">
                    SPECIAL
                </span>

                <h3>
                    پیشنهاد ویژه
                </h3>

                <p>
                    برای اطلاع از تخفیف‌ها،
                    موجودی و قیمت تماس بگیرید.
                </p>

            </article>


        </div>


        <div class="cf-controls">

            <button
                class="cf-arrow"
                id="cfPrev"
                aria-label="قبلی">

                →

            </button>


            <div
                class="cf-dots"
                id="cfDots">
            </div>


            <button
                class="cf-arrow"
                id="cfNext"
                aria-label="بعدی">

                ←

            </button>

        </div>


        <div class="coverflow-hint">

            👆 لمس و کشیدن
            •
            🖱️ موس
            •
            ⌨️ کلیدهای ← →

        </div>

    </div>

</section>


<!-- =====================================================
     SPECIAL OFFER
===================================================== -->

<section class="section">

    <div class="section-title">

        <h2>
            ⭐ پیشنهاد ویژه رایان افزار
        </h2>

        <p>
            هر روز یک پیشنهاد جذاب
        </p>

    </div>


    <div class="special">

        <div class="special-icon">
            🎁
        </div>


        <div>

            <h2>
                پیشنهاد ویژه امروز 🔥
            </h2>

            <p>

                برای اطلاع از پیشنهادهای ویژه،
                تخفیف‌ها و محصولات موجود،
                با فروشگاه رایان افزار تماس بگیرید.

            </p>


            <div class="special-price">
                تخفیف‌های ویژه
            </div>


            <a
                href="tel:09129582157"
                class="main-btn">

                📞 دریافت پیشنهاد

            </a>

        </div>

    </div>

</section>


<!-- =====================================================
     FEATURES
===================================================== -->

<section class="section">

    <div class="section-title">

        <h2>
            چرا رایان افزار؟
        </h2>

        <p>
            خدمات و مزایای فروشگاه
        </p>

    </div>


    <div class="features">


        <div class="feature">

            <div class="feature-icon">
                💳
            </div>

            <h3>
                اقساط بدون بهره
            </h3>

            <p>
                امکان خرید اقساطی
                طبق شرایط فروشگاه.
            </p>

        </div>


        <div class="feature">

            <div class="feature-icon">
                🔧
            </div>

            <h3>
                تعمیرات تخصصی
            </h3>

            <p>
                خدمات تعمیر و عیب‌یابی
                تخصصی لپ‌تاپ و کامپیوتر.
            </p>

        </div>


        <div class="feature">

            <div class="feature-icon">
                🧩
            </div>

            <h3>
                قطعات و لوازم جانبی
            </h3>

            <p>
                انواع قطعات و لوازم
                جانبی کامپیوتر.
            </p>

        </div>


        <div class="feature">

            <div class="feature-icon">
                🛠️
            </div>

            <h3>
                اسمبل و ارتقا
            </h3>

            <p>
                اسمبل، ارتقا و
                بهینه‌سازی سیستم.
            </p>

        </div>


    </div>

</section>


<!-- =====================================================
     CART
===================================================== -->

<section
    class="section"
    id="cart">

    <div class="cart">

        <h2>
            🛒 سبد خرید
        </h2>

        <div id="cartItems">

            برای خرید و اطلاع از قیمت
            محصولات با ما تماس بگیرید.

        </div>


        <div class="total">

            📞 0912 958 2157

            &nbsp; | &nbsp;

            📱 0920 958 2157

        </div>

    </div>

</section>


<!-- =====================================================
     SOCIAL
===================================================== -->

<section
    class="section"
    id="social">

    <div class="section-title">

        <h2>
            📲 ارتباط با رایان افزار
        </h2>

        <p>
            از طریق شبکه‌های اجتماعی با ما در ارتباط باشید
        </p>

    </div>


    <div class="social-grid">


        <a
            class="social-card telegram"
            href="https://t.me/rayanAfzar_official"
            target="_blank"
            rel="noopener">

            <div class="social-icon">
                ✈️
            </div>

            <div>

                <strong>
                    Telegram
                </strong>

                <small>
                    @rayanAfzar_official
                </small>

            </div>

        </a>


        <a
            class="social-card instagram"
            href="https://www.instagram.com/rayanafzar_official?utm_source=qr&igsh=MWtldzA2OWt1ZHhkZg=="
            target="_blank"
            rel="noopener">

            <div class="social-icon">
                📸
            </div>

            <div>

                <strong>
                    Instagram
                </strong>

                <small>
                    @rayanafzar_official
                </small>

            </div>

        </a>


        <a
            class="social-card whatsapp"
            href="https://wa.me/989129582157"
            target="_blank"
            rel="noopener">

            <div class="social-icon">
                💬
            </div>

            <div>

                <strong>
                    WhatsApp
                </strong>

                <small>
                    0912 958 2157
                </small>

            </div>

        </a>


    </div>


    <div class="service-strip">

        <span>
            💻 فروش لپ‌تاپ
        </span>

        <span>
            🔧 تعمیرات تخصصی
        </span>

        <span>
            🧩 قطعات و لوازم
        </span>

        <span>
            🪟 نصب ویندوز
        </span>

        <span>
            🎮 نصب بازی
        </span>

        <span>
            🛠️ اسمبل و ارتقا
        </span>

        <span>
            🧹 سرویس و نظافت
        </span>

        <span>
            🔍 عیب‌یابی
        </span>

    </div>

</section>


<!-- =====================================================
     CONTACT
===================================================== -->

<section
    class="contact"
    id="contact">


    <h2>
        📍 منتظر دیدارتون هستیم
    </h2>


    <p>

        برای قیمت،
        موجودی و شرایط اقساط
        با ما تماس بگیرید.

    </p>


    <a
        class="phone"
        href="tel:09129582157">

        📞 09129582157

    </a>


    <div class="address">

        📍

        <strong>
            آدرس فروشگاه
        </strong>

        <br>

        سمنان،
        شهرک گلستان،
        میدان فرهنگ،
        ضلع جنوبی،
        فروشگاه رایان افزار

    </div>


    <a
        href="tel:09129582157"
        class="main-btn">

        📞 تماس با فروشگاه

    </a>

</section>


<!-- =====================================================
     FOOTER
===================================================== -->

<footer>

    <strong>
        ⚡ رایان افزار
    </strong>

    <br>

    فروشگاه کامپیوتر و تجهیزات دیجیتال

    <br>

    سمنان |
    شهرک گلستان |
    میدان فرهنگ

    <br>

    📞 09129582157

    <br><br>

    © 2026
    تمامی حقوق محفوظ است.

</footer>


<!-- =====================================================
     JAVASCRIPT
===================================================== -->

<script>


/* =====================================================
   THEME
===================================================== */

function changeTheme(){

    document.body
        .classList
        .toggle("dark");


    const button =
        document.getElementById(
            "themeButton"
        );


    if(
        document.body
            .classList
            .contains("dark")
    ){

        button.innerHTML = "☀️";

        localStorage.setItem(
            "theme",
            "dark"
        );

    }else{

        button.innerHTML = "🌙";

        localStorage.setItem(
            "theme",
            "light"
        );

    }

}


/* =====================================================
   LOAD THEME
===================================================== */

if(
    localStorage.getItem("theme")
    !== "light"
){

    document.body
        .classList
        .add("dark");

    document
        .getElementById("themeButton")
        .innerHTML = "☀️";

}


/* =====================================================
   GO TO SHOWCASE
===================================================== */

function goProducts(){

    document
        .getElementById("showcase")
        .scrollIntoView({

            behavior:"smooth"

        });

}


/* =====================================================
   CALL SHOP
===================================================== */

function callShop(){

    window.location.href =
        "tel:09129582157";

}


/* =====================================================
   3D COVERFLOW
===================================================== */

(function(){

    const slider =
        document.getElementById(
            "coverflow"
        );


    if(!slider)
        return;


    const cards =
        [
            ...slider.querySelectorAll(
                ".coverflow-card"
            )
        ];


    const dotsBox =
        document.getElementById(
            "cfDots"
        );


    let index = 0;

    let startX = 0;

    let dragging = false;

    let autoTimer = null;

    let resumeTimer = null;


    /* =================================================
       DOTS
    ================================================= */

    cards.forEach(
        (_,i)=>{

            const dot =
                document.createElement(
                    "button"
                );


            dot.className =
                "cf-dot";


            dot.setAttribute(
                "aria-label",
                "محصول " + (i + 1)
            );


            dot.onclick = ()=>{

                index = i;

                render();

                restartAuto();

            };


            dotsBox.appendChild(
                dot
            );

        }
    );


    /* =================================================
       RENDER
    ================================================= */

    function render(){

        const total =
            cards.length;


        const mobile =
            window.innerWidth <= 700;


        cards.forEach(
            (card,i)=>{


                let distance =
                    i - index;


                if(
                    distance >
                    total / 2
                ){

                    distance -= total;

                }


                if(
                    distance <
                    -total / 2
                ){

                    distance += total;

                }


                const abs =
                    Math.abs(
                        distance
                    );


                const spread =
                    mobile
                        ? 155
                        : 230;


                const x =
                    distance *
                    spread;


                const z =
                    -abs *
                    (
                        mobile
                            ? 105
                            : 145
                    );


                const rotation =
                    distance * -38;


                const scale =
                    abs === 0

                        ? 1

                        : Math.max(
                            .67,
                            1 -
                            abs * .105
                        );


                card.style.transform =

                    `translate(-50%,-50%)
                     translateX(${x}px)
                     translateZ(${z}px)
                     rotateY(${rotation}deg)
                     scale(${scale})`;


                card.style.opacity =

                    abs > 2
                        ? "0"
                        : abs === 2
                            ? ".25"
                            : "1";


                card.style.filter =

                    abs === 0

                        ? "none"

                        : `
                            brightness(
                                ${abs === 1
                                    ? ".62"
                                    : ".40"}
                            )
                            saturate(
                                ${abs === 1
                                    ? ".78"
                                    : ".55"}
                            )
                        `;


                card.style.zIndex =
                    100 -
                    abs * 10;


                card.classList.toggle(
                    "active",
                    abs === 0
                );

            }
        );


        [
            ...dotsBox.children
        ].forEach(
            (dot,i)=>{

                dot.classList.toggle(
                    "active",
                    i === index
                );

            }
        );

    }


    /* =================================================
       NEXT
    ================================================= */

    function next(){

        index =
            (index + 1)
            % cards.length;

        render();

    }


    /* =================================================
       PREVIOUS
    ================================================= */

    function previous(){

        index =
            (
                index -
                1 +
                cards.length
            )
            % cards.length;

        render();

    }


    /* =================================================
       AUTO PLAY
    ================================================= */

    function stopAuto(){

        clearInterval(
            autoTimer
        );

        autoTimer = null;

    }


    function startAuto(){

        stopAuto();

        autoTimer =
            setInterval(
                next,
                3200
            );

    }


    function restartAuto(){

        stopAuto();

        clearTimeout(
            resumeTimer
        );

        resumeTimer =
            setTimeout(
                startAuto,
                1800
            );

    }


    /* =================================================
       BUTTONS
    ================================================= */

    document
        .getElementById("cfNext")
        .onclick = ()=>{

            next();

            restartAuto();

        };


    document
        .getElementById("cfPrev")
        .onclick = ()=>{

            previous();

            restartAuto();

        };


    /* =================================================
       CLICK CARDS
    ================================================= */

    cards.forEach(
        (card,i)=>{

            card.addEventListener(
                "click",
                ()=>{

                    if(
                        i !== index
                    ){

                        index = i;

                        render();

                        restartAuto();

                    }

                }
            );

        }
    );


    /* =================================================
       TOUCH / MOUSE DRAG
    ================================================= */

    slider.addEventListener(
        "pointerdown",
        e=>{

            dragging = true;

            startX =
                e.clientX;

            stopAuto();

            slider.setPointerCapture(
                e.pointerId
            );

        }
    );


    slider.addEventListener(
        "pointerup",
        e=>{

            if(!dragging)
                return;


            dragging = false;


            const movement =
                e.clientX -
                startX;


            if(
                Math.abs(
                    movement
                ) > 45
            ){

                if(
                    movement < 0
                ){

                    next();

                }else{

                    previous();

                }

            }


            restartAuto();

        }
    );


    slider.addEventListener(
        "pointercancel",
        ()=>{

            dragging = false;

            restartAuto();

        }
    );


    /* =================================================
       MOUSE HOVER
    ================================================= */

    slider.addEventListener(
        "mouseenter",
        stopAuto
    );


    slider.addEventListener(
        "mouseleave",
        ()=>{

            if(!dragging){

                startAuto();

            }

        }
    );


    /* =================================================
       KEYBOARD
    ================================================= */

    document.addEventListener(
        "keydown",
        e=>{

            if(
                e.key ===
                "ArrowLeft"
            ){

                next();

                restartAuto();

            }


            if(
                e.key ===
                "ArrowRight"
            ){

                previous();

                restartAuto();

            }

        }
    );


    /* =================================================
       RESPONSIVE
    ================================================= */

    window.addEventListener(
        "resize",
        render
    );


    /* =================================================
       START
    ================================================= */

    render();

    startAuto();

})();

</script>

</body>
</html>
