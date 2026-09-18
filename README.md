<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>SOMGOD Interiors | Luxury Interior & Electrical Design</title>

<meta name="description" content="SOMGOD Interiors creates refined interiors, premium electrical systems, lighting and property transformations for discerning clients and developers.">

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600&family=Playfair+Display:wght@400;500;600&display=swap" rel="stylesheet">

<style>

:root{
    --black:#080808;
    --black2:#111111;
    --gold:#D4AF37;
    --gold-light:#e8ce72;
    --cream:#f5f1e8;
    --muted:#aaa59b;
    --line:rgba(212,175,55,.22);
}

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    background:var(--black);
    color:white;
    font-family:"DM Sans",sans-serif;
    line-height:1.6;
}

a{
    color:inherit;
    text-decoration:none;
}

img{
    width:100%;
    display:block;
}

.container{
    width:min(1180px,90%);
    margin:auto;
}

/* ================= HEADER ================= */

header{
    position:fixed;
    top:0;
    left:0;
    width:100%;
    z-index:1000;
    padding:22px 0;
    background:linear-gradient(
        to bottom,
        rgba(0,0,0,.88),
        transparent
    );
}

.nav{
    display:flex;
    align-items:center;
    justify-content:space-between;
}

.logo{
    font-family:"Playfair Display",serif;
    letter-spacing:3px;
    font-size:20px;
}

.logo span{
    color:var(--gold);
}

nav{
    display:flex;
    gap:30px;
    align-items:center;
}

nav a{
    font-size:13px;
    color:#ddd;
    transition:.3s;
}

nav a:hover{
    color:var(--gold);
}

.nav-btn{
    border:1px solid var(--gold);
    padding:11px 18px;
    color:var(--gold);
    font-size:12px;
    letter-spacing:1px;
}

/* ================= HERO ================= */

.hero{
    min-height:100vh;
    position:relative;
    display:flex;
    align-items:center;
    overflow:hidden;

    background:
    linear-gradient(
        90deg,
        rgba(0,0,0,.88) 0%,
        rgba(0,0,0,.65) 45%,
        rgba(0,0,0,.25) 100%
    ),
    url("https://images.unsplash.com/photo-1600607687920-4e2a09cf159d?auto=format&fit=crop&w=2200&q=90")
    center/cover;
}

.hero::after{
    content:"";
    position:absolute;
    inset:0;
    background:linear-gradient(
        to top,
        var(--black),
        transparent 25%
    );
}

.hero-content{
    position:relative;
    z-index:2;
    max-width:800px;
}

.eyebrow{
    color:var(--gold);
    letter-spacing:4px;
    font-size:11px;
    margin-bottom:25px;
    text-transform:uppercase;
}

.hero h1{
    font-family:"Playfair Display",serif;
    font-size:clamp(48px,8vw,94px);
    line-height:.98;
    font-weight:400;
    margin-bottom:30px;
}

.hero h1 span{
    color:var(--gold);
}

.hero p{
    max-width:570px;
    color:#d1cec7;
    font-size:17px;
    margin-bottom:38px;
}

.buttons{
    display:flex;
    gap:14px;
    flex-wrap:wrap;
}

.btn{
    padding:15px 25px;
    font-size:12px;
    letter-spacing:1.5px;
    text-transform:uppercase;
    transition:.3s;
}

.btn-gold{
    background:var(--gold);
    color:#080808;
}

.btn-gold:hover{
    background:var(--gold-light);
    transform:translateY(-2px);
}

.btn-outline{
    border:1px solid rgba(255,255,255,.5);
}

.btn-outline:hover{
    border-color:var(--gold);
    color:var(--gold);
}

/* ================= INTRO ================= */

.intro{
    padding:120px 0;
    text-align:center;
    background:var(--black);
}

.intro .eyebrow{
    margin-bottom:18px;
}

.intro h2{
    font-family:"Playfair Display",serif;
    font-weight:400;
    font-size:clamp(35px,5vw,62px);
    max-width:850px;
    margin:auto;
}

.intro p{
    max-width:650px;
    margin:25px auto 0;
    color:var(--muted);
}

/* ================= SERVICES ================= */

.section{
    padding:110px 0;
}

.section-heading{
    margin-bottom:55px;
}

.section-heading h2{
    font-family:"Playfair Display",serif;
    font-size:clamp(38px,5vw,58px);
    font-weight:400;
}

.section-heading p{
    color:var(--muted);
    max-width:600px;
    margin-top:15px;
}

.services{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:1px;
    background:var(--line);
}

.service{
    background:var(--black);
    padding:42px 30px;
    min-height:270px;
    transition:.4s;
}

.service:hover{
    background:#121212;
    transform:translateY(-5px);
}

.service-number{
    color:var(--gold);
    font-size:12px;
    letter-spacing:2px;
}

.service h3{
    font-family:"Playfair Display",serif;
    font-size:27px;
    font-weight:400;
    margin:65px 0 15px;
}

.service p{
    color:var(--muted);
    font-size:14px;
}

/* ================= PROJECTS ================= */

.projects{
    display:grid;
    grid-template-columns:1.3fr .7fr;
    gap:18px;
}

.project{
    position:relative;
    min-height:520px;
    overflow:hidden;
    background:#111;
}

.project.small{
    min-height:251px;
}

.project-stack{
    display:grid;
    gap:18px;
}

.project img{
    height:100%;
    object-fit:cover;
    transition:transform .8s;
}

.project:hover img{
    transform:scale(1.05);
}

.project-overlay{
    position:absolute;
    inset:auto 0 0;
    padding:35px;
    background:linear-gradient(
        transparent,
        rgba(0,0,0,.9)
    );
}

.project-overlay small{
    color:var(--gold);
    letter-spacing:2px;
    text-transform:uppercase;
}

.project-overlay h3{
    font-family:"Playfair Display",serif;
    font-size:28px;
    font-weight:400;
    margin-top:8px;
}

/* ================= VALUE ================= */

.value{
    background:#101010;
}

.value-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:70px;
    align-items:center;
}

.value-image{
    min-height:550px;
    background:
    linear-gradient(rgba(0,0,0,.1),rgba(0,0,0,.1)),
    url("https://images.unsplash.com/photo-1600607688969-a5bfcd646154?auto=format&fit=crop&w=1400&q=90")
    center/cover;
}

.value-content h2{
    font-family:"Playfair Display",serif;
    font-size:clamp(40px,5vw,65px);
    font-weight:400;
    line-height:1.05;
}

.value-content h2 span{
    color:var(--gold);
}

.value-content > p{
    color:var(--muted);
    margin:25px 0 35px;
}

.features{
    display:grid;
    gap:22px;
}

.feature{
    border-top:1px solid var(--line);
    padding-top:18px;
}

.feature h4{
    font-family:"Playfair Display",serif;
    font-size:20px;
    font-weight:400;
}

.feature p{
    color:var(--muted);
    font-size:13px;
    margin-top:5px;
}

/* ================= PARTNERS ================= */

.partners{
    text-align:center;
    padding:120px 0;
}

.partners h2{
    font-family:"Playfair Display",serif;
    font-size:clamp(40px,6vw,70px);
    font-weight:400;
    max-width:850px;
    margin:auto;
}

.partners h2 span{
    color:var(--gold);
}

.partners p{
    color:var(--muted);
    max-width:650px;
    margin:25px auto 50px;
}

.partner-list{
    display:flex;
    justify-content:center;
    flex-wrap:wrap;
    gap:12px;
}

.partner-list span{
    border:1px solid var(--line);
    padding:14px 20px;
    font-size:12px;
    letter-spacing:1px;
}

/* ================= PROCESS ================= */

.process-grid{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    border-top:1px solid var(--line);
}

.process{
    padding:35px 25px;
    border-right:1px solid var(--line);
}

.process:last-child{
    border-right:none;
}

.process-number{
    color:var(--gold);
    font-size:12px;
}

.process h3{
    font-family:"Playfair Display",serif;
    font-size:25px;
    font-weight:400;
    margin:40px 0 10px;
}

.process p{
    color:var(--muted);
    font-size:13px;
}

/* ================= CTA ================= */

.cta{
    padding:130px 0;
    text-align:center;
    background:
    linear-gradient(
        rgba(0,0,0,.78),
        rgba(0,0,0,.9)
    ),
    url("https://images.unsplash.com/photo-1600607687939-ce8a6c25118c?auto=format&fit=crop&w=2000&q=90")
    center/cover;
}

.cta h2{
    font-family:"Playfair Display",serif;
    font-size:clamp(42px,7vw,78px);
    font-weight:400;
    line-height:1;
    max-width:850px;
    margin:0 auto 25px;
}

.cta p{
    color:#ccc;
    max-width:550px;
    margin:0 auto 35px;
}

/* ================= CONTACT ================= */

.contact-grid{
    display:grid;
    grid-template-columns:.8fr 1.2fr;
    gap:80px;
}

.contact-info h2{
    font-family:"Playfair Display",serif;
    font-size:55px;
    font-weight:400;
    line-height:1;
}

.contact-info p{
    color:var(--muted);
    margin:25px 0;
}

.contact-link{
    color:var(--gold);
    display:block;
    margin-top:12px;
}

form{
    display:grid;
    gap:15px;
}

input,
textarea,
select{
    width:100%;
    background:#111;
    border:1px solid #292929;
    color:white;
    padding:16px;
    font-family:inherit;
    outline:none;
}

input:focus,
textarea:focus,
select:focus{
    border-color:var(--gold);
}

textarea{
    min-height:140px;
    resize:vertical;
}

select{
    appearance:auto;
}

form button{
    border:none;
    cursor:pointer;
}

/* ================= FOOTER ================= */

footer{
    border-top:1px solid #222;
    padding:35px 0;
}

.footer{
    display:flex;
    justify-content:space-between;
    gap:20px;
    color:#777;
    font-size:12px;
}

.footer strong{
    color:white;
    font-family:"Playfair Display",serif;
    letter-spacing:2px;
}

/* ================= WHATSAPP ================= */

.whatsapp{
    position:fixed;
    right:22px;
    bottom:22px;
    z-index:999;
    width:58px;
    height:58px;
    border-radius:50%;
    background:#25D366;
    color:white;
    display:flex;
    align-items:center;
    justify-content:center;
    font-size:23px;
    box-shadow:0 8px 30px rgba(0,0,0,.4);
}

/* ================= MOBILE ================= */

@media(max-width:850px){

    nav{
        display:none;
    }

    .hero{
        min-height:90vh;
    }

    .hero h1{
        font-size:55px;
    }

    .services{
        grid-template-columns:1fr 1fr;
    }

    .projects{
        grid-template-columns:1fr;
    }

    .project{
        min-height:400px;
    }

    .value-grid,
    .contact-grid{
        grid-template-columns:1fr;
    }

    .value-image{
        min-height:420px;
    }

    .process-grid{
        grid-template-columns:1fr 1fr;
    }

    .process{
        border-bottom:1px solid var(--line);
    }

}

@media(max-width:550px){

    .container{
        width:88%;
    }

    .logo{
        font-size:16px;
    }

    .nav-btn{
        padding:9px 12px;
        font-size:10px;
    }

    .hero h1{
        font-size:48px;
    }

    .hero p{
        font-size:15px;
    }

    .section{
        padding:80px 0;
    }

    .services{
        grid-template-columns:1fr;
    }

    .service{
        min-height:230px;
    }

    .project{
        min-height:350px;
    }

    .project.small{
        min-height:350px;
    }

    .process-grid{
        grid-template-columns:1fr;
    }

    .process{
        border-right:none;
    }

    .footer{
        flex-direction:column;
    }

    .contact-info h2{
        font-size:45px;
    }

}

</style>
</head>

<body>

<!-- HEADER -->

<header>

<div class="container nav">

<a href="#" class="logo">
SOMGOD <span>INTERIORS</span>
</a>

<nav>
<a href="#services">Services</a>
<a href="#projects">Projects</a>
<a href="#process">Process</a>
<a href="#contact">Contact</a>
</nav>

<a href="#contact" class="nav-btn">
PRIVATE CONSULTATION
</a>

</div>

</header>


<!-- HERO -->

<section class="hero">

<div class="container">

<div class="hero-content">

<div class="eyebrow">
Luxury Interior • Electrical • Lighting
</div>

<h1>
Luxury Designed.<br>
<span>Beautifully Built.</span>
</h1>

<p>
We create refined interiors, architectural lighting and precision electrical systems for exceptional homes, commercial spaces and property developments.
</p>

<div class="buttons">

<a href="#projects" class="btn btn-gold">
View Our Work
</a>

<a href="#contact" class="btn btn-outline">
Private Consultation
</a>

</div>

</div>

</div>

</section>


<!-- INTRO -->

<section class="intro">

<div class="container">

<div class="eyebrow">
SOMGOD INTERIORS
</div>

<h2>
Where refined design meets precision execution.
</h2>

<p>
From concept to completion, we transform spaces into sophisticated environments designed around comfort, character, functionality and lasting value.
</p>

</div>

</section>


<!-- SERVICES -->

<section class="section" id="services">

<div class="container">

<div class="section-heading">

<div class="eyebrow">
What We Do
</div>

<h2>
Designed for distinction.
</h2>

<p>
A complete design and finishing approach for clients who expect more from their spaces.
</p>

</div>

<div class="services">

<div class="service">

<div class="service-number">01</div>

<h3>Interior Design</h3>

<p>
Bespoke residential and commercial interiors with carefully considered materials, proportions, furniture and finishes.
</p>

</div>


<div class="service">

<div class="service-number">02</div>

<h3>Electrical & Lighting</h3>

<p>
Professional electrical systems and architectural lighting designed to combine safety, functionality and visual impact.
</p>

</div>


<div class="service">

<div class="service-number">03</div>

<h3>Painting & Finishes</h3>

<p>
Premium surface finishes and colour systems that give every environment a refined final character.
</p>

</div>


<div class="service">

<div class="service-number">04</div>

<h3>Property Transformation</h3>

<p>
End-to-end improvement of homes and properties through coordinated design, finishing and technical execution.
</p>

</div>

</div>

</div>

</section>


<!-- PROJECTS -->

<section class="section" id="projects">

<div class="container">

<div class="section-heading">

<div class="eyebrow">
Selected Spaces
</div>

<h2>
A glimpse into the vision.
</h2>

<p>
Every project begins with a vision and ends with a space designed to be experienced.
</p>

</div>


<div class="projects">

<div class="project">

<img
src="https://images.unsplash.com/photo-1600210492486-724fe5c67fb0?auto=format&fit=crop&w=1600&q=90"
alt="Luxury contemporary interior">

<div class="project-overlay">

<small>Residential</small>

<h3>
Contemporary Luxury Residence
</h3>

</div>

</div>


<div class="project-stack">

<div class="project small">

<img
src="https://images.unsplash.com/photo-1616486338812-3dadae4b4ace?auto=format&fit=crop&w=1200&q=90"
alt="Luxury living space">

<div class="project-overlay">

<small>Residential</small>

<h3>
Executive Living
</h3>

</div>

</div>


<div class="project small">

<img
src="https://images.unsplash.com/photo-1600566753086-00f18fb6b3ea?auto=format&fit=crop&w=1200&q=90"
alt="Architectural lighting">

<div class="project-overlay">

<small>Lighting</small>

<h3>
Architectural Illumination
</h3>

</div>

</div>

</div>

</div>

</div>

</section>


<!-- VALUE -->

<section class="section value">

<div class="container">

<div class="value-grid">

<div class="value-image"></div>


<div class="value-content">

<div class="eyebrow">
The SOMGOD Standard
</div>

<h2>
Design that creates <span>value.</span>
</h2>

<p>
We approach every project as both a design opportunity and a long-term property investment. The goal is not simply to make a space beautiful, but to make it memorable, functional and valuable.
</p>


<div class="features">

<div class="feature">

<h4>Bespoke Design</h4>

<p>
Every project is developed around the client's vision, property and lifestyle.
</p>

</div>


<div class="feature">

<h4>Precision Execution</h4>

<p>
Design intent is carried through into the technical and finishing details.
</p>

</div>


<div class="feature">

<h4>Premium Experience</h4>

<p>
A carefully managed journey from initial consultation through final reveal.
</p>

</div>

</div>

</div>

</div>

</div>

</section>


<!-- PARTNERS -->

<section class="partners">

<div class="container">

<div class="eyebrow">
For Property Owners & Developers
</div>

<h2>
Build properties people <span>want to own.</span>
</h2>

<p>
We collaborate with property owners, developers and businesses to create spaces that communicate quality from the moment someone walks through the door.
</p>


<div class="partner-list">

<span>Luxury Property Owners</span>
<span>Real Estate Developers</span>
<span>Residential Projects</span>
<span>Commercial Projects</span>
<span>Hospitality Spaces</span>

</div>

</div>

</section>


<!-- PROCESS -->

<section class="section" id="process">

<div class="container">

<div class="section-heading">

<div class="eyebrow">
Our Process
</div>

<h2>
From vision to reality.
</h2>

</div>


<div class="process-grid">

<div class="process">

<div class="process-number">01</div>

<h3>Discover</h3>

<p>
We understand the property, objectives, lifestyle and desired outcome.
</p>

</div>


<div class="process">

<div class="process-number">02</div>

<h3>Design</h3>

<p>
We develop the creative direction, materials, lighting and spatial concept.
</p>

</div>


<div class="process">

<div class="process-number">03</div>

<h3>Execute</h3>

<p>
Our design moves into coordinated technical and finishing execution.
</p>

</div>


<div class="process">

<div class="process-number">04</div>

<h3>Reveal</h3>

<p>
The completed environment is delivered with attention to the final details.
</p>

</div>

</div>

</div>

</section>


<!-- CTA -->

<section class="cta">

<div class="container">

<div class="eyebrow">
Your Space. Our Craft.
</div>

<h2>
Let's create something exceptional.
</h2>

<p>
Tell us about your project and let's explore what is possible.
</p>

<a href="#contact" class="btn btn-gold">
Start Your Project
</a>

</div>

</section>


<!-- CONTACT -->

<section class="section" id="contact">

<div class="container">

<div class="contact-grid">

<div class="contact-info">

<div class="eyebrow">
Private Consultation
</div>

<h2>
Let's talk about your project.
</h2>

<p>
For residential, commercial, electrical, lighting or complete property transformation projects, contact SOMGOD Interiors.
</p>

<a class="contact-link" href="tel:+2349063922073">
+234 906 392 2073
</a>

<a class="contact-link" href="https://wa.me/2349063922073">
WhatsApp Consultation →
</a>

</div>


<form action="https://formsubmit.co/09063922073" method="POST">

<input
type="hidden"
name="_subject"
value="New SOMGOD Interiors Project Enquiry">

<input
type="hidden"
name="_captcha"
value="false">

<input
type="hidden"
name="_template"
value="table">


<input
type="text"
name="name"
placeholder="Full Name"
required>


<input
type="tel"
name="phone"
placeholder="Phone / WhatsApp"
required>


<input
type="email"
name="email"
placeholder="Email Address">


<select name="project">

<option value="">Project Type</option>
<option>Interior Design</option>
<option>Electrical & Lighting</option>
<option>Painting & Finishes</option>
<option>Property Transformation</option>
<option>Commercial Project</option>
<option>Other</option>

</select>


<textarea
name="message"
placeholder="Tell us about your project..."
required></textarea>


<button
type="submit"
class="btn btn-gold">

Request Consultation

</button>

</form>

</div>

</div>

</section>


<!-- FOOTER -->

<footer>

<div class="container footer">

<div>
<strong>SOMGOD INTERIORS</strong>
</div>

<div>
© 2026 SOMGOD Interiors. All rights reserved.
</div>

<div>
Luxury Designed. Beautifully Built.
</div>

</div>

</footer>


<!-- WHATSAPP -->

<a
class="whatsapp"
href="https://wa.me/2349063922073"
aria-label="Chat with SOMGOD Interiors on WhatsApp">

WA

</a>


</body>
</html>
