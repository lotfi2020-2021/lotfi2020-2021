
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no"/>
<title>Lotfi Hmida | Full Stack Java/Angular Engineer</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&family=Montserrat:wght@800&family=Raleway:wght@300;400;500;600;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css" />
<style>
:root {
--primary: #2563eb;
--primary-light: #3b82f6;
--secondary: #1e40af;
--accent: #8b5cf6;
--accent2: #ec4899;
--light: #f8fafc;
--dark: #0f172a;
--gray: #64748b;
--light-gray: #e2e8f0;
--success: #10b981;
--warning: #f59e0b;
--danger: #ef4444;
--card-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1), 0 8px 10px -6px rgba(0, 0, 0, 0.1);
--transition: all 0.3s ease;
--github-color: #181717;
--linkedin-color: #0a66c2;
--facebook-color: #1877f2;
--instagram-color: #e1306c;
--gmail-color: #ea4335;
--location-color: #4285f4;
--phone-color: #34a853;
--whatsapp-color: #25D366;
}
* {
margin: 0;
padding: 0;
box-sizing: border-box;
}
body {
font-family: 'Poppins', sans-serif;
background: linear-gradient(135deg, #f0f9ff 0%, #e0f2fe 100%);
color: var(--dark);
line-height: 1.6;
overflow-x: hidden;
position: relative;
transition: background 0.35s ease, color 0.35s ease;
}
body::before {
content: '';
position: fixed;
top: 0;
left: 0;
width: 100%;
height: 100%;
background: radial-gradient(circle at 10% 20%, rgba(37, 99, 235, 0.05) 0%, rgba(255, 255, 255, 0) 25%);
z-index: -1;
}
.container {
max-width: 1200px;
margin: 0 auto;
padding: 0 24px;
}
/* Section styling with improved transitions */
section {
padding: 100px 0;
position: relative;
overflow: hidden;
}
/* Section header styling for consistency */
.section-title {
text-align: center;
position: relative;
margin-bottom: 20px;
font-family: 'Montserrat', sans-serif;
font-size: 36px;
font-weight: 800;
color: var(--secondary);
}
.section-title::after {
content: '';
position: absolute;
bottom: -10px;
left: 50%;
transform: translateX(-50%);
width: 80px;
height: 4px;
background: linear-gradient(90deg, var(--primary), var(--accent));
border-radius: 2px;
}
.section-description {
text-align: center;
margin: 25px auto 0;
max-width: 700px;
color: var(--gray);
font-size: 18px;
line-height: 1.7;
}
/* Section dividers */
.section-divider {
height: 60px;
position: relative;
display: flex;
align-items: center;
justify-content: center;
}
.section-divider::before {
content: '';
position: absolute;
width: 150px;
height: 150px;
border-radius: 50%;
background: linear-gradient(135deg, rgba(37, 99, 235, 0.1), rgba(139, 92, 246, 0.1));
z-index: -1;
animation: pulseDivider 3s infinite alternate;
}
@keyframes pulseDivider {
0% { transform: scale(0.95); opacity: 0.3; }
100% { transform: scale(1.05); opacity: 0.5; }
}
.divider-icon {
font-size: 24px;
color: var(--primary);
background: rgba(37, 99, 235, 0.1);
width: 60px;
height: 60px;
border-radius: 50%;
display: flex;
align-items: center;
justify-content: center;
box-shadow: 0 4px 10px rgba(0, 0, 0, 0.05);
animation: floating 3s ease-in-out infinite;
}
/* Navbar - Enhanced animations */
nav {
position: fixed;
top: 0;
left: 0;
width: 100%;
background: rgba(255, 255, 255, 0.95);
-webkit-backdrop-filter: blur(10px);
backdrop-filter: blur(10px);
z-index: 1000;
padding: 16px 0;
transition: var(--transition);
transform: translateY(0);
box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
}
nav.scrolled {
padding: 12px 0;
background: rgba(255, 255, 255, 0.98);
box-shadow: 0 4px 20px rgba(0, 0, 0, 0.08);
}
nav.hidden {
transform: translateY(-100%);
transition: transform 0.3s ease, background 0.3s ease, box-shadow 0.3s ease;
}
.nav-container {
display: flex;
justify-content: space-between;
align-items: center;
padding: 0 24px;
}
.nav-logo {
font-family: 'Montserrat', sans-serif;
font-size: 24px;
font-weight: 800;
color: var(--primary);
text-decoration: none;
display: flex;
align-items: center;
gap: 8px;
transition: font-size 0.3s ease;
}
nav.scrolled .nav-logo {
font-size: 22px;
}
.nav-logo span {
color: var(--secondary);
}
.nav-links {
display: flex;
gap: 32px;
}
.nav-links a {
color: var(--dark);
text-decoration: none;
font-weight: 500;
transition: var(--transition);
position: relative;
font-size: 16px;
padding: 5px 0;
}
.nav-links a.active,
.nav-links a:hover {
color: var(--primary);
}
.nav-links a::after {
content: '';
position: absolute;
bottom: 0;
left: 0;
width: 0;
height: 2px;
background: var(--primary);
transition: var(--transition);
}
.nav-links a.active::after,
.nav-links a:hover::after {
width: 100%;
}
.mobile-toggle {
display: none;
background: none;
border: none;
font-size: 24px;
color: var(--primary);
cursor: pointer;
padding: 8px;
}
.nav-actions {
display: flex;
align-items: center;
gap: 10px;
}
.theme-toggle {
display: inline-flex;
align-items: center;
gap: 8px;
padding: 8px 14px;
border-radius: 999px;
border: 1px solid rgba(37, 99, 235, 0.25);
background: rgba(37, 99, 235, 0.08);
color: var(--secondary);
font-family: 'Poppins', sans-serif;
font-size: 14px;
font-weight: 600;
cursor: pointer;
transition: var(--transition);
}
.theme-toggle:hover {
background: rgba(37, 99, 235, 0.16);
transform: translateY(-1px);
}
.theme-toggle i {
font-size: 16px;
}
.mobile-theme-toggle {
display: none;
width: calc(100% - 32px);
margin: 10px 16px 0;
padding: 10px 14px;
border-radius: 12px;
border: 1px solid rgba(37, 99, 235, 0.25);
background: rgba(37, 99, 235, 0.08);
color: var(--secondary);
font-family: 'Poppins', sans-serif;
font-size: 14px;
font-weight: 600;
cursor: pointer;
text-align: left;
transition: var(--transition);
}
.mobile-theme-toggle:hover {
background: rgba(37, 99, 235, 0.16);
}
/* NEW HERO SECTION WITH STUNNING ANIMATIONS */
#hero {
min-height: 100vh;
display: flex;
align-items: center;
padding-top: 80px;
position: relative;
overflow: hidden;
background: linear-gradient(40deg, #01183a 0%, #010c1c 52%, #001027 100%);
color: var(--light);
text-align: center;
}
.starry-background {
position: absolute;
top: 0;
left: 0;
width: 100%;
height: 100%;
z-index: 0;
}
.starry-background::before {
content: '';
position: absolute;
width: 200%;
height: 200%;
background: radial-gradient(circle, rgba(255,255,255,0.1) 1px, transparent 1px);
background-size: 50px 50px;
animation: rotateStars 200s linear infinite;
}
.starry-background::after {
content: '';
position: absolute;
top: 0;
left: 0;
width: 100%;
height: 100%;
background: radial-gradient(ellipse at center, rgba(147, 197, 253, 0.1) 0%, rgba(99, 102, 241, 0.04) 50%, rgba(99, 102, 241, 0) 78%);
z-index: 0;
}
.network-canvas {
position: absolute;
inset: 0;
width: 100%;
height: 100%;
z-index: 1;
opacity: 0.78;
pointer-events: none;
}
@keyframes rotateStars {
from { transform: rotate(0deg); }
to { transform: rotate(360deg); }
}
.comet {
position: absolute;
height: 2px;
background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.8), transparent);
border-radius: 50%;
animation: comet linear infinite;
animation-duration: calc(15s + var(--duration));
animation-delay: var(--delay);
}
@keyframes comet {
0% { transform: translate(var(--start-x), var(--start-y)) rotate(0deg) scale(0); opacity: 0; }
20% { opacity: 1; }
80% { opacity: 1; }
100% { transform: translate(var(--end-x), var(--end-y)) rotate(0deg) scale(1); opacity: 0; }
}
.nebula {
position: absolute;
width: 500px;
height: 500px;
border-radius: 50%;
background: radial-gradient(circle, rgba(125, 211, 252, 0.08), transparent 70%);
z-index: 0;
animation: float 15s ease-in-out infinite;
}
.nebula:nth-child(2) {
width: 700px;
height: 700px;
background: radial-gradient(circle, rgba(56, 189, 248, 0.07), transparent 70%);
left: 20%;
top: 40%;
animation-delay: -5s;
}
.nebula:nth-child(3) {
width: 400px;
height: 400px;
background: radial-gradient(circle, rgba(165, 180, 252, 0.08), transparent 70%);
right: 10%;
top: 30%;
animation-delay: -10s;
}
@keyframes float {
0%, 100% { transform: translate(0, 0) scale(1); }
50% { transform: translate(10px, 15px) scale(1.05); }
}
.content-wrapper {
position: relative;
z-index: 2;
width: 100%;
padding-top: 2px;
}
.hero-content {
display: flex;
flex-direction: row;
align-items: center;
justify-content: center;
gap: 56px;
max-width: 1180px;
margin: 0 auto;
padding: 20px;
}
/* Profile image centered at top */
.profile-wrapper-centered {
flex: 0 0 320px;
display: flex;
flex-direction: column;
align-items: center;
justify-content: center;
margin-bottom: 0;
animation: fadeInUp 1s ease forwards 0.2s;
}
.profile-container-centered {
position: relative;
width: 280px;
height: 280px;
}
.profile-border-centered {
position: absolute;
width: 100%;
height: 100%;
border-radius: 50%;
background: linear-gradient(45deg, #1d4ed8, #3b82f6, #6366f1);
top: 0;
left: 0;
z-index: 1;
animation: rotate 12s linear infinite;
box-shadow: 0 0 18px rgba(37, 99, 235, 0.35);
}
.profile-border-centered::before {
content: '';
position: absolute;
top: 2px;
left: 2px;
right: 2px;
bottom: 2px;
background: linear-gradient(135deg, rgba(15, 23, 42, 0.9), rgba(30, 41, 59, 0.95));
border-radius: 50%;
z-index: -1;
}
.profile-border-centered::after {
content: '';
position: absolute;
top: -5px;
left: -5px;
right: -5px;
bottom: -5px;
background: linear-gradient(45deg, transparent, rgba(59, 130, 246, 0.2), transparent);
border-radius: 50%;
z-index: -1;
filter: blur(10px);
animation: pulse 3s infinite alternate;
}
.profile-img-centered {
position: absolute;
width: 270px;
height: 270px;
border-radius: 50%;
object-fit: cover;
border: 2px solid rgba(37, 99, 235, 0.32);
top: 5px;
left: 5px;
z-index: 2;
transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
box-shadow: 0 8px 18px rgba(15, 23, 42, 0.26);
background-size: cover;
background-position: center;
transform-style: preserve-3d;
animation: float 6s ease-in-out infinite;
cursor: zoom-in;
}
.profile-img-centered:hover {
transform: scale(1.07) rotateY(15deg) rotateX(5deg);
box-shadow: 0 12px 26px rgba(37, 99, 235, 0.38);
}
.profile-img-centered:focus-visible {
outline: 3px solid rgba(96, 165, 250, 0.9);
outline-offset: 5px;
}
body.no-scroll {
overflow: hidden;
}
.image-zoom-overlay {
position: fixed;
inset: 0;
display: flex;
align-items: center;
justify-content: center;
padding: 24px;
background: rgba(2, 6, 23, 0.8);
z-index: 2200;
opacity: 0;
visibility: hidden;
pointer-events: none;
transition: opacity 0.25s ease, visibility 0.25s ease;
}
.image-zoom-overlay.open {
opacity: 1;
visibility: visible;
pointer-events: auto;
}
.image-zoom-content {
width: auto;
height: auto;
max-width: 92vw;
max-height: 92vh;
object-fit: cover;
border-radius: 50%;
border: 4px solid rgba(255, 255, 255, 0.85);
box-shadow: 0 28px 60px rgba(15, 23, 42, 0.55);
transform: scale(0.88);
transition: transform 0.25s ease;
}
.image-zoom-overlay.open .image-zoom-content {
transform: scale(1);
}
.hero-text-centered {
flex: 1;
max-width: 760px;
animation: fadeInUp 1s ease forwards 0.6s;
}
.hero-text-centered h1 {
font-family: 'Montserrat', sans-serif;
font-size: 46px;
font-weight: 800;
margin-bottom: 20px;
line-height: 1.2;
position: relative;
text-shadow: 0 2px 20px rgba(0, 0, 0, 0.3);
}
.hero-text-centered h1 span {
display: inline-flex;
opacity: 2;
animation: slideIn 0.5s forwards;
}
.hero-text-centered h1 span:nth-child(1) { animation-delay: 0.1s; }
.hero-text-centered h1 span:nth-child(2) { animation-delay: 0.2s; }
.hero-text-centered h1 span:nth-child(3) { animation-delay: 0.3s; }
.hero-text-centered h1 span:nth-child(4) { animation-delay: 0.4s; }
.hero-text-centered h1 span:nth-child(5) { animation-delay: 0.5s; }
.hero-text-centered h1 span:nth-child(6) { animation-delay: 0.6s; }
.hero-text-centered h1 span:nth-child(7) { animation-delay: 0.7s; }
.hero-text-centered h1 span:nth-child(8) { animation-delay: 0.8s; }
.hero-text-centered h1 span:nth-child(9) { animation-delay: 0.9s; }
.hero-text-centered h1 span:nth-child(10) { animation-delay: 1.0s; }
@keyframes slideIn {
0% { transform: translateY(30px); opacity: 0; }
70% { transform: translateY(-5px); opacity: 1; }
100% { transform: translateY(0); opacity: 1; }
}
.typewriter-container {
margin: 20px 0 35px;
position: relative;
}
.typewriter-container::before {
content: '';
position: absolute;
top: 50%;
left: 0;
width: 100%;
height: 2px;
background: linear-gradient(90deg, transparent, transparent, transparent);
transform: translateY(-30%);
}
.typewriter {
font-size: 26px;
color: var(--location-color);;
margin-bottom: 30px;
font-weight: 700;
white-space: normal;
word-break: break-word;
overflow: hidden;
width: 38ch;
animation: pulse 3.5s steps(38) infinite, blink 0.75s step-end infinite;
margin: 0 auto;
display: inline-block;
}
@keyframes typing {
0%, 50% { width: 0; }
60%, 100% { width: 31ch; }
}
@keyframes blink {
100% { border-color: transparent; }
}
.summary-box {
background: rgba(255, 255, 255, 0.08);
-webkit-backdrop-filter: blur(10px);
backdrop-filter: blur(10px);
padding: 32px;
border-radius: 24px;
margin: 30px 0;
border: 1px solid rgba(255, 255, 255, 0.1);
box-shadow: 0 8px 32px rgba(0, 0, 0, 0.2);
transition: var(--transition);
position: relative;
overflow: hidden;
animation: fadeInUp 1s ease forwards 1s;
}
.summary-box::before {
content: '';
position: absolute;
top: -50%;
left: -50%;
width: 200%;
height: 200%;
background: linear-gradient(45deg, transparent, rgba(255, 255, 255, 0.1), transparent);
transform: rotate(30deg);
animation: shimmer 3s infinite;
}
@keyframes shimmer {
0% { transform: rotate(30deg) translateX(-100%); }
100% { transform: rotate(30deg) translateX(100%); }
}
.summary-box:hover {
transform: translateY(-8px);
box-shadow: 0 15px 40px rgba(0, 0, 0, 0.3);
}
.summary-box p {
font-size: 18px;
line-height: 1.8;
color: rgba(255, 255, 255, 0.9);
}
.contact-info {
display: flex;
flex-wrap: nowrap;
justify-content: center;
gap: 14px;
margin: 30px 0;
}
.contact-item {
display: flex;
align-items: center;
gap: 12px;
color: rgba(255, 255, 255, 0.85);
font-weight: 500;
font-size: 15px;
transition: var(--transition);
padding: 8px 12px;
border-radius: 12px;
animation: fadeInUp 1s ease forwards 1.2s;
background: rgba(255, 255, 255, 0.08);
border: 1px solid rgba(255, 255, 255, 0.1);
white-space: nowrap;
}
.contact-item:hover {
background: rgba(37, 99, 235, 0.3);
color: white;
transform: translateX(5px);
}
.contact-item i {
font-size: 20px;
width: 28px;
height: 28px;
display: flex;
align-items: center;
justify-content: center;
border-radius: 8px;
background: rgba(255, 255, 255, 0.15);
}
.contact-item.email i {
color: var(--gmail-color);
}
.contact-item.phone i {
color: var(--phone-color);
}
.contact-item.location i {
color: var(--location-color);
}
.contact-item.whatsapp i {
color: var(--whatsapp-color);
}
.socials {
display: flex;
gap: 18px;
margin: 25px 0;
flex-wrap: wrap;
animation: fadeInUp 1s ease forwards 1.4s;
justify-content: center;
}
.social-link {
width: 60px;
height: 60px;
border-radius: 20px;
background: rgba(255, 255, 255, 0.08);
backdrop-filter: blur(5px);
-webkit-backdrop-filter: blur(5px);
display: flex;
align-items: center;
justify-content: center;
color: white;
font-size: 24px;
transition: var(--transition);
border: 1px solid rgba(255, 255, 255, 0.1);
box-shadow: 0 4px 15px rgba(0, 0, 0, 0.15);
position: relative;
overflow: hidden;
}
.social-link::before {
content: '';
position: absolute;
top: 0;
left: 0;
width: 100%;
height: 100%;
background: linear-gradient(45deg, var(--primary), var(--accent));
opacity: 0;
transition: var(--transition);
z-index: 1;
}
.social-link.whatsapp::before {
background: linear-gradient(45deg, var(--whatsapp-color), #128C7E);
}
.social-link i {
position: relative;
z-index: 2;
transition: var(--transition);
}
.social-link:hover {
transform: translateY(-8px) rotate(8deg);
box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
}
.social-link:hover::before {
opacity: 1;
}
.social-link:hover i {
color: white;
}
.btn {
display: inline-block;
background: linear-gradient(90deg, var(--primary), var(--secondary));
color: white;
padding: 16px 40px;
border-radius: 50px;
text-decoration: none;
font-weight: 600;
margin-top: 16px;
transition: var(--transition);
border: none;
cursor: pointer;
font-size: 17px;
position: relative;
overflow: hidden;
animation: fadeInUp 1s ease forwards 1.6s;
box-shadow: 0 5px 20px rgba(37, 99, 235, 0.4);
}
.btn::before {
content: '';
position: absolute;
top: 0;
left: -100%;
width: 100%;
height: 100%;
background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
transition: var(--transition);
}
.btn:hover {
transform: translateY(-4px) scale(1.05);
box-shadow: 0 8px 30px rgba(37, 99, 235, 0.6);
}
.btn:hover::before {
left: 100%;
}
.btn-outline {
background: transparent;
border: 2px solid rgba(255, 255, 255, 0.5);
color: white;
margin-left: 15px;
transition: all 0.4s ease;
}
.hero-buttons {
display: flex;
gap: 15px;
flex-wrap: wrap;
justify-content: center;
margin-top: 20px;
}
.profile-wrapper-centered .hero-buttons {
margin-top: 28px;
}
.profile-wrapper-centered .hero-buttons .btn {
width: 220px;
display: inline-flex;
align-items: center;
justify-content: center;
}
.profile-wrapper-centered .hero-buttons .btn-outline {
margin-left: 0;
}
/* Experience timeline */
#experience {
background-color: #f8fafc;
position: relative;
padding: 100px 0;
}
.experience-container {
max-width: 1200px;
margin: 0 auto;
padding: 0 20px;
}
.experience-grid {
position: relative;
display: flex;
flex-direction: column;
gap: 20px;
margin-top: 45px;
padding: 8px 0;
}
.company-group {
background: rgba(255, 255, 255, 0.94);
border-radius: 18px;
box-shadow: 0 14px 28px -20px rgba(15, 23, 42, 0.35);
border: 1px solid rgba(37, 99, 235, 0.16);
overflow: hidden;
}
.wind-group .company-header {
display: none;
}
.company-summary {
list-style: none;
cursor: pointer;
display: flex;
align-items: center;
justify-content: space-between;
gap: 16px;
padding: 20px 24px;
background: linear-gradient(90deg, rgba(37, 99, 235, 0.08), rgba(139, 92, 246, 0.06));
border-bottom: 1px solid rgba(148, 163, 184, 0.25);
}
.company-summary::-webkit-details-marker {
display: none;
}
.company-summary-info {
display: flex;
align-items: center;
gap: 12px;
}
.company-summary-text h3 {
font-size: 22px;
line-height: 1.2;
color: var(--secondary);
}
.company-summary-text p {
margin-top: 2px;
font-size: 14px;
color: var(--gray);
}
.company-toggle-icon {
font-size: 18px;
color: var(--primary);
transition: transform 0.25s ease;
}
.company-group[open] .company-toggle-icon {
transform: rotate(180deg);
}
.company-jobs {
display: flex;
flex-direction: column;
gap: 14px;
padding: 16px 16px 16px 54px;
position: relative;
}
.company-jobs::before {
content: '';
position: absolute;
top: 10px;
bottom: 32px;
left: 22px;
width: 4px;
background: linear-gradient(180deg, rgba(37, 99, 235, 0.18), rgba(139, 92, 246, 0.28));
border-radius: 999px;
}
/* Company header styles */
.company-header {
display: flex;
align-items: center;
margin-bottom: 20px;
gap: 15px;
}
.company-logo {
width: 60px;
height: 60px;
border-radius: 16px;
background: linear-gradient(135deg, var(--primary), var(--accent));
display: flex;
align-items: center;
justify-content: center;
color: white;
font-weight: bold;
font-size: 24px;
flex-shrink: 0;
}
/* Experience card styles */
.experience-card {
background: rgba(255, 255, 255, 0.98);
border-radius: 16px;
overflow: visible;
box-shadow: 0 10px 24px -18px rgba(15, 23, 42, 0.42);
transition: var(--transition);
position: relative;
display: flex;
flex-direction: column;
width: 100%;
border: 1px solid rgba(37, 99, 235, 0.16);
}
.company-jobs .experience-card::before {
content: '';
position: absolute;
top: 28px;
width: 12px;
height: 12px;
border-radius: 50%;
background: #fff;
border: 3px solid var(--primary);
box-shadow: 0 0 0 4px rgba(37, 99, 235, 0.1);
z-index: 2;
}
.company-jobs .experience-card::before {
left: -39px;
}
.experience-card.current {
border-color: rgba(139, 92, 246, 0.45);
}
.experience-card.current::before {
border-color: var(--accent);
box-shadow: 0 0 0 4px rgba(139, 92, 246, 0.18);
}
.wind-group .card-header {
padding: 25px;
}
.wind-group .experience-date {
margin-bottom: 0;
}
.experience-card:hover {
transform: translateY(-3px);
box-shadow: 0 16px 30px -16px rgba(15, 23, 42, 0.3);
}
/* Card header with date */
.card-header {
padding: 25px 25px 15px;
border-bottom: 1px solid rgba(148, 163, 184, 0.2);
background: linear-gradient(90deg, rgba(37, 99, 235, 0.05), rgba(139, 92, 246, 0.03));
}
.experience-date {
color: var(--primary);
font-weight: 600;
font-size: 16px;
margin-bottom: 8px;
}
/* Card body */
.card-body {
padding: 25px;
flex-grow: 1;
}
.experience-title {
font-size: 22px;
font-weight: 700;
color: var(--secondary);
margin-bottom: 5px;
}
.experience-role {
color: var(--accent);
font-weight: 600;
margin-bottom: 5px;
font-size: 18px;
}
.experience-company {
font-weight: 600;
margin-bottom: 15px;
font-size: 17px;
color: var(--dark);
}
.experience-desc {
color: var(--gray);
line-height: 1.7;
margin-bottom: 20px;
}
/* Skills/tags section */
.experience-skills {
display: flex;
flex-wrap: wrap;
gap: 8px;
margin-top: 15px;
}
.skill-tag {
background: transparent;
color: var(--dark);
padding: 6px 12px;
border-radius: 999px;
font-size: 14px;
font-weight: 500;
transition: var(--transition);
border: 1px solid rgba(148, 163, 184, 0.45);
display: flex;
align-items: center;
gap: 5px;
}
.skill-tag:hover {
border-color: rgba(37, 99, 235, 0.35);
transform: translateY(-1px);
}
.skill-tag i {
font-size: 14px;
}
.skill-tag.has-logo i {
display: none;
}
.skill-tag .tag-logo {
width: 16px;
height: 16px;
object-fit: contain;
flex-shrink: 0;
}
/* Timeline indicator for mobile view */
.timeline-indicator {
display: none;
}
/* Projects Section */
.projects-grid {
display: grid;
grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
gap: 30px;
margin-top: 20px;
align-items: stretch;
}
.project-card {
background: white;
border-radius: 22px;
overflow: hidden;
box-shadow: var(--card-shadow);
transition: var(--transition);
position: relative;
display: flex;
flex-direction: column;
height: 100%;
}
.project-card:hover {
transform: translateY(-10px);
box-shadow: 0 20px 40px -5px rgba(0, 0, 0, 0.18);
}
.project-img {
height: 200px;
background: linear-gradient(45deg, var(--primary), var(--accent));
display: flex;
align-items: center;
justify-content: center;
position: relative;
overflow: hidden;
}
.project-img.color1 { background: linear-gradient(45deg, #2563eb, #8b5cf6); }
.project-img.color2 { background: linear-gradient(45deg, #0ea5e9, #14b8a6); }
.project-img.color3 { background: linear-gradient(45deg, #f97316, #f59e0b); }
.project-img.color4 { background: linear-gradient(45deg, #ef4444, #f97316); }
.project-img.color5 { background: linear-gradient(45deg, #8b5cf6, #ec4899); }
.project-img.color6 { background: linear-gradient(45deg, #4f46e5, #7c3aed); }
.project-img::before {
content: '';
position: absolute;
width: 200%;
height: 200%;
background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
animation: rotate 15s linear infinite;
}
@keyframes rotate {
0% { transform: rotate(0deg); }
100% { transform: rotate(360deg); }
}
.project-img i {
font-size: 80px;
color: rgba(255, 255, 255, 0.85);
position: relative;
animation: pulseIcon 2s infinite;
}
@keyframes pulseIcon {
0% { transform: scale(1); opacity: 0.8; }
50% { transform: scale(1.1); opacity: 1; }
100% { transform: scale(1); opacity: 0.8; }
}
.project-content {
padding: 25px;
display: block;
height: 100%;
}
.project-title {
font-size: 22px;
font-weight: 700;
color: var(--secondary);
margin-bottom: 10px;
}
.project-date {
color: var(--primary);
font-weight: 600;
margin-bottom: 15px;
display: block;
}
.project-desc {
color: var(--gray);
margin-bottom: 20px;
line-height: 1.7;
}
.project-tags {
display: flex;
flex-wrap: wrap;
gap: 8px;
margin-top: 15px;
}
.project-tag {
background: transparent;
color: var(--dark);
padding: 6px 14px;
border-radius: 50px;
font-size: 14px;
font-weight: 500;
transition: var(--transition);
border: 1px solid rgba(148, 163, 184, 0.45);
display: flex;
align-items: center;
gap: 5px;
}
.project-tag i {
font-size: 14px;
}
.project-tag.has-logo i {
display: none;
}
.project-tag .tag-logo {
width: 16px;
height: 16px;
object-fit: contain;
flex-shrink: 0;
}
.project-tag:hover {
border-color: rgba(37, 99, 235, 0.35);
transform: translateY(-1px);
}
.project-tag.log4j { background: rgba(245, 158, 11, 0.1); color: #d97706; border-color: rgba(245, 158, 11, 0.2); }
.project-tag.log4j:hover { background: #f59e0b; color: white; }
.project-tag.kafka { background: rgba(71, 85, 105, 0.1); color: #6366f1; border-color: rgba(71, 85, 105, 0.2); }
.project-tag.kafka:hover { background: #6366f1; color: white; }
.project-tag.logstash { background: rgba(220, 38, 38, 0.1); color: #dc2626; border-color: rgba(220, 38, 38, 0.2); }
.project-tag.logstash:hover { background: #dc2626; color: white; }
.project-tag.elasticsearch { background: rgba(56, 189, 113, 0.1); color: #38bda1; border-color: rgba(56, 189, 113, 0.2); }
.project-tag.elasticsearch:hover { background: #0d9488; color: white; }
.project-tag.angular { background: rgba(220, 38, 38, 0.1); color: #dd2224; border-color: rgba(220, 38, 38, 0.2); }
.project-tag.angular:hover { background: #dd2224; color: white; }
.project-tag.java { background: rgba(238, 88, 49, 0.1); color: #ee5831; border-color: rgba(238, 88, 49, 0.2); }
.project-tag.java:hover { background: #ee5831; color: white; }
.project-tag.spring { background: rgba(64, 169, 78, 0.1); color: #40a94e; border-color: rgba(64, 169, 78, 0.2); }
.project-tag.spring:hover { background: #40a94e; color: white; }
.project-tag.docker { background: rgba(27, 163, 239, 0.1); color: #1ba3ef; border-color: rgba(27, 163, 239, 0.2); }
.project-tag.docker:hover { background: #1ba3ef; color: white; }
.project-tag.postgresql { background: rgba(37, 104, 163, 0.1); color: #2568a3; border-color: rgba(37, 104, 163, 0.2); }
.project-tag.postgresql:hover { background: #2568a3; color: white; }
.project-tag.aws { background: rgba(255, 153, 0, 0.1); color: #ff9900; border-color: rgba(255, 153, 0, 0.2); }
.project-tag.aws:hover { background: #ff9900; color: white; }
/* Skills - New redesigned layout */
#skills {
background: linear-gradient(135deg, #eff6ff 0%, #dbeafe 100%);
padding-bottom: 60px;
}
.skills-grid {
display: grid;
grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
gap: 20px;
margin-top: 30px;
}
.skill-column {
background: rgba(255, 255, 255, 0.94);
border: 1px solid rgba(37, 99, 235, 0.16);
border-radius: 20px;
padding: 22px 18px 18px;
box-shadow: var(--card-shadow);
transition: var(--transition);
position: relative;
overflow: hidden;
}
.skill-column:hover {
transform: translateY(-5px);
box-shadow: 0 16px 34px -12px rgba(15, 23, 42, 0.25);
}
.skill-column::before {
content: '';
position: absolute;
top: 0;
left: 0;
width: 100%;
height: 4px;
background: linear-gradient(90deg, var(--primary), var(--accent));
}
.skill-column h3 {
color: var(--secondary);
margin-bottom: 14px;
font-size: 21px;
display: flex;
align-items: center;
gap: 10px;
}
.skill-column h3 i {
color: var(--primary);
}
.skill-fleet {
display: flex;
flex-wrap: wrap;
gap: 10px;
}
.skill-ship {
display: inline-flex;
align-items: center;
gap: 8px;
padding: 7px 11px;
border-radius: 999px;
background: transparent;
border: 1px solid rgba(148, 163, 184, 0.45);
font-size: 13px;
font-weight: 600;
color: var(--dark);
line-height: 1;
box-shadow: none;
transition: border-color 0.2s ease, transform 0.2s ease;
}
.skill-ship:hover {
transform: translateY(-1px);
border-color: rgba(37, 99, 235, 0.35);
}
.skill-ship img {
width: 16px;
height: 16px;
object-fit: contain;
}
/* Education */
.education-compact {
margin-top: 36px;
display: flex;
flex-direction: column;
gap: 18px;
}
.edu-row {
background: linear-gradient(180deg, rgba(255, 255, 255, 0.96), rgba(248, 250, 252, 0.95));
border: 1px solid rgba(37, 99, 235, 0.2);
border-radius: 20px;
box-shadow: 0 14px 30px -20px rgba(15, 23, 42, 0.45);
overflow: hidden;
transition: transform 0.25s ease, box-shadow 0.25s ease, border-color 0.25s ease;
position: relative;
}
.edu-row:hover {
transform: translateY(-3px);
border-color: rgba(59, 130, 246, 0.35);
box-shadow: 0 20px 36px -20px rgba(15, 23, 42, 0.35);
}
.edu-row::before {
content: '';
position: absolute;
left: 0;
top: 0;
bottom: 0;
width: 5px;
background: linear-gradient(180deg, var(--primary), var(--accent));
}
.edu-row[open] {
border-color: rgba(59, 130, 246, 0.45);
box-shadow: 0 24px 42px -22px rgba(15, 23, 42, 0.42);
}
.edu-row-main {
list-style: none;
cursor: pointer;
display: grid;
grid-template-columns: 96px 1fr auto;
gap: 18px;
align-items: center;
padding: 18px 22px;
}
.edu-row-main::-webkit-details-marker {
display: none;
}
.edu-side {
display: flex;
align-items: center;
gap: 10px;
}
.edu-index {
width: 26px;
height: 26px;
border-radius: 999px;
display: inline-flex;
align-items: center;
justify-content: center;
font-size: 12px;
font-weight: 700;
color: var(--primary);
background: rgba(37, 99, 235, 0.12);
border: 1px solid rgba(37, 99, 235, 0.22);
}
.edu-main-text {
min-width: 0;
}
.edu-degree {
font-size: 22px;
font-weight: 700;
color: var(--secondary);
line-height: 1.3;
}
.edu-school-link {
display: inline-block;
font-size: 17px;
color: #475569;
text-decoration: none;
margin-top: 6px;
font-weight: 500;
}
.edu-school-link:hover {
color: var(--secondary);
text-decoration: underline;
}
.edu-actions {
display: flex;
align-items: center;
gap: 12px;
}
.edu-period {
display: inline-flex;
align-items: center;
gap: 8px;
padding: 8px 14px;
border-radius: 999px;
background: linear-gradient(90deg, rgba(219, 234, 254, 0.85), rgba(224, 242, 254, 0.75));
border: 1px solid rgba(37, 99, 235, 0.25);
color: var(--primary);
font-weight: 600;
font-size: 14px;
white-space: nowrap;
}
.edu-toggle {
color: var(--primary);
font-size: 18px;
transition: transform 0.2s ease, color 0.2s ease;
}
.edu-row[open] .edu-toggle {
transform: rotate(180deg);
color: var(--accent);
}
.edu-row-extra {
padding: 0 22px 20px 136px;
}
.school-logo {
width: 60px;
height: 60px;
border-radius: 12px;
background: linear-gradient(135deg, rgba(255, 255, 255, 0.98), rgba(224, 242, 254, 0.95));
border: 1px solid rgba(37, 99, 235, 0.2);
display: flex;
align-items: center;
justify-content: center;
overflow: hidden;
flex-shrink: 0;
box-shadow: 0 8px 16px -10px rgba(15, 23, 42, 0.45);
}
.school-logo img {
width: 58px;
height: 66px;
object-fit: contain;
}
.edu-desc {
margin: 10px 0 0;
color: var(--gray);
line-height: 1.7;
font-size: 16px;
}
.tech-tags {
display: flex;
flex-wrap: wrap;
gap: 10px;
margin-top: 16px;
padding-top: 14px;
border-top: 1px dashed rgba(148, 163, 184, 0.6);
}
.tech-tag {
background: rgba(37, 99, 235, 0.1);
color: var(--primary);
padding: 6px 14px;
border-radius: 50px;
font-size: 14px;
font-weight: 500;
transition: var(--transition);
border: 1px solid rgba(37, 99, 235, 0.2);
display: flex;
align-items: center;
gap: 5px;
}
.tech-tag i {
font-size: 14px;
}
.tech-tag:hover {
background: var(--primary);
color: white;
transform: scale(1.05);
}
/* Languages */
.languages-intel {
margin-top: 28px;
display: grid;
gap: 16px;
}
.language-node {
background: linear-gradient(180deg, rgba(255, 255, 255, 0.97), rgba(248, 250, 252, 0.95));
border: 1px solid rgba(37, 99, 235, 0.16);
border-radius: 18px;
padding: 18px 18px 16px;
box-shadow: 0 14px 28px -20px rgba(15, 23, 42, 0.42);
transition: transform 0.25s ease, box-shadow 0.25s ease, border-color 0.25s ease;
position: relative;
overflow: hidden;
}
.language-node:hover {
transform: translateY(-3px);
border-color: rgba(59, 130, 246, 0.34);
box-shadow: 0 18px 34px -18px rgba(15, 23, 42, 0.36);
}
.language-node::before {
content: '';
position: absolute;
left: 0;
top: 0;
bottom: 0;
width: 4px;
background: linear-gradient(180deg, var(--primary), var(--accent));
}
.language-node.native::before {
background: linear-gradient(180deg, #10b981, #22c55e);
}
.language-top {
display: flex;
align-items: center;
justify-content: space-between;
gap: 12px;
margin-bottom: 12px;
}
.language-id {
display: flex;
align-items: center;
gap: 10px;
}
.language-pin {
width: 11px;
height: 11px;
border-radius: 50%;
background: linear-gradient(135deg, var(--primary), var(--accent));
box-shadow: 0 0 0 6px rgba(37, 99, 235, 0.14);
}
.language-node.native .language-pin {
background: linear-gradient(135deg, #10b981, #22c55e);
box-shadow: 0 0 0 6px rgba(16, 185, 129, 0.14);
}
.language-name-title {
font-size: 28px;
line-height: 1.1;
font-weight: 700;
color: var(--secondary);
}
.language-level-pill {
display: inline-flex;
align-items: center;
padding: 7px 12px;
border-radius: 999px;
font-size: 12px;
font-weight: 700;
white-space: nowrap;
border: 1px solid rgba(37, 99, 235, 0.18);
background: rgba(219, 234, 254, 0.7);
color: var(--primary);
}
.language-node.native .language-level-pill {
background: rgba(16, 185, 129, 0.14);
border-color: rgba(16, 185, 129, 0.3);
color: #0f766e;
}
.language-node.intermediate .language-level-pill {
background: rgba(245, 158, 11, 0.14);
border-color: rgba(245, 158, 11, 0.3);
color: #b45309;
}
.language-matrix {
display: grid;
grid-template-columns: repeat(3, minmax(0, 1fr));
gap: 10px;
}
.lang-metric {
background: rgba(241, 245, 249, 0.85);
border: 1px solid rgba(148, 163, 184, 0.2);
border-radius: 12px;
padding: 8px 10px;
}
.metric-head {
display: flex;
justify-content: space-between;
align-items: center;
font-size: 12px;
font-weight: 600;
color: #334155;
margin-bottom: 6px;
}
.metric-bar {
height: 8px;
border-radius: 999px;
background: rgba(148, 163, 184, 0.22);
overflow: hidden;
}
.metric-bar span {
display: block;
height: 100%;
width: var(--value);
border-radius: 999px;
background: linear-gradient(90deg, var(--primary), var(--accent));
}
.language-node.native .metric-bar span {
background: linear-gradient(90deg, #10b981, #22c55e);
}
.language-node.intermediate .metric-bar span {
background: linear-gradient(90deg, #f59e0b, #f97316);
}
/* Hobbies Section */
#hobbies {
background: linear-gradient(135deg, #eff6ff 0%, #dbeafe 100%);
}
.hobbies-grid {
display: grid;
grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
gap: 20px;
padding-top: 26px;
}
.hobby-card {
background: linear-gradient(170deg, rgba(255, 255, 255, 0.98), rgba(239, 246, 255, 0.93));
border-radius: 22px;
padding: 24px 22px;
text-align: left;
box-shadow: 0 14px 28px -16px rgba(15, 23, 42, 0.28);
transition: transform 0.25s ease, box-shadow 0.25s ease, border-color 0.25s ease;
position: relative;
overflow: hidden;
border: 1px solid rgba(148, 163, 184, 0.28);
}
.hobby-card::before {
content: '';
position: absolute;
inset: 0 auto auto 0;
width: 100%;
height: 5px;
background: linear-gradient(90deg, #3b82f6, #60a5fa);
opacity: 0.95;
}
.hobby-card:hover {
transform: translateY(-6px);
box-shadow: 0 20px 34px -18px rgba(15, 23, 42, 0.34);
border-color: rgba(59, 130, 246, 0.42);
}
.hobby-icon {
width: 56px;
height: 56px;
border-radius: 16px;
display: inline-flex;
align-items: center;
justify-content: center;
font-size: 28px;
margin-bottom: 14px;
color: #2563eb;
background: rgba(59, 130, 246, 0.12);
transition: transform 0.25s ease, box-shadow 0.25s ease;
position: relative;
}
.hobby-card:hover .hobby-icon {
transform: translateY(-2px) scale(1.05);
box-shadow: 0 8px 16px -10px rgba(37, 99, 235, 0.55);
}
.hobby-card h3 {
font-size: 24px;
line-height: 1.2;
margin-bottom: 10px;
color: var(--secondary);
}
.hobby-card p {
font-size: 15px;
line-height: 1.7;
color: #334155;
margin-bottom: 12px;
}
.hobby-note {
display: inline-flex;
align-items: center;
gap: 8px;
font-size: 13px;
font-weight: 600;
padding: 7px 12px;
border-radius: 999px;
background: rgba(59, 130, 246, 0.1);
color: #1d4ed8;
border: 1px solid rgba(59, 130, 246, 0.2);
}
.hobby-note i {
font-size: 12px;
}
.hobby-card.chess::before {
background: linear-gradient(90deg, #4f46e5, #818cf8);
}
.hobby-card.outdoor::before {
background: linear-gradient(90deg, #0ea5a4, #22d3ee);
}
.hobby-card.learning::before {
background: linear-gradient(90deg, #2563eb, #60a5fa);
}
.hobby-card.music::before {
background: linear-gradient(90deg, #0f766e, #34d399);
}
/* Contact */
.contact-container {
display: grid;
grid-template-columns: minmax(320px, 1.05fr) minmax(320px, 1fr);
gap: 26px;
padding-top: 28px;
align-items: stretch;
}
.contact-details {
display: flex;
flex-direction: column;
gap: 14px;
height: 100%;
}
.contact-method {
display: flex;
gap: 14px;
background: linear-gradient(135deg, rgba(255, 255, 255, 0.98), rgba(239, 246, 255, 0.9));
padding: 16px 18px;
border-radius: 16px;
box-shadow: 0 10px 24px -18px rgba(15, 23, 42, 0.35);
transition: transform 0.25s ease, box-shadow 0.25s ease, border-color 0.25s ease;
align-items: center;
border: 1px solid rgba(148, 163, 184, 0.24);
}
.contact-method:hover {
transform: translateY(-3px);
box-shadow: 0 16px 28px -20px rgba(15, 23, 42, 0.4);
border-color: rgba(37, 99, 235, 0.35);
}
.contact-icon {
width: 52px;
height: 52px;
border-radius: 14px;
display: flex;
align-items: center;
justify-content: center;
font-size: 22px;
flex-shrink: 0;
color: white;
transition: var(--transition);
background: var(--gray);
}
.contact-method.email .contact-icon {
background: var(--gmail-color);
}
.contact-method.phone .contact-icon {
background: var(--phone-color);
}
.contact-method.location .contact-icon {
background: var(--location-color);
}
.contact-method.whatsapp .contact-icon {
background: var(--whatsapp-color);
}
/* Effet hover (optionnel, tu peux garder la même couleur ou foncer) */
.contact-method.email:hover .contact-icon {
background: var(--gmail-color);
}
.contact-method.phone:hover .contact-icon {
background: var(--phone-color);
}
.contact-method.location:hover .contact-icon {
background: var(--location-color);
}
.contact-method.whatsapp:hover .contact-icon {
background: var(--whatsapp-color);
}
.contact-text h3 {
color: var(--secondary);
margin-bottom: 2px;
font-size: 21px;
line-height: 1.2;
}
.contact-text p {
font-size: 15px;
color: #334155;
}
.contact-form {
background: linear-gradient(160deg, rgba(255, 255, 255, 0.99), rgba(239, 246, 255, 0.92));
padding: 28px;
border-radius: 20px;
box-shadow: 0 16px 30px -20px rgba(15, 23, 42, 0.4);
border: 1px solid rgba(148, 163, 184, 0.26);
position: relative;
overflow: hidden;
height: 100%;
}
.contact-form form {
display: flex;
flex-direction: column;
height: 100%;
}
.contact-form::before {
content: '';
position: absolute;
top: 0;
left: 0;
right: 0;
height: 4px;
background: linear-gradient(90deg, #2563eb, #38bdf8);
}
.form-group {
margin-bottom: 16px;
}
.form-group label {
display: block;
margin-bottom: 8px;
font-weight: 600;
color: var(--dark);
font-size: 15px;
}
.form-control {
width: 100%;
padding: 14px 16px;
background: rgba(248, 250, 252, 0.92);
border: 1px solid rgba(148, 163, 184, 0.28);
border-radius: 12px;
color: var(--dark);
font-family: 'Poppins', sans-serif;
font-size: 15px;
transition: var(--transition);
outline: none;
}
.form-control:focus {
border-color: #3b82f6;
box-shadow: 0 0 0 3px rgba(59, 130, 246, 0.15);
background: #fff;
}
.form-control::placeholder {
color: var(--gray);
}
textarea.form-control {
min-height: 130px;
resize: vertical;
}
.submit-btn {
width: 100%;
background: linear-gradient(90deg, var(--primary), var(--secondary));
color: white;
border: none;
padding: 14px;
border-radius: 12px;
font-weight: 600;
cursor: pointer;
transition: var(--transition);
font-size: 16px;
margin-top: 6px;
box-shadow: 0 8px 18px -10px rgba(37, 99, 235, 0.55);
position: relative;
overflow: hidden;
}
.submit-btn::before {
content: '';
position: absolute;
top: 0;
left: -100%;
width: 100%;
height: 100%;
background: linear-gradient(90deg, transparent, rgba(255,255,255,0.2), transparent);
transition: var(--transition);
}
.submit-btn:hover {
transform: translateY(-2px);
box-shadow: 0 12px 22px -10px rgba(37, 99, 235, 0.6);
}
.submit-btn:hover::before {
left: 100%;
}
/* Toast Notification */
.toast {
position: fixed;
bottom: 30px;
right: 30px;
background: white;
color: var(--dark);
padding: 15px 25px;
border-radius: 12px;
box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
display: flex;
align-items: center;
gap: 15px;
z-index: 9999;
transform: translateX(200%);
transition: transform 0.4s ease, opacity 0.4s ease;
opacity: 0;
}
.toast.show {
transform: translateX(0);
opacity: 1;
}
.toast.success {
border-left: 4px solid var(--success);
}
.toast i {
font-size: 24px;
}
.toast.success i {
color: var(--success);
}
.toast .message {
font-weight: 500;
}
.toast .close-toast {
background: none;
border: none;
font-size: 18px;
color: var(--gray);
cursor: pointer;
margin-left: 15px;
}
/* Map */
.map-container {
min-height: 280px;
border-radius: 16px;
overflow: hidden;
margin-top: 4px;
box-shadow: 0 16px 28px -20px rgba(15, 23, 42, 0.45);
position: relative;
border: 1px solid rgba(148, 163, 184, 0.24);
flex: 1 1 auto;
}
iframe {
border: none;
width: 100%;
height: 100%;
}
/* Footer */
footer {
background: linear-gradient(40deg, #01183a 0%, #010c1c 52%, #001027 100%);
color: var(--light);
text-align: center;
padding: 50px 0 30px;
margin-top: 50px;
position: relative;
overflow: hidden;
border-top: 1px solid rgba(191, 219, 254, 0.35);
}
footer::before {
content: '';
position: absolute;
top: -50%;
left: -50%;
width: 200%;
height: 200%;
background: transparent;
z-index: 0;
animation: none;
}
footer::after {
content: '';
position: absolute;
inset: -30%;
background: transparent;
opacity: 0;
z-index: 0;
animation: none;
}
.footer-content {
max-width: 700px;
margin: 0 auto;
position: relative;
z-index: 2;
}
.footer-starry-background {
position: absolute;
inset: 0;
z-index: 0;
}
.footer-starry-background::before {
content: '';
position: absolute;
width: 200%;
height: 200%;
background: radial-gradient(circle, rgba(255,255,255,0.1) 1px, transparent 1px);
background-size: 50px 50px;
animation: rotateStars 200s linear infinite;
}
.footer-starry-background::after {
content: '';
position: absolute;
inset: 0;
background: radial-gradient(ellipse at center, rgba(147, 197, 253, 0.1) 0%, rgba(99, 102, 241, 0.04) 50%, rgba(99, 102, 241, 0) 78%);
}
.footer-network-canvas {
z-index: 1;
opacity: 0.72;
}
.footer-logo {
font-family: 'Montserrat', sans-serif;
font-size: 32px;
margin-bottom: 15px;
background:  var(--light);
-webkit-background-clip: text;
-webkit-text-fill-color: transparent;
}
.footer-links {
display: flex;
justify-content: center;
gap: 25px;
margin: 25px 0;
flex-wrap: wrap;
}
.footer-links a {
color: var(--light-gray);
text-decoration: none;
transition: var(--transition);
font-size: 17px;
padding: 5px 0;
}
.footer-links a:hover {
color: #7dd3fc;
}
.copyright {
color: var(--light-gray);
font-size: 16px;
margin-top: 20px;
}
.socials-footer {
display: flex;
justify-content: center;
gap: 18px;
margin: 15px 0;
flex-wrap: wrap;
}
/* Animation Classes */
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
@keyframes bounce {
0%, 100% { transform: translateY(0); }
50% { transform: translateY(-10px); }
}
.floating {
animation: floating 3s ease-in-out infinite;
}
@keyframes floating {
0% { transform: translateY(0px); }
50% { transform: translateY(-15px); }
100% { transform: translateY(0px); }
}
.pulse {
animation: pulse 2s infinite;
}
@keyframes pulse {
0% { transform: scale(1); opacity: 1; }
50% { transform: scale(1.05); opacity: 0.8; }
100% { transform: scale(1); opacity: 1; }
}
@keyframes shine {
0% { background-position: -100% 0; }
100% { background-position: 100% 0; }
}
/* Progress animations */
.progress-animated .skill-progress {
animation: progress 1.5s ease forwards;
}
@keyframes progress {
from { width: 0; }
to { width: var(--width); }
}
/* Scroll Progress Indicator */
#scroll-progress {
position: fixed;
top: 0;
left: 0;
height: 4px;
background: linear-gradient(90deg, var(--primary), var(--accent));
z-index: 9999;
transition: width 0.1s;
}
/* Custom scrollbar */
::-webkit-scrollbar {
width: 10px;
}
::-webkit-scrollbar-track {
background: #f1f5f9;
}
::-webkit-scrollbar-thumb {
background: linear-gradient(var(--primary), var(--accent));
border-radius: 5px;
}
::-webkit-scrollbar-thumb:hover {
background: var(--secondary);
}
/* Mobile menu */
.mobile-menu {
position: fixed;
top: 70px;
left: 0;
width: 100%;
background: white;
box-shadow: 0 4px 6px rgba(0,0,0,0.1);
padding: 15px 0;
display: none;
z-index: 999;
}
.mobile-menu a {
display: block;
padding: 12px 24px;
color: var(--dark);
text-decoration: none;
font-weight: 500;
border-bottom: 1px solid var(--light-gray);
}
.mobile-menu a:last-child {
border-bottom: none;
}
.mobile-menu a.active, .mobile-menu a:hover {
color: var(--primary);
background: rgba(37, 99, 235, 0.05);
}
/* Animation for section titles */
@keyframes slideInTitle {
0% { transform: translateX(-30px); opacity: 0; }
100% { transform: translateX(0); opacity: 1; }
}
.section-title {
animation: slideInTitle 0.8s ease forwards;
}
/* Section background alternation for better visual separation */
#experience {
background: linear-gradient(135deg, #f0f9ff 0%, #e0f2fe 100%);
}
#projects {
background: linear-gradient(135deg, #dbeafe 0%, #bfdbfe 100%);
}
#skills {
background: linear-gradient(135deg, #eff6ff 0%, #dbeafe 100%);
}
#education {
background: linear-gradient(135deg, #f0f9ff 0%, #e0f2fe 100%);
}
#languages {
background: linear-gradient(135deg, #dbeafe 0%, #bfdbfe 100%);
}
#hobbies {
background: linear-gradient(135deg, #eff6ff 0%, #dbeafe 100%);
}
#contact {
background: linear-gradient(135deg, #f0f9ff 0%, #e0f2fe 100%);
position: relative;
overflow: hidden;
}
#contact::before {
content: '';
position: absolute;
top: -120px;
right: -120px;
width: 360px;
height: 360px;
border-radius: 50%;
background: radial-gradient(circle, rgba(59, 130, 246, 0.12) 0%, rgba(59, 130, 246, 0) 70%);
pointer-events: none;
}
#contact::after {
content: '';
position: absolute;
left: -100px;
bottom: -130px;
width: 300px;
height: 300px;
border-radius: 50%;
background: radial-gradient(circle, rgba(14, 165, 233, 0.1) 0%, rgba(14, 165, 233, 0) 72%);
pointer-events: none;
}
#contact .container {
position: relative;
z-index: 1;
}
/* Dark mode */
body.dark-mode {
background: linear-gradient(135deg, #020617 0%, #0f172a 100%);
color: #e2e8f0;
color-scheme: dark;
}
body.dark-mode::before {
background: radial-gradient(circle at 10% 20%, rgba(59, 130, 246, 0.2) 0%, rgba(2, 6, 23, 0) 28%);
}
body.dark-mode nav {
background: rgba(2, 6, 23, 0.9);
box-shadow: 0 2px 10px rgba(0, 0, 0, 0.35);
}
body.dark-mode nav.scrolled {
background: rgba(2, 6, 23, 0.96);
}
body.dark-mode .nav-logo span,
body.dark-mode .nav-links a,
body.dark-mode .mobile-menu a {
color: #e2e8f0;
}
body.dark-mode .theme-toggle {
background: rgba(30, 64, 175, 0.35);
border-color: rgba(147, 197, 253, 0.35);
color: #dbeafe;
}
body.dark-mode .theme-toggle:hover {
background: rgba(37, 99, 235, 0.45);
}
body.dark-mode .mobile-theme-toggle {
background: rgba(30, 64, 175, 0.35);
border-color: rgba(147, 197, 253, 0.35);
color: #dbeafe;
}
body.dark-mode .mobile-theme-toggle:hover {
background: rgba(37, 99, 235, 0.45);
}
body.dark-mode .mobile-menu {
background: #0b1220;
border-top: 1px solid rgba(148, 163, 184, 0.2);
}
body.dark-mode .mobile-menu a {
border-bottom: 1px solid rgba(148, 163, 184, 0.2);
}
body.dark-mode .mobile-menu a.active,
body.dark-mode .mobile-menu a:hover {
background: rgba(37, 99, 235, 0.2);
}
body.dark-mode #experience,
body.dark-mode #projects,
body.dark-mode #skills,
body.dark-mode #education,
body.dark-mode #languages,
body.dark-mode #hobbies,
body.dark-mode #contact {
background: linear-gradient(135deg, #0f172a 0%, #111827 100%);
}
body.dark-mode .section-title,
body.dark-mode .experience-title,
body.dark-mode .company-summary-text h3,
body.dark-mode .contact-text h3,
body.dark-mode .education-degree,
body.dark-mode .project-title {
color: #93c5fd;
}
body.dark-mode .section-description,
body.dark-mode .experience-desc,
body.dark-mode .company-summary-text p,
body.dark-mode .contact-text p,
body.dark-mode .education-institution,
body.dark-mode .project-desc,
body.dark-mode .hobby-card p,
body.dark-mode .language-level {
color: #cbd5e1;
}
body.dark-mode .company-group,
body.dark-mode .experience-card,
body.dark-mode .project-card,
body.dark-mode .skill-column,
body.dark-mode .edu-row,
body.dark-mode .language-node,
body.dark-mode .education-card,
body.dark-mode .language-card,
body.dark-mode .hobby-card,
body.dark-mode .contact-method,
body.dark-mode .contact-form,
body.dark-mode .toast {
background: rgba(15, 23, 42, 0.9);
border-color: rgba(148, 163, 184, 0.3);
box-shadow: 0 10px 24px -14px rgba(0, 0, 0, 0.65);
color: #e2e8f0;
}
body.dark-mode .project-content,
body.dark-mode .project-date,
body.dark-mode .project-desc {
color: #e2e8f0;
}
body.dark-mode .edu-degree,
body.dark-mode .language-name-title {
color: #dbeafe;
}
body.dark-mode .edu-school-link,
body.dark-mode .edu-desc,
body.dark-mode .metric-head {
color: #cbd5e1;
}
body.dark-mode .edu-school-link:hover {
color: #93c5fd;
}
body.dark-mode .edu-period,
body.dark-mode .language-level-pill {
background: rgba(30, 64, 175, 0.2);
border-color: rgba(147, 197, 253, 0.35);
color: #bfdbfe;
}
body.dark-mode .language-node.native .language-level-pill {
background: rgba(16, 185, 129, 0.2);
border-color: rgba(16, 185, 129, 0.4);
color: #a7f3d0;
}
body.dark-mode .language-node.intermediate .language-level-pill {
background: rgba(245, 158, 11, 0.2);
border-color: rgba(245, 158, 11, 0.4);
color: #fde68a;
}
body.dark-mode .school-logo {
background: linear-gradient(135deg, rgba(15, 23, 42, 0.95), rgba(30, 41, 59, 0.9));
border-color: rgba(148, 163, 184, 0.3);
}
body.dark-mode .lang-metric {
background: rgba(15, 23, 42, 0.75);
border-color: rgba(148, 163, 184, 0.28);
}
body.dark-mode .metric-bar {
background: rgba(148, 163, 184, 0.3);
}
body.dark-mode .tech-tags {
border-top-color: rgba(148, 163, 184, 0.35);
}
body.dark-mode footer {
background: linear-gradient(40deg, #01183a 0%, #010c1c 52%, #001027 100%);
border-top: none;
margin-top: 0;
}
body.dark-mode footer .footer-links a,
body.dark-mode footer .copyright,
body.dark-mode footer p {
color: rgba(226, 232, 240, 0.92);
}
body.dark-mode .project-date {
color: #93c5fd;
}
body.dark-mode .skill-column h3 {
color: #bfdbfe;
}
body.dark-mode .skill-ship,
body.dark-mode .project-tag,
body.dark-mode .skill-tag,
body.dark-mode .tech-tag {
color: #e2e8f0 !important;
border-color: rgba(148, 163, 184, 0.45) !important;
background: rgba(15, 23, 42, 0.35) !important;
}
body.dark-mode .card-header,
body.dark-mode .company-summary {
background: linear-gradient(90deg, rgba(30, 64, 175, 0.25), rgba(30, 41, 59, 0.18));
border-bottom-color: rgba(148, 163, 184, 0.22);
}
body.dark-mode .form-group label,
body.dark-mode .form-control {
color: #e2e8f0;
}
body.dark-mode .form-control {
background: rgba(15, 23, 42, 0.85);
border-color: rgba(148, 163, 184, 0.38);
}
body.dark-mode .form-control:focus {
background: rgba(15, 23, 42, 0.95);
}
body.dark-mode .form-control::placeholder {
color: #94a3b8;
}
body.dark-mode ::-webkit-scrollbar-track {
background: #0f172a;
}
/* Responsive Adjustments */
@media (max-width: 992px) {
.hero-content {
flex-direction: column;
gap: 34px;
}
.profile-wrapper-centered {
flex: none;
width: 100%;
}
.hero-text-centered h1 {
font-size: 42px;
}
.profile-container-centered {
width: 250px;
height: 250px;
}
.profile-img-centered {
width: 240px;
height: 240px;
}
.projects-grid {
grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
}
}
@media (max-width: 768px) {
.hero-content {
gap: 30px;
}
.hero-text-centered h1 {
font-size: 36px;
}
.profile-container-centered {
width: 220px;
height: 220px;
}
.profile-img-centered {
width: 210px;
height: 210px;
}
.nav-links {
display: none;
}
.mobile-toggle {
display: block;
}
.theme-toggle span {
display: none;
}
.mobile-theme-toggle {
display: block;
}
.section-title {
font-size: 30px;
}
.section-description {
font-size: 16px;
}
.btn {
display: block;
width: 100%;
margin: 10px 0;
}
.btn-outline {
margin-left: 0;
margin-top: 10px;
}
.contact-info {
flex-direction: column;
}
.contact-container {
grid-template-columns: 1fr;
}
.typewriter {
font-size: 22px;
width: 30ch;
}
.experience-grid {
padding-left: 0;
gap: 14px;
}
.company-jobs {
padding-left: 42px;
}
.company-jobs::before {
left: 14px;
}
.company-jobs .experience-card::before {
left: -31px;
}
.projects-grid,
.skills-grid,
.hobbies-grid {
grid-template-columns: 1fr;
}
.language-top {
flex-direction: column;
align-items: flex-start;
gap: 9px;
}
.language-matrix {
grid-template-columns: 1fr;
}
.language-name-title {
font-size: 22px;
}
.edu-row-main {
grid-template-columns: 1fr;
row-gap: 10px;
}
.edu-side {
width: fit-content;
}
.edu-actions {
width: 100%;
justify-content: space-between;
}
.edu-period {
width: fit-content;
}
.edu-toggle {
display: none;
}
.edu-row-extra {
padding-left: 18px;
}
.school-logo {
align-self: flex-start;
}
.contact-method {
flex-direction: row;
text-align: left;
align-items: center;
}
.contact-icon {
margin-bottom: 0;
}
.map-container {
height: 250px;
}
footer .footer-links {
flex-direction: column;
align-items: center;
gap: 10px;
}
}
@media (max-width: 480px) {
:root {
--card-shadow: 0 5px 15px -3px rgba(0, 0, 0, 0.1);
}
.hero-text-centered h1 {
font-size: 28px;
line-height: 1.3;
}
.hero-text-centered h1 span {
font-size: 24px;
}
.typewriter {
font-size: 20px;
width: 14ch;
white-space: normal;
word-break: break-word;
}
.summary-box {
padding: 20px 15px;
font-size: 16px;
}
.contact-item {
font-size: 15px;
padding: 6px 12px;
}
.socials {
gap: 12px;
}
.social-link {
width: 50px;
height: 50px;
font-size: 20px;
}
.btn {
padding: 14px 25px;
font-size: 16px;
}
.profile-container-centered {
width: 180px;
height: 180px;
}
.profile-img-centered {
width: 170px;
height: 170px;
}
.section-title {
font-size: 26px;
}
.section-description {
font-size: 15px;
}
.project-img {
height: 160px;
}
.project-img i {
font-size: 60px;
}
.project-title {
font-size: 20px;
}
.experience-title, .project-title, .edu-title {
font-size: 20px;
}
.skill-column h3, .hobby-card h3 {
font-size: 20px;
}
.language-name-title { font-size: 19px; }
.contact-icon {
width: 55px;
height: 55px;
font-size: 22px;
}
.contact-text h3 {
font-size: 18px;
}
.contact-form {
padding: 25px 20px;
}
.form-control {
padding: 14px 15px;
font-size: 15px;
}
.submit-btn {
padding: 14px;
font-size: 16px;
}
.map-container {
height: 200px;
}
.footer-logo {
font-size: 26px;
}
.copyright {
font-size: 14px;
}
.school-logo {
width: 50px;
height: 50px;
}
.edu-degree {
font-size: 17px;
}
.edu-school-link {
font-size: 14px;
}
.tech-tag {
font-size: 13px;
padding: 5px 12px;
}
.skill-name {
font-size: 15px;
}
.skill-name i {
font-size: 16px;
}
.experience-date, .project-date {
font-size: 15px;
}
.hobby-icon {
font-size: 45px;
}
.project-tags, .experience-skills, .tech-tags {
gap: 6px;
}
.project-tag, .skill-tag, .tech-tag {
font-size: 13px;
padding: 5px 10px;
}
.project-tag i, .skill-tag i, .tech-tag i {
font-size: 12px;
}
.project-tag .tag-logo, .skill-tag .tag-logo {
width: 14px;
height: 14px;
}
}
.responsive-title {
font-size: clamp(18px, 5vw, 64px);
white-space: normal;   /* autorise le retour à la ligne */
text-align: center;
width: 100%;
}
.responsive-title span {
display: inline-block;
}
</style>
</head>
<body>
<!-- Scroll Progress Indicator -->
<div id="scroll-progress"></div>
<!-- Toast Notification -->
<div class="toast success" id="successToast">
<i class="fas fa-check-circle"></i>
<div class="message">Your message has been sent successfully!</div>
<button class="close-toast" id="closeToast">&times;</button>
</div>
<!-- Navbar -->
<nav id="navbar">
<div class="container nav-container">
<a href="#hero" class="nav-logo">Lotfi<span>Hmida</span></a>
<div class="nav-links">
<a href="#hero" class="nav-link active">Home</a>
<a href="#experience" class="nav-link">Experience</a>
<a href="#projects" class="nav-link">Projects</a>
<a href="#skills" class="nav-link">Skills</a>
<a href="#education" class="nav-link">Education</a>
<a href="#languages" class="nav-link">Languages</a>
<a href="#hobbies" class="nav-link">Hobbies</a>
<a href="#contact" class="nav-link">Contact</a>
</div>
<div class="nav-actions">
<button class="theme-toggle" id="themeToggle" aria-label="Activer mode sombre">
<i class="fas fa-moon"></i>
<span>Mode sombre</span>
</button>
<button class="mobile-toggle" id="mobileToggle">
<i class="fas fa-bars"></i>
</button>
</div>
</div>
<div class="mobile-menu" id="mobileMenu">
<button class="mobile-theme-toggle" id="mobileThemeToggle" aria-label="Activer mode sombre">
<i class="fas fa-moon"></i>
 Mode sombre
</button>
<a href="#hero" class="nav-link">Home</a>
<a href="#experience" class="nav-link">Experience</a>
<a href="#projects" class="nav-link">Projects</a>
<a href="#skills" class="nav-link">Skills</a>
<a href="#education" class="nav-link">Education</a>
<a href="#languages" class="nav-link">Languages</a>
<a href="#hobbies" class="nav-link">Hobbies</a>
<a href="#contact" class="nav-link">Contact</a>
</div>
</nav>
<!-- NEW STUNNING HERO SECTION -->
<section id="hero">
<div class="starry-background">
<div class="nebula"></div>
<div class="nebula"></div>
<div class="nebula"></div>
</div>
<canvas id="heroNetwork" class="network-canvas"></canvas>
<div class="comet" style="--duration: 12s; --delay: 0s; --start-x: -100px; --start-y: 50%; --end-x: 110%; --end-y: 50%;"></div>
<div class="comet" style="--duration: 15s; --delay: 4s; --start-x: -50px; --start-y: 30%; --end-x: 110%; --end-y: 60%;"></div>
<div class="comet" style="--duration: 18s; --delay: 8s; --start-x: -80px; --start-y: 70%; --end-x: 110%; --end-y: 40%;"></div>
<div class="container content-wrapper">
<div class="hero-content">
<!-- Centered profile image at the top -->
<div class="profile-wrapper-centered">
<div class="profile-container-centered">
<div class="profile-border-centered"></div>
<div class="profile-img-centered floating" id="profileImg" role="button" tabindex="0" aria-label="Agrandir la photo de profil" style="background-image: url('images/lo.jpg');"></div>
</div>
<div class="hero-buttons">
<a href="images\cv_lotfi_hmida_english.pdf" class="btn" target="_blank">Download CV</a>
<a href="#contact" class="btn btn-outline">Contact Me</a>
</div>
</div>
<!-- Centered text content below the image -->
<div class="hero-text-centered">
<h1 class="responsive-title">
<span>Full</span>
<span>Stack</span>
<span>Java/Angular</span>
<span>Engineer</span>
</h1>
<div class="typewriter-container">
<div class="typewriter">Building Scalable Enterprise Solutions</div>
</div>
<div class="summary-box">
<p>
As a software engineer, I am dedicated to crafting efficient and robust solutions, constantly seeking opportunities to expand my knowledge and create meaningful impact. Possessing a natural enthusiasm, insatiable curiosity, and a knack for rapid learning, I am poised to drive innovation and make a tangible difference.
</p>
</div>
<div class="contact-info">
<div class="contact-item email"><i class="fas fa-envelope"></i> lotfi.hmida01@gmail.com</div>
<div class="contact-item phone"><i class="fas fa-phone"></i> +216 25 622 677</div>
<div class="contact-item location"><i class="fas fa-map-marker-alt"></i> Tunis, Tunisia</div>
<div class="contact-item whatsapp"><i class="fab fa-whatsapp"></i> +216 25 622 677</div>
</div>
<div class="socials">
<a href="https://github.com/lotfi2020-2021" target="_blank" class="social-link github"><i class="fab fa-github"></i></a>
<a href="https://www.linkedin.com/in/lotfi-hmida" target="_blank" class="social-link linkedin"><i class="fab fa-linkedin-in"></i></a>
<a href="https://www.instagram.com/lotfi_hmeda" target="_blank" class="social-link instagram"><i class="fab fa-instagram"></i></a>
<a href="https://www.facebook.com/lot.fi.801148" target="_blank" class="social-link facebook"><i class="fab fa-facebook-f"></i></a>
<a href="https://wa.me/21625622677" target="_blank" class="social-link whatsapp"><i class="fab fa-whatsapp"></i></a>
</div>
</div>
</div>
</div>
</section>
<!-- NEW EXPERIENCE SECTION (REPLACING TIMELINE) -->
<section id="experience">
<div class="container">
<h2 class="section-title">Professional Experience </h2>
<p class="section-description">My career progression showcasing my growth from software engineer to technical leadership roles.</p>
<div class="experience-grid">
<details class="company-group wind-group">
<summary class="company-summary">
<div class="company-summary-info">
<div class="company-logo">W</div>
<div class="company-summary-text">
<h3>Wind Consulting</h3>
<p>6 roles · Jan 2023 - Present</p>
</div>
</div>
<i class="fas fa-chevron-down company-toggle-icon"></i>
</summary>
<div class="company-jobs">
<!-- Current Position -->
<div class="experience-card current">
<div class="card-header">
<div class="experience-date">Aug 2025 – Present</div>
<div class="company-header">
<div class="company-logo">W</div>
<div class="experience-company">Wind Consulting</div>
</div>
</div>
<div class="card-body">
<h3 class="experience-title">Full Stack Engineer</h3>
<span class="experience-role">Technical Leadership</span>
<p class="experience-desc">
Technical leadership role overseeing architecture decisions, code quality, and team coordination for a critical healthcare management platform serving multiple Tunisian hospitals. Responsible for technology stack selection, microservices design, and mentoring junior developers.
</p>
<p class="experience-desc">
<strong>Project:</strong> Hospitals Management Platform
</p>
<div class="experience-skills">
<span class="skill-tag"><i class="fas fa-crown"></i> Technical Leadership</span>
<span class="skill-tag"><i class="fas fa-project-diagram"></i> System Architecture</span>
<span class="skill-tag"><i class="fas fa-cogs"></i> JHipster</span>
<span class="skill-tag"><i class="fab fa-bitbucket"></i> Bitbucket</span>
<span class="skill-tag"><i class="fab fa-java"></i> Java</span>
<span class="skill-tag"><i class="fab fa-angular"></i> Angular</span>
<span class="skill-tag"><i class="fas fa-cube"></i> Microservices</span>
<span class="skill-tag"><i class="fas fa-database"></i> PostgreSQL</span>
<span class="skill-tag"><i class="fas fa-search"></i> Elasticsearch</span>
</div>
</div>
</div>
<!-- Dubai Now Application -->
<div class="experience-card">
<div class="card-header">
<div class="experience-date">Apr 2025 – Aug 2025</div>
<div class="company-header">
<div class="company-logo">W</div>
<div class="experience-company">Wind Consulting</div>
</div>
</div>
<div class="card-body">
<h3 class="experience-title">Backend Engineer</h3>
<span class="experience-role">Healthcare Systems</span>
<p class="experience-desc">
Led backend development for a critical health module within the Dubai Now application. Collaborated with Dubai Health Authority to integrate systems and ensure compliance with healthcare data regulations while delivering high-performance APIs.
</p>
<p class="experience-desc">
<strong>Project:</strong> Dubai Now Application (Health Module)
</p>
<div class="experience-skills">
<span class="skill-tag"><i class="fab fa-java"></i> Java</span>
<span class="skill-tag"><i class="fas fa-leaf"></i> Spring Boot</span>
<span class="skill-tag"><i class="fas fa-shield-alt"></i> Data Security</span>
<span class="skill-tag"><i class="fas fa-tasks"></i> Agile (Scrum)</span>
<span class="skill-tag"><i class="fas fa-users"></i> Team Collaboration</span>
</div>
</div>
</div>
<!-- Autopal Platform -->
<div class="experience-card">
<div class="card-header">
<div class="experience-date">Sep 2024 – Mar 2025</div>
<div class="company-header">
<div class="company-logo">W</div>
<div class="experience-company">Wind Consulting</div>
</div>
</div>
<div class="card-body">
<h3 class="experience-title">Full Stack Engineer</h3>
<span class="experience-role">Vehicle Management Systems</span>
<p class="experience-desc">
Spearheaded development of a comprehensive vehicle management platform with focus on microservice architecture and real-time features. Responsible for both frontend Angular interfaces and backend Java services with emphasis on performance optimization and user experience.
</p>
<p class="experience-desc">
<strong>Project:</strong> Autopal Platform
</p>
<div class="experience-skills">
<span class="skill-tag"><i class="fab fa-java"></i> Java</span>
<span class="skill-tag"><i class="fas fa-leaf"></i> Spring Boot</span>
<span class="skill-tag"><i class="fab fa-angular"></i> Angular</span>
<span class="skill-tag"><i class="fas fa-mobile-alt"></i> Mobile Integration</span>
<span class="skill-tag"><i class="fas fa-exchange-alt"></i> RabbitMQ</span>
<span class="skill-tag"><i class="fas fa-comments"></i> WebSocket</span>
<span class="skill-tag"><i class="fab fa-docker"></i> Docker</span>
<span class="skill-tag"><i class="fas fa-exchange-alt"></i> Kafka</span>
</div>
</div>
</div>
<!-- Konouz ERP -->
<div class="experience-card">
<div class="card-header">
<div class="experience-date">Dec 2023 – Aug 2024</div>
<div class="company-header">
<div class="company-logo">W</div>
<div class="experience-company">Wind Consulting</div>
</div>
</div>
<div class="card-body">
<h3 class="experience-title">Full Stack Engineer</h3>
<span class="experience-role">ERP Development</span>
<p class="experience-desc">
Developed a customized CRM system for travel management using a microservice architecture. Implemented core features for managing offers, prospects, trips, and sales representatives with integration to external APIs and messaging platforms.
</p>
<p class="experience-desc">
<strong>Project:</strong> Konouz ERP
</p>
<div class="experience-skills">
<span class="skill-tag"><i class="fab fa-java"></i> Java</span>
<span class="skill-tag"><i class="fas fa-leaf"></i> Spring Boot</span>
<span class="skill-tag"><i class="fab fa-angular"></i> Angular</span>
<span class="skill-tag"><i class="fas fa-cube"></i> Microservices</span>
<span class="skill-tag"><i class="fas fa-exchange-alt"></i> Kafka</span>
<span class="skill-tag"><i class="fas fa-robot"></i> Meta API Integration</span>
<span class="skill-tag"><i class="fas fa-paperclip"></i> Webhooks</span>
</div>
</div>
</div>
<!-- Wind ERP (Multi-tenant) -->
<div class="experience-card">
<div class="card-header">
<div class="experience-date">Jan 2023 – Nov 2023</div>
<div class="company-header">
<div class="company-logo">W</div>
<div class="experience-company">Wind Consulting</div>
</div>
</div>
<div class="card-body">
<h3 class="experience-title">Full Stack Engineer</h3>
<span class="experience-role">Multi-tenant Solutions</span>
<p class="experience-desc">
Designed and developed backend services for a multi-tenant ERP application. Implemented modular architecture allowing customization for different business verticals while maintaining code reusability and scalability.
</p>
<p class="experience-desc">
<strong>Project:</strong> Wind ERP (Multi-tenant Solution)
</p>
<div class="experience-skills">
<span class="skill-tag"><i class="fab fa-java"></i> Java</span>
<span class="skill-tag"><i class="fas fa-leaf"></i> Spring Boot</span>
<span class="skill-tag"><i class="fas fa-cube"></i> Microservices</span>
<span class="skill-tag"><i class="fab fa-docker"></i> Docker</span>
<span class="skill-tag"><i class="fas fa-exchange-alt"></i> Kafka</span>
<span class="skill-tag"><i class="fas fa-shield-alt"></i> Spring Security</span>
<span class="skill-tag"><i class="fab fa-git"></i> Git</span>
<span class="skill-tag"><i class="fab fa-aws"></i> AWS Web Services</span>
</div>
</div>
</div>
<!-- Wind ERP (User Management) -->
<div class="experience-card">
<div class="card-header">
<div class="experience-date">Jan 2023 – July 2023</div>
<div class="company-header">
<div class="company-logo">W</div>
<div class="experience-company">Wind Consulting</div>
</div>
</div>
<div class="card-body">
<h3 class="experience-title">Software Engineer Intern</h3>
<span class="experience-role">User Management Systems</span>
<p class="experience-desc">
Developed a specialized user management module including advanced features such as meeting scheduling, video conferencing integration, and internal chat functionality as part of my final year engineering project.
</p>
<p class="experience-desc">
<strong>Project:</strong> Wind ERP - User Management Module
</p>
<div class="experience-skills">
<span class="skill-tag"><i class="fab fa-angular"></i> Angular</span>
<span class="skill-tag"><i class="fas fa-leaf"></i> Spring Boot</span>
<span class="skill-tag"><i class="fas fa-shield-alt"></i> Spring Security</span>
<span class="skill-tag"><i class="fab fa-google"></i> Google API</span>
<span class="skill-tag"><i class="fas fa-comments"></i> WebSocket</span>
</div>
</div>
</div>
</div>
</details>
<!-- Swatek Internship -->
<details class="company-group">
<summary class="company-summary">
<div class="company-summary-info">
<div class="company-logo">S</div>
<div class="company-summary-text">
<h3>Swatek</h3>
<p>1 role - Jun 2022 - Aug 2022</p>
</div>
</div>
<i class="fas fa-chevron-down company-toggle-icon"></i>
</summary>
<div class="company-jobs">
<div class="experience-card">
<div class="card-header">
<div class="experience-date">June 2022 – Aug 2022</div>
<div class="company-header">
<div class="company-logo">S</div>
<div class="experience-company">Swatek</div>
</div>
</div>
<div class="card-body">
<h3 class="experience-title">Engineering Intern</h3>
<span class="experience-role">Social Networking Platform</span>
<p class="experience-desc">
Designed and developed core features for a social networking platform enabling municipalities to interact with citizens through posts, comments, and community management tools.
</p>
<p class="experience-desc">
<strong>Project:</strong> Social Networking Platform for Municipalities
</p>
<div class="experience-skills">
<span class="skill-tag"><i class="fab fa-angular"></i> Angular</span>
<span class="skill-tag"><i class="fas fa-leaf"></i> Spring Boot</span>
<span class="skill-tag"><i class="fas fa-shield-alt"></i> Spring Security</span>
<span class="skill-tag"><i class="fab fa-angular"></i> Angular Material</span>
</div>
</div>
</div>
</details>
</div>
</div>
</section>
<!-- Projects Section - Separate section -->
<section id="projects">
<div class="container">
<h2 class="section-title">Project Portfolio</h2>
<p class="section-description">Explore my project portfolio, showcasing my expertise in developing enterprise solutions with Java and Angular technologies.</p>
<div class="projects-grid">
<div class="project-card">
<div class="project-img color1">
<i class="fas fa-hospital"></i>
</div>
<div class="project-content">
<h3 class="project-title">Hospitals Management Platform</h3>
<span class="project-date">Aug 2025 – Present</span>
<p class="project-desc">
Development of a platform dedicated to Tunisian hospitals for centralized management of stocks, medical items, equipment, and services. The solution improves traceability, resource optimization, and operational monitoring (inventory, maintenance, transfers, contracts, and interventions).
</p>
<div class="project-tags">
<span class="project-tag java"><i class="fab fa-java"></i> Java</span>
<span class="project-tag"><i class="fas fa-cogs"></i> JHipster</span>
<span class="project-tag"><i class="fab fa-bitbucket"></i> Bitbucket</span>
<span class="project-tag microservices"><i class="fas fa-cube"></i> Microservices</span>
<span class="project-tag angular"><i class="fab fa-angular"></i> Angular</span>
<span class="project-tag postgresql"><i class="fas fa-database"></i> PostgreSQL</span>
<span class="project-tag elasticsearch"><i class="fas fa-search"></i> Elasticsearch</span>
<span class="project-tag kafka"><i class="fas fa-exchange-alt"></i> Kafka</span>
<span class="project-tag"><i class="fas fa-comments"></i> WebSocket</span>
<span class="project-tag"><i class="fas fa-cloud"></i> MinIO</span>
<span class="project-tag"><i class="fas fa-chart-line"></i> Grafana</span>
<span class="project-tag"><i class="fas fa-bug"></i> SonarQube</span>
<span class="project-tag"><i class="fas fa-key"></i> Keycloak</span>
</div>
</div>
</div>
<div class="project-card">
<div class="project-img color2">
<i class="fas fa-heartbeat"></i>
</div>
<div class="project-content">
<h3 class="project-title">Dubai Now Application</h3>
<span class="project-date">Apr 2025 – Aug 2025</span>
<p class="project-desc">
Backend services for a health module in the Dubai Now application, focused on generating digital questionnaires for parents and medical reports for health professionals, integrated with Dubai Health Authority systems.
</p>
<div class="project-tags">
<span class="project-tag java"><i class="fab fa-java"></i> Java</span>
<span class="project-tag spring"><i class="fas fa-leaf"></i> Spring Boot</span>
<span class="project-tag"><i class="fas fa-shield-alt"></i> Data Security</span>
<span class="project-tag"><i class="fas fa-tasks"></i> Agile (Scrum)</span>
</div>
</div>
</div>
<div class="project-card">
<div class="project-img color3">
<i class="fas fa-car"></i>
</div>
<div class="project-content">
<h3 class="project-title">Autopal</h3>
<span class="project-date">Sep 2024 – Mar 2025</span>
<p class="project-desc">
Mobile application dedicated to vehicle management, covering comprehensive features for users, partners, vehicles, towing, insurance, and payments.
</p>
<div class="project-tags">
<span class="project-tag java"><i class="fab fa-java"></i> Java</span>
<span class="project-tag spring"><i class="fas fa-leaf"></i> Spring Boot</span>
<span class="project-tag angular"><i class="fab fa-angular"></i> Angular</span>
<span class="project-tag"><i class="fas fa-mobile-alt"></i> Mobile App</span>
<span class="project-tag rabbitmq"><i class="fas fa-exchange-alt"></i> RabbitMQ</span>
<span class="project-tag"><i class="fas fa-cogs"></i> REST APIs</span>
<span class="project-tag security"><i class="fas fa-shield-alt"></i> Spring Security</span>
<span class="project-tag docker"><i class="fab fa-docker"></i> Docker</span>
<span class="project-tag kafka"><i class="fas fa-exchange-alt"></i> Kafka</span>

</div>
</div>
</div>
<div class="project-card">
<div class="project-img color4">
<i class="fas fa-database"></i>
</div>
<div class="project-content">
<h3 class="project-title">Log Management System</h3>
<span class="project-date">2024</span>
<p class="project-desc">
Development of a centralized log management system for monitoring and analyzing logs across microservices with real-time capabilities.
</p>
<div class="project-tags">
<span class="project-tag log4j"><i class="fas fa-bug"></i> Log4j</span>
<span class="project-tag kafka"><i class="fas fa-exchange-alt"></i> Kafka</span>
<span class="project-tag logstash"><i class="fas fa-filter"></i> Logstash</span>
<span class="project-tag"><i class="fas fa-chart-bar"></i> Kibana</span>
<span class="project-tag elasticsearch"><i class="fas fa-search"></i> Elasticsearch</span>
</div>
</div>
</div>
<div class="project-card">
<div class="project-img color5">
<i class="fas fa-route"></i>
</div>
<div class="project-content">
<h3 class="project-title">Konouz ERP</h3>
<span class="project-date">Dec 2023 – Aug 2024</span>
<p class="project-desc">
Customized CRM system for travel management with efficient management of offers, prospects, trips, and sales representatives, based on a microserver architecture.
</p>
<div class="project-tags">
<span class="project-tag java"><i class="fab fa-java"></i> Java</span>
<span class="project-tag spring"><i class="fas fa-leaf"></i> Spring Boot</span>
<span class="project-tag angular"><i class="fab fa-angular"></i> Angular</span>
<span class="project-tag microservices"><i class="fas fa-cube"></i> Microservices</span>
<span class="project-tag kafka"><i class="fas fa-exchange-alt"></i> Kafka</span>
<span class="project-tag rabbitmq"><i class="fas fa-exchange-alt"></i> RabbitMQ</span>
<span class="project-tag"><i class="fab fa-file-alt"></i> Alfresco</span>
<span class="project-tag"><i class="fas fa-file-pdf"></i> Jasper PDF</span>
<span class="project-tag docker"><i class="fab fa-docker"></i> Docker</span>
<span class="project-tag"><i class="fas fa-robot"></i> Meta API</span>
<span class="project-tag"><i class="fas fa-paperclip"></i> Meta Webhook</span>
</div>
</div>
</div>
<div class="project-card">
<div class="project-img color6">
<i class="fas fa-building"></i>
</div>
<div class="project-content">
<h3 class="project-title">Wind ERP</h3>
<span class="project-date">Jan 2023 – Nov 2023</span>
<p class="project-desc">
Multi-tenant ERP application designed to meet business management needs in a modular and scalable manner with real-time collaboration features.
</p>
<div class="project-tags">
<span class="project-tag java"><i class="fab fa-java"></i> Java</span>
<span class="project-tag spring"><i class="fas fa-leaf"></i> Spring Boot</span>
<span class="project-tag angular"><i class="fab fa-angular"></i> Angular</span>
<span class="project-tag microservices"><i class="fas fa-cube"></i> Microservices</span>
<span class="project-tag kafka"><i class="fas fa-exchange-alt"></i> Kafka</span>
<span class="project-tag rabbitmq"><i class="fas fa-exchange-alt"></i> RabbitMQ</span>
<span class="project-tag"><i class="fab fa-file-alt"></i> Alfresco</span>
<span class="project-tag"><i class="fas fa-file-pdf"></i> Jasper PDF</span>
<span class="project-tag docker"><i class="fab fa-docker"></i> Docker</span>
<span class="project-tag aws"><i class="fab fa-aws"></i> AWS Web Services</span>
</div>
</div>
</div>
</div>
</div>
</section>
<!-- Skills - New classification -->
<section id="skills">
<div class="container">
<h2 class="section-title">Technical Skills</h2>
<p class="section-description">My technical expertise spans across multiple domains, with a strong focus on Java ecosystem and modern web technologies.</p>
<div class="skills-grid">
<div class="skill-column">
<h3><i class="fas fa-server"></i> Backend Development</h3>
<div class="skill-fleet">
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:openjdk.svg?color=%23f89820" alt="Java logo"> Java</span>
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:springboot.svg?color=%236db33f" alt="Spring Boot logo"> Spring Boot</span>
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:kubernetes.svg?color=%23326ce5" alt="Microservices logo"> Microservices</span>
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:postman.svg?color=%23ff6c37" alt="REST APIs logo"> REST APIs</span>
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:hibernate.svg?color=%2359666c" alt="Hibernate logo"> Hibernate</span>
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:springsecurity.svg?color=%236db33f" alt="Spring Security logo"> Spring Security</span>
</div>
</div>
<div class="skill-column">
<h3><i class="fas fa-laptop-code"></i> Frontend Development</h3>
<div class="skill-fleet">
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:angular.svg?color=%23dd0031" alt="Angular logo"> Angular</span>
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:tailwindcss.svg?color=%2306b6d4" alt="Tailwind CSS logo"> Tailwind CSS</span>
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:socketdotio.svg?color=%23010101" alt="WebSocket logo"> WebSocket</span>
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:google.svg?color=%234285f4" alt="Google API logo"> Google API</span>
<span class="skill-ship"><img src="https://www.vectorlogo.zone/logos/alfresco/alfresco-icon.svg" alt="Alfresco logo"> Alfresco API</span>
</div>
</div>
<div class="skill-column">
<h3><i class="fas fa-database"></i> Databases &amp; Messaging</h3>
<div class="skill-fleet">
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:postgresql.svg?color=%234169e1" alt="PostgreSQL logo"> PostgreSQL</span>
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:elasticsearch.svg?color=%23005571" alt="Elasticsearch logo"> Elasticsearch</span>
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:apachekafka.svg?color=%23231f20" alt="Kafka logo"> Kafka</span>
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:rabbitmq.svg?color=%23ff6600" alt="RabbitMQ logo"> RabbitMQ</span>
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:minio.svg?color=%23c72e49" alt="MinIO logo"> MinIO</span>
</div>
</div>
<div class="skill-column">
<h3><i class="fas fa-tools"></i> DevOps &amp; Tools</h3>
<div class="skill-fleet">
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:docker.svg?color=%232496ed" alt="Docker logo"> Docker</span>
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:git.svg?color=%23f05032" alt="Git logo"> Git</span>
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:bitbucket.svg?color=%230052cc" alt="Bitbucket logo"> Bitbucket</span>
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:jira.svg?color=%230052cc" alt="Jira logo"> Jira</span>
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:jenkins.svg?color=%23d24939" alt="Jenkins logo"> Jenkins</span>
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:grafana.svg?color=%23f46800" alt="Grafana logo"> Grafana</span>
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:sonarqube.svg?color=%234e9bcd" alt="SonarQube logo"> SonarQube</span>
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:keycloak.svg?color=%234d4d4d" alt="Keycloak logo"> Keycloak</span>
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:scrumalliance.svg?color=%23009cde" alt="Agile Scrum logo"> Agile/Scrum</span>
<span class="skill-ship"><img src="https://api.iconify.design/simple-icons:amazonaws.svg?color=%23ff9900" alt="AWS logo"> AWS Web Services</span>
</div>
</div>
</div>
</div>
</section>
<!-- Education -->
<section id="education">
<div class="container">
<h2 class="section-title">Education</h2>
<p class="section-description">My academic journey has provided me with a strong foundation in engineering principles and specialized software development skills.</p>
<div class="education-compact">
<details class="edu-row">
<summary class="edu-row-main">
<div class="edu-side">
<span class="edu-index">01</span>
<div class="school-logo">
<a href="https://www.esprit.tn" target="_blank" rel="noopener noreferrer">
<img src="images/esprit-logo.png" alt="ESPRIT Logo">
</a>
</div>
</div>
<div class="edu-main-text">
<div class="edu-degree">Computer Engineer specialized in Software Engineering</div>
<a class="edu-school-link" href="https://www.esprit.tn" target="_blank" rel="noopener noreferrer">
Private Higher School of Engineering and Technology (Esprit)
</a>
</div>
<div class="edu-actions">
<div class="edu-period"><i class="far fa-calendar-alt"></i> Sep 2020 – Oct 2023</div>
<span class="edu-toggle"><i class="fas fa-chevron-down"></i></span>
</div>
</summary>
<div class="edu-row-extra">
<p class="edu-desc">
Comprehensive engineering program focused on software development, system architecture, and modern engineering practices. Specialization in enterprise application development with Java ecosystem and modern web technologies.
</p>
<div class="tech-tags">
<span class="tech-tag"><i class="fas fa-building"></i> Software Architecture</span>
<span class="tech-tag"><i class="fas fa-project-diagram"></i> System Design</span>
<span class="tech-tag"><i class="fas fa-server"></i> Enterprise Applications</span>
<span class="tech-tag"><i class="fas fa-tasks"></i> Agile Methodologies</span>
<span class="tech-tag"><i class="fas fa-cloud"></i> Cloud Computing</span>
</div>
</div>
</details>
<details class="edu-row">
<summary class="edu-row-main">
<div class="edu-side">
<span class="edu-index">02</span>
<div class="school-logo">
<a href="https://issatso.rnu.tn/" target="_blank" rel="noopener noreferrer">
<img src="images/issat-logo.jpg" alt="ISSAT Sousse Logo">
</a>
</div>
</div>
<div class="edu-main-text">
<div class="edu-degree">Applied Bachelor Degree in Electromechanics</div>
<a class="edu-school-link" href="https://issatso.rnu.tn/" target="_blank" rel="noopener noreferrer">
Higher Institute of Applied Sciences and Technologies Sousse (ISSAT)
</a>
</div>
<div class="edu-actions">
<div class="edu-period"><i class="far fa-calendar-alt"></i> Sep 2017 – Oct 2020</div>
<span class="edu-toggle"><i class="fas fa-chevron-down"></i></span>
</div>
</summary>
<div class="edu-row-extra">
<p class="edu-desc">
Foundation in engineering principles with practical applications in electromechanical systems. This background provides me with a unique perspective on integrating software solutions with physical systems and understanding hardware constraints in application development.
</p>
<div class="tech-tags">
<span class="tech-tag"><i class="fas fa-cogs"></i> Engineering Fundamentals</span>
<span class="tech-tag"><i class="fas fa-network-wired"></i> Systems Integration</span>
<span class="tech-tag"><i class="fas fa-brain"></i> Technical Problem Solving</span>
</div>
</div>
</details>
</div>
</div>
</section>
<!-- Languages -->
<section id="languages">
<div class="container">
<h2 class="section-title">Languages</h2>
<p class="section-description">I am proficient in multiple languages, enabling effective communication in diverse professional environments.</p>
<div class="languages-intel">
<article class="language-node native">
<div class="language-top">
<div class="language-id">
<span class="language-pin"></span>
<h3 class="language-name-title">Arabic</h3>
</div>
<span class="language-level-pill">Native Proficiency</span>
</div>
<div class="language-matrix">
<div class="lang-metric">
<div class="metric-head"><span>Speaking</span><span>Excellent</span></div>
<div class="metric-bar"><span style="--value:100%;"></span></div>
</div>
<div class="lang-metric">
<div class="metric-head"><span>Reading</span><span>Excellent</span></div>
<div class="metric-bar"><span style="--value:100%;"></span></div>
</div>
<div class="lang-metric">
<div class="metric-head"><span>Writing</span><span>Excellent</span></div>
<div class="metric-bar"><span style="--value:100%;"></span></div>
</div>
</div>
</article>
<article class="language-node intermediate">
<div class="language-top">
<div class="language-id">
<span class="language-pin"></span>
<h3 class="language-name-title">English</h3>
</div>
<span class="language-level-pill">Intermediate Proficiency</span>
</div>
<div class="language-matrix">
<div class="lang-metric">
<div class="metric-head"><span>Speaking</span><span>Good</span></div>
<div class="metric-bar"><span style="--value:72%;"></span></div>
</div>
<div class="lang-metric">
<div class="metric-head"><span>Reading</span><span>Good</span></div>
<div class="metric-bar"><span style="--value:78%;"></span></div>
</div>
<div class="lang-metric">
<div class="metric-head"><span>Writing</span><span>Intermediate</span></div>
<div class="metric-bar"><span style="--value:68%;"></span></div>
</div>
</div>
</article>
<article class="language-node intermediate">
<div class="language-top">
<div class="language-id">
<span class="language-pin"></span>
<h3 class="language-name-title">French</h3>
</div>
<span class="language-level-pill">Intermediate Proficiency</span>
</div>
<div class="language-matrix">
<div class="lang-metric">
<div class="metric-head"><span>Speaking</span><span>Good</span></div>
<div class="metric-bar"><span style="--value:70%;"></span></div>
</div>
<div class="lang-metric">
<div class="metric-head"><span>Reading</span><span>Good</span></div>
<div class="metric-bar"><span style="--value:76%;"></span></div>
</div>
<div class="lang-metric">
<div class="metric-head"><span>Writing</span><span>Intermediate</span></div>
<div class="metric-bar"><span style="--value:66%;"></span></div>
</div>
</div>
</article>
</div>
</div>
</div>
</section>
<!-- Hobbies Section -->
<section id="hobbies">
<div class="container">
<h2 class="section-title">Personal Interests</h2>
<p class="section-description">Beyond coding, I enjoy activities that stimulate creativity, physical well-being, and continuous learning.</p>
<div class="hobbies-grid">
<div class="hobby-card chess">
<div class="hobby-icon">
<i class="fas fa-chess"></i>
</div>
<h3>Strategic Games</h3>
<p>Chess and strategy games sharpen decision-making, anticipation, and problem decomposition.</p>
<span class="hobby-note"><i class="fas fa-lightbulb"></i> Better system thinking</span>
</div>
<div class="hobby-card outdoor">
<div class="hobby-icon">
<i class="fas fa-hiking"></i>
</div>
<h3>Outdoor Activities</h3>
<p>Outdoor activities help me reset, improve focus, and return to work with more clarity and energy.</p>
<span class="hobby-note"><i class="fas fa-heart-pulse"></i> Better focus and balance</span>
</div>
<div class="hobby-card learning">
<div class="hobby-icon">
<i class="fas fa-book-open"></i>
</div>
<h3>Continuous Learning</h3>
<p>I learn continuously through technical books, blogs, and hands-on experiments with new tools.</p>
<span class="hobby-note"><i class="fas fa-rocket"></i> Always improving</span>
</div>
<div class="hobby-card music">
<div class="hobby-icon">
<i class="fas fa-music"></i>
</div>
<h3>Music</h3>
<p>Music helps me enter deep focus mode during coding and keeps long work sessions more enjoyable.</p>
<span class="hobby-note"><i class="fas fa-wave-square"></i> Better flow state</span>
</div>
</div>
</div>
</section>
<!-- Contact -->
<section id="contact">
<div class="container">
<h2 class="section-title">Get In Touch</h2>
<p class="section-description">Have a project in mind or want to discuss potential opportunities? Feel free to reach out!</p>
<div class="contact-container">
<div class="contact-details">
<div class="contact-method email">
<div class="contact-icon">
<i class="fas fa-envelope"></i>
</div>
<div class="contact-text">
<h3>Email</h3>
<p>lotfi.hmida01@gmail.com</p>
</div>
</div>
<div class="contact-method phone">
<div class="contact-icon">
<i class="fas fa-phone"></i>
</div>
<div class="contact-text">
<h3>Phone</h3>
<p>+216 25 622 677</p>
</div>
</div>
<div class="contact-method whatsapp">
<div class="contact-icon">
<i class="fab fa-whatsapp"></i>
</div>
<div class="contact-text">
<h3>WhatsApp</h3>
<p>+216 25 622 677</p>
</div>
</div>
<div class="contact-method location">
<div class="contact-icon">
<i class="fas fa-map-marker-alt"></i>
</div>
<div class="contact-text">
<h3>Location</h3>
<p>Tunis, Tunisia</p>
</div>
</div>
<div class="contact-method">
<div class="contact-icon">
<i class="fas fa-clock"></i>
</div>
<div class="contact-text">
<h3>Working Hours</h3>
<p>Monday - Friday: 9:00 AM - 6:00 PM</p>
<p>Weekends: By appointment only</p>
</div>
</div>
<div class="map-container">
<iframe id="googleMap" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3194.935747157237!2d10.180082176132438!3d36.80650847217167!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x12fd33e6e4b3e7c1%3A0xc2f6e3e4e4e4e4e4!2sTunis%2C%20Tunisia!5e0!3m2!1sen!2sus!4v1710000000000!5m2!1sen!2sus" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade" title="Tunis map"></iframe>
</div>
</div>
<div class="contact-form">
<form id="contactForm">
<div class="form-group">
<label for="name">Your Name</label>
<input type="text" id="name" class="form-control" placeholder="Enter your name" required>
</div>
<div class="form-group">
<label for="email">Your Email</label>
<input type="email" id="email" class="form-control" placeholder="Enter your email" required>
</div>
<div class="form-group">
<label for="subject">Subject</label>
<input type="text" id="subject" class="form-control" placeholder="What is this regarding?" required>
</div>
<div class="form-group">
<label for="message">Your Message</label>
<textarea id="message" class="form-control" placeholder="Type your message here..." required></textarea>
</div>
<button type="submit" class="submit-btn">Send Message</button>
</form>
</div>
</div>
</div>
</section>
<!-- Footer -->
<footer>
<div class="footer-starry-background">
<div class="nebula"></div>
<div class="nebula"></div>
<div class="nebula"></div>
</div>
<canvas id="footerNetwork" class="network-canvas footer-network-canvas"></canvas>
<div class="container">
<div class="footer-content">
<div class="footer-logo">Lotfi Hmida</div>
<p>Full Stack Java/Angular Engineer </p>
<div class="socials-footer">
<a href="https://github.com/lotfi2020-2021" target="_blank" class="social-link github"><i class="fab fa-github"></i></a>
<a href="https://www.linkedin.com/in/lotfi-hmida" target="_blank" class="social-link linkedin"><i class="fab fa-linkedin-in"></i></a>
<a href="https://www.instagram.com/lotfi_hmeda" target="_blank" class="social-link instagram"><i class="fab fa-instagram"></i></a>
<a href="https://www.facebook.com/lot.fi.801148" target="_blank" class="social-link facebook"><i class="fab fa-facebook-f"></i></a>
<a href="https://wa.me/21625622677" target="_blank" class="social-link whatsapp"><i class="fab fa-whatsapp"></i></a>
</div>
<div class="footer-links">
<a href="#hero">Home</a>
<a href="#experience">Experience</a>
<a href="#projects">Projects</a>
<a href="#skills">Skills</a>
<a href="#education">Education</a>
<a href="#contact">Contact</a>
</div>
<div class="copyright">
© 2026 Lotfi Hmida — All Rights Reserved
</div>
</div>
</div>
</footer>
<script>
// Scroll progress indicator
window.addEventListener('scroll', function() {
const scrollProgress = document.getElementById('scroll-progress');
const scrollTop = document.documentElement.scrollTop;
const scrollHeight = document.documentElement.scrollHeight - document.documentElement.clientHeight;
const scrolled = (scrollTop / scrollHeight) * 100;
scrollProgress.style.width = scrolled + '%';
});
// Section animations
document.addEventListener('DOMContentLoaded', function() {
const themeToggle = document.getElementById('themeToggle');
const mobileThemeToggle = document.getElementById('mobileThemeToggle');
const updateThemeButtons = (isDarkMode) => {
if (themeToggle) {
themeToggle.innerHTML = isDarkMode
? '<i class="fas fa-sun"></i><span>Mode normal</span>'
: '<i class="fas fa-moon"></i><span>Mode sombre</span>';
themeToggle.setAttribute('aria-label', isDarkMode ? 'Activer mode normal' : 'Activer mode sombre');
}
if (mobileThemeToggle) {
mobileThemeToggle.innerHTML = isDarkMode
? '<i class="fas fa-sun"></i> Mode normal'
: '<i class="fas fa-moon"></i> Mode sombre';
mobileThemeToggle.setAttribute('aria-label', isDarkMode ? 'Activer mode normal' : 'Activer mode sombre');
}
};
const applyTheme = (theme) => {
const isDarkMode = theme === 'dark';
document.body.classList.toggle('dark-mode', isDarkMode);
updateThemeButtons(isDarkMode);
};
const savedTheme = localStorage.getItem('theme');
applyTheme(savedTheme || 'light');
if (themeToggle) {
themeToggle.addEventListener('click', function() {
const nextTheme = document.body.classList.contains('dark-mode') ? 'light' : 'dark';
applyTheme(nextTheme);
localStorage.setItem('theme', nextTheme);
});
}
if (mobileThemeToggle) {
mobileThemeToggle.addEventListener('click', function() {
const nextTheme = document.body.classList.contains('dark-mode') ? 'light' : 'dark';
applyTheme(nextTheme);
localStorage.setItem('theme', nextTheme);
});
}
const profileImage = document.getElementById('profileImg');
if (profileImage) {
const zoomOverlay = document.createElement('div');
zoomOverlay.className = 'image-zoom-overlay';
zoomOverlay.setAttribute('aria-hidden', 'true');
zoomOverlay.innerHTML = '<img class="image-zoom-content" alt="Photo de profil agrandie">';
document.body.appendChild(zoomOverlay);
const zoomImage = zoomOverlay.querySelector('.image-zoom-content');
const getImageUrl = (element) => {
const bg = window.getComputedStyle(element).backgroundImage;
const match = /url\((['"]?)(.*?)\1\)/.exec(bg);
return match ? match[2] : '';
};
const openZoom = () => {
const src = getImageUrl(profileImage);
if (!src) return;
const probe = new Image();
probe.onload = () => {
const safeWidth = Math.min(probe.naturalWidth || 400, window.innerWidth * 0.92);
const safeHeight = Math.min(probe.naturalHeight || 400, window.innerHeight * 0.92);
zoomImage.style.width = `${safeWidth}px`;
zoomImage.style.height = `${safeHeight}px`;
zoomImage.src = src;
zoomOverlay.classList.add('open');
zoomOverlay.setAttribute('aria-hidden', 'false');
document.body.classList.add('no-scroll');
};
probe.onerror = () => {
zoomImage.style.width = 'min(92vw, 400px)';
zoomImage.style.height = 'auto';
zoomImage.src = src;
zoomOverlay.classList.add('open');
zoomOverlay.setAttribute('aria-hidden', 'false');
document.body.classList.add('no-scroll');
};
probe.src = src;
};
const closeZoom = () => {
zoomOverlay.classList.remove('open');
zoomOverlay.setAttribute('aria-hidden', 'true');
document.body.classList.remove('no-scroll');
};
profileImage.addEventListener('click', openZoom);
profileImage.addEventListener('keydown', (event) => {
if (event.key === 'Enter' || event.key === ' ') {
event.preventDefault();
openZoom();
}
});
zoomOverlay.addEventListener('click', () => {
closeZoom();
});
document.addEventListener('keydown', (event) => {
if (event.key === 'Escape' && zoomOverlay.classList.contains('open')) {
closeZoom();
}
});
}
// Section animations
const sections = document.querySelectorAll('section');
const sectionObserver = new IntersectionObserver((entries) => {
entries.forEach(entry => {
if (entry.isIntersecting) {
entry.target.classList.add('visible');
}
});
}, { threshold: 0.1 });
sections.forEach(section => {
sectionObserver.observe(section);
});
// Hero moving network background (nodes + links)
const heroNetworkCanvas = document.getElementById('heroNetwork');
if (heroNetworkCanvas) {
const ctx = heroNetworkCanvas.getContext('2d');
let nodes = [];
let networkWidth = 0;
let networkHeight = 0;
const prefersReducedMotion = window.matchMedia('(prefers-reduced-motion: reduce)').matches;
const createNodes = () => {
const baseCount = window.innerWidth < 768 ? 24 : 42;
nodes = Array.from({ length: baseCount }, () => ({
x: Math.random() * networkWidth,
y: Math.random() * networkHeight,
vx: (Math.random() - 0.5) * 0.25,
vy: (Math.random() - 0.5) * 0.25
}));
};
const resizeNetwork = () => {
const heroRect = document.getElementById('hero').getBoundingClientRect();
networkWidth = Math.max(1, Math.floor(heroRect.width));
networkHeight = Math.max(1, Math.floor(heroRect.height));
heroNetworkCanvas.width = networkWidth;
heroNetworkCanvas.height = networkHeight;
createNodes();
};
const drawNetwork = () => {
ctx.clearRect(0, 0, networkWidth, networkHeight);
for (let i = 0; i < nodes.length; i++) {
const a = nodes[i];
a.x += a.vx;
a.y += a.vy;
if (a.x <= 0 || a.x >= networkWidth) a.vx *= -1;
if (a.y <= 0 || a.y >= networkHeight) a.vy *= -1;
for (let j = i + 1; j < nodes.length; j++) {
const b = nodes[j];
const dx = a.x - b.x;
const dy = a.y - b.y;
const dist = Math.sqrt(dx * dx + dy * dy);
if (dist < 170) {
const alpha = 1 - dist / 170;
ctx.strokeStyle = `rgba(125, 211, 252, ${0.38 * alpha})`;
ctx.lineWidth = 1;
ctx.beginPath();
ctx.moveTo(a.x, a.y);
ctx.lineTo(b.x, b.y);
ctx.stroke();
}
}
ctx.fillStyle = 'rgba(96, 165, 250, 0.85)';
ctx.beginPath();
ctx.arc(a.x, a.y, 2.5, 0, Math.PI * 2);
ctx.fill();
}
if (!prefersReducedMotion) {
requestAnimationFrame(drawNetwork);
}
};
resizeNetwork();
if (!prefersReducedMotion) {
requestAnimationFrame(drawNetwork);
}
window.addEventListener('resize', resizeNetwork);
}
// Footer moving network background (same style as hero)
const footerNetworkCanvas = document.getElementById('footerNetwork');
if (footerNetworkCanvas) {
const footerCtx = footerNetworkCanvas.getContext('2d');
let footerNodes = [];
let footerWidth = 0;
let footerHeight = 0;
const prefersReducedMotionFooter = window.matchMedia('(prefers-reduced-motion: reduce)').matches;
const createFooterNodes = () => {
const baseCount = window.innerWidth < 768 ? 18 : 34;
footerNodes = Array.from({ length: baseCount }, () => ({
x: Math.random() * footerWidth,
y: Math.random() * footerHeight,
vx: (Math.random() - 0.5) * 0.22,
vy: (Math.random() - 0.5) * 0.22
}));
};
const resizeFooterNetwork = () => {
const footerRect = document.querySelector('footer').getBoundingClientRect();
footerWidth = Math.max(1, Math.floor(footerRect.width));
footerHeight = Math.max(1, Math.floor(footerRect.height));
footerNetworkCanvas.width = footerWidth;
footerNetworkCanvas.height = footerHeight;
createFooterNodes();
};
const drawFooterNetwork = () => {
footerCtx.clearRect(0, 0, footerWidth, footerHeight);
for (let i = 0; i < footerNodes.length; i++) {
const a = footerNodes[i];
a.x += a.vx;
a.y += a.vy;
if (a.x <= 0 || a.x >= footerWidth) a.vx *= -1;
if (a.y <= 0 || a.y >= footerHeight) a.vy *= -1;
for (let j = i + 1; j < footerNodes.length; j++) {
const b = footerNodes[j];
const dx = a.x - b.x;
const dy = a.y - b.y;
const dist = Math.sqrt(dx * dx + dy * dy);
if (dist < 160) {
const alpha = 1 - dist / 160;
footerCtx.strokeStyle = `rgba(125, 211, 252, ${0.34 * alpha})`;
footerCtx.lineWidth = 1;
footerCtx.beginPath();
footerCtx.moveTo(a.x, a.y);
footerCtx.lineTo(b.x, b.y);
footerCtx.stroke();
}
}
footerCtx.fillStyle = 'rgba(96, 165, 250, 0.8)';
footerCtx.beginPath();
footerCtx.arc(a.x, a.y, 2.2, 0, Math.PI * 2);
footerCtx.fill();
}
if (!prefersReducedMotionFooter) {
requestAnimationFrame(drawFooterNetwork);
}
};
resizeFooterNetwork();
if (!prefersReducedMotionFooter) {
requestAnimationFrame(drawFooterNetwork);
}
window.addEventListener('resize', resizeFooterNetwork);
}
// Replace Experience/Project skill tags with original logos
const si = (slug, color = '2563eb') => `https://api.iconify.design/simple-icons:${slug}.svg?color=%23${color}`;
const fallbackLogoMap = {
'SonarQube': 'https://www.vectorlogo.zone/logos/sonarqube/sonarqube-icon.svg',
'Alfresco': 'https://www.vectorlogo.zone/logos/alfresco/alfresco-icon.svg',
'Alfresco API': 'https://www.vectorlogo.zone/logos/alfresco/alfresco-icon.svg',
'AWS Web Services': 'https://www.vectorlogo.zone/logos/amazon_aws/amazon_aws-icon.svg'
};
const tagLogoMap = {
'Java': si('openjdk', 'f89820'),
'Angular': si('angular', 'dd0031'),
'Angular Material': si('angular', 'dd0031'),
'JHipster': si('jhipster', '3e8acc'),
'Spring Boot': si('springboot', '6db33f'),
'Spring Security': si('springsecurity', '6db33f'),
'Microservices': si('kubernetes', '326ce5'),
'REST APIs': si('postman', 'ff6c37'),
'PostgreSQL': si('postgresql', '4169e1'),
'Elasticsearch': si('elasticsearch', '005571'),
'Kafka': si('apachekafka', '231f20'),
'RabbitMQ': si('rabbitmq', 'ff6600'),
'WebSocket': si('socketdotio', '010101'),
'Docker': si('docker', '2496ed'),
'Git': si('git', 'f05032'),
'Bitbucket': si('bitbucket', '0052cc'),
'AWS Web Services': si('amazonaws', 'ff9900'),
'Google API': si('google', '4285f4'),
'MinIO': si('minio', 'c72e49'),
'Grafana': si('grafana', 'f46800'),
'SonarQube': si('sonarqube', '4e9bcd'),
'Keycloak': si('keycloak', '4d4d4d'),
'Log4j': si('apache', 'd22128'),
'Logstash': si('logstash', '005571'),
'Kibana': si('kibana', '005571'),
'Alfresco': 'https://www.vectorlogo.zone/logos/alfresco/alfresco-icon.svg',
'Alfresco API': 'https://www.vectorlogo.zone/logos/alfresco/alfresco-icon.svg',
'Jasper PDF': si('adobeacrobatreader', 'ec1c24'),
'Meta API': si('meta', '0467df'),
'Meta API Integration': si('meta', '0467df'),
'Meta Webhook': si('meta', '0467df'),
'Webhooks': si('webhooks', '6a3df0'),
'Mobile App': si('android', '3ddc84'),
'Mobile Integration': si('android', '3ddc84'),
'Agile/Scrum': si('scrumalliance', '009cde'),
'Agile (Scrum)': si('scrumalliance', '009cde')
};
const tagColorMap = {
'Java': '#f89820',
'Angular': '#dd0031',
'Angular Material': '#dd0031',
'JHipster': '#3e8acc',
'Spring Boot': '#6db33f',
'Spring Security': '#6db33f',
'Microservices': '#326ce5',
'REST APIs': '#ff6c37',
'PostgreSQL': '#4169e1',
'Elasticsearch': '#005571',
'Kafka': '#231f20',
'RabbitMQ': '#ff6600',
'WebSocket': '#010101',
'Docker': '#2496ed',
'Git': '#f05032',
'Bitbucket': '#0052cc',
'AWS Web Services': '#ff9900',
'Google API': '#4285f4',
'MinIO': '#c72e49',
'Grafana': '#f46800',
'SonarQube': '#4e9bcd',
'Keycloak': '#4d4d4d',
'Log4j': '#d22128',
'Logstash': '#005571',
'Kibana': '#005571',
'Alfresco': '#39b54a',
'Alfresco API': '#39b54a',
'Jasper PDF': '#ec1c24',
'Meta API': '#0467df',
'Meta API Integration': '#0467df',
'Meta Webhook': '#0467df',
'Webhooks': '#6a3df0',
'Mobile App': '#3ddc84',
'Mobile Integration': '#3ddc84',
'Agile/Scrum': '#009cde',
'Agile (Scrum)': '#009cde'
};
const hexToRgba = (hex, alpha) => {
const clean = hex.replace('#', '');
const full = clean.length === 3 ? clean.split('').map((c) => c + c).join('') : clean;
const n = parseInt(full, 16);
const r = (n >> 16) & 255;
const g = (n >> 8) & 255;
const b = n & 255;
return `rgba(${r}, ${g}, ${b}, ${alpha})`;
};
// Ensure Skills section uses the same colored original logos
document.querySelectorAll('#skills .skill-ship').forEach((ship) => {
const label = ship.textContent.replace(/\s+/g, ' ').trim();
const logoSrc = tagLogoMap[label];
const img = ship.querySelector('img');
if (!img || !logoSrc) return;
img.src = logoSrc;
img.referrerPolicy = 'no-referrer';
img.onerror = () => {
const fallback = fallbackLogoMap[label];
if (fallback && img.src !== fallback) {
img.src = fallback;
}
};
});
document.querySelectorAll('.skill-tag, .project-tag').forEach(tag => {
const label = tag.textContent.replace(/\s+/g, ' ').trim();
const logoSrc = tagLogoMap[label];
const brand = tagColorMap[label];
if (!logoSrc || tag.querySelector('img.tag-logo')) return;
const img = document.createElement('img');
img.className = 'tag-logo';
img.src = logoSrc;
img.alt = `${label} logo`;
img.loading = 'lazy';
img.referrerPolicy = 'no-referrer';
img.dataset.logoLabel = label;
img.onerror = () => {
const fallback = fallbackLogoMap[label];
if (fallback && img.src !== fallback) {
img.src = fallback;
return;
}
img.remove();
tag.classList.remove('has-logo');
};
tag.classList.add('has-logo');
tag.prepend(img);
if (brand) {
tag.style.color = '#1f2937';
tag.style.borderColor = hexToRgba(brand, 0.35);
tag.style.backgroundColor = 'transparent';
}
});
document.querySelectorAll('#skills .skill-ship img').forEach((img) => {
const label = img.parentElement.textContent.replace(/\s+/g, ' ').trim();
img.onerror = () => {
const fallback = fallbackLogoMap[label];
if (fallback && img.src !== fallback) {
img.src = fallback;
}
};
});
// Enhanced Navbar animations - hide/show based on scroll direction
let lastScrollTop = 0;
const navbar = document.getElementById('navbar');
const threshold = 50; // Minimum scroll distance before hiding/showing nav
window.addEventListener('scroll', function() {
const scrollTop = window.pageYOffset || document.documentElement.scrollTop;
// Update scroll direction indicator
if (scrollTop > lastScrollTop && scrollTop > threshold) {
// Scrolling down - hide navbar
navbar.classList.remove('scrolled');
} else if (scrollTop < lastScrollTop) {
// Scrolling up - show navbar
navbar.classList.remove('hidden');
if (scrollTop > 100) {
navbar.classList.add('scrolled');
} else {
navbar.classList.remove('scrolled');
}
}
lastScrollTop = scrollTop <= 0 ? 0 : scrollTop; // For Mobile or negative scrolling
// Active nav link based on scroll position
let currentSection = '';
sections.forEach(section => {
const sectionTop = section.offsetTop - 100;
const sectionHeight = section.clientHeight;
if (pageYOffset >= sectionTop && pageYOffset < sectionTop + sectionHeight) {
currentSection = section.getAttribute('id');
}
});
const navLinks = document.querySelectorAll('.nav-link');
navLinks.forEach(link => {
link.classList.remove('active');
if (link.getAttribute('href').substring(1) === currentSection) {
link.classList.add('active');
}
});
});
// Smooth scrolling for anchor links
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
anchor.addEventListener('click', function(e) {
e.preventDefault();
const targetId = this.getAttribute('href');
if (targetId === '#') return;
const targetElement = document.querySelector(targetId);
if (targetElement) {
// Close mobile menu if open
const mobileMenu = document.getElementById('mobileMenu');
if (mobileMenu && mobileMenu.style.display === 'block') {
mobileMenu.style.display = 'none';
document.getElementById('mobileToggle').innerHTML = '<i class="fas fa-bars"></i>';
}
window.scrollTo({
top: targetElement.offsetTop - 80,
behavior: 'smooth'
});
}
});
});
// Form submission with toast notification
const contactForm = document.getElementById('contactForm');
const successToast = document.getElementById('successToast');
const closeToast = document.getElementById('closeToast');
if (contactForm) {
contactForm.addEventListener('submit', function(e) {
e.preventDefault();
// Get form values
const name = document.getElementById('name').value;
const email = document.getElementById('email').value;
const subject = document.getElementById('subject').value;
const message = document.getElementById('message').value;
// Create a simple email link
const mailtoBody = `Name: ${name}\nEmail: ${email}\nMessage:\n${message}`;
const mailtoLink = `mailto:lotfi.hmida01@gmail.com?subject=${encodeURIComponent(subject)}&body=${encodeURIComponent(mailtoBody)}`;
window.location.href = mailtoLink;
// Show success toast notification
successToast.classList.add('show');
// Hide toast after 5 seconds
setTimeout(() => {
successToast.classList.remove('show');
}, 5000);
// Reset form
this.reset();
});
}
// Close toast manually
if (closeToast) {
closeToast.addEventListener('click', function() {
successToast.classList.remove('show');
});
}
// Mobile menu toggle
const mobileToggle = document.getElementById('mobileToggle');
const mobileMenu = document.getElementById('mobileMenu');
if (mobileToggle && mobileMenu) {
mobileToggle.addEventListener('click', function() {
if (mobileMenu.style.display === 'block') {
mobileMenu.style.display = 'none';
this.innerHTML = '<i class="fas fa-bars"></i>';
} else {
mobileMenu.style.display = 'block';
this.innerHTML = '<i class="fas fa-times"></i>';
}
});
}
// Close mobile menu when clicking a link
if (mobileMenu) {
const mobileLinks = mobileMenu.querySelectorAll('a');
mobileLinks.forEach(link => {
link.addEventListener('click', function() {
mobileMenu.style.display = 'none';
mobileToggle.innerHTML = '<i class="fas fa-bars"></i>';
});
});
}
// Add sparkle effect to buttons on hover
const allButtons = document.querySelectorAll('.btn, .submit-btn');
allButtons.forEach(button => {
button.addEventListener('mouseenter', function(e) {
const rect = this.getBoundingClientRect();
const x = e.clientX - rect.left;
const y = e.clientY - rect.top;
const sparkle = document.createElement('span');
sparkle.classList.add('sparkle');
sparkle.style.left = `${x}px`;
sparkle.style.top = `${y}px`;
this.appendChild(sparkle);
setTimeout(() => {
sparkle.remove();
}, 1000);
});
});
});
</script>
</body>
</html>
