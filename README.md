# PPCC-2025---Power-Pages-CSS
Repository with code snippets from my PPCC 2025 Power Pages session!


# ✨ Simple CSS Tricks to Instantly Elevate Your Power Pages

A quick and fun guide to making your **Power Pages** look like a million bucks!  

---

## 💡 Why This Exists

Power Pages are amazing for business portals — but let’s be honest…  
the default styling looks like it graduated from 2010.  
This repo collects simple, beginner-friendly CSS snippets that instantly elevate your design  
and make your portals feel **modern, polished, and intentional**.

✅ No front-end experience required  
✅ 100% Power Pages-friendly

---

## 🪄 The Rules of Styling Power Pages

1. **Power Pages ≠ Websites**  
   Don’t fight the platform — enhance it.

2. **Keep It Simple**  
   CSS = polish, not reconstruction.

3. **Test Responsiveness**  
   Always check mobile view before showing your boss.

4. **Backup Before You Paste**  
   Because one misplaced bracket can ruin your day.

---

## 🎨 CSS Tricks

### 

ADD CUSTOM FONTS!!

1. Custom fonts

```css

@import url('https://fonts.googleapis.com/css2?family=Oswald:wght@200..700&display=swap');

* {
  font-family: 'Oswald', sans-serif !important;
}
```

2. Box Shadows

```css
.card {
  box-shadow: 0 4px 12px rgba(0,0,0,0.08);
  border-radius: 12px;
}
```


3. Hover Animations


```css
.card:hover {
  transform: translateY(-6px);
  transition: 0.3s ease;
  box-shadow: 0 10px 25px rgba(0,0,0,0.1);
}
```


What it does: Adds depth and softness.
Use for: Sections, cards, modals.
Pro tip: Avoid dark, harsh shadows — subtle wins.

4. Button hover

Pulsing button hover:

```css

button.pulse-button-hover {
	animation: colorShift 10000ms infinite ease-in;
}

button:hover,
button:focus {
	animation: borderPulse 1000ms infinite ease-out, colorShift 10000ms infinite ease-in, hoverShine 200ms;
}

/* Declate color shifting animation */
@keyframes colorShift {
	0%, 100% {
			background: #0045e6;
	}
	33% {
		background: #fb3e3e;
	}
	66%{
		background: #0dcc00;
	}
}

/* Declare border pulse animation */
@keyframes borderPulse {
  0% {
    box-shadow: inset 0px 0px 0px 5px rgba(255, 255, 255,.4), 0px 0px 0px 0px rgba(255,255,255,1);
  }
  100% {
    box-shadow: inset 0px 0px 0px 3px rgba(117, 117, 255,.2), 0px 0px 0px 10px rgba(255,255,255,0);
  }
}

/* Declare shine on hover animation */
@keyframes hoverShine {
	0%{
		background-image: linear-gradient(135deg, rgba(255,255,255,.4) 0%, rgba(255,255,255,0) 50%, rgba(255,255,255,0) 100%);
	}
	50%{
		background-image: linear-gradient(135deg, rgba(255,255,255,0) 0%, rgba(255,255,255,.4) 50%, rgba(255,255,255,0) 100%);
	}
	100%{
		background-image: linear-gradient(135deg, rgba(255,255,255,0) 0%, rgba(255,255,255,0) 50%, rgba(255,255,255,.4) 100%);
	}
}

.pulse-button-hover {
	margin: 15px auto;
	font-family: "Montserrat";
	font-size: 20px;
	color: #ffffff;
	cursor: pointer;
	border-radius: 100px;
	padding: 15px 20px;
	border: 0px solid #000;		
	}

```


Over the top button:


HTML: 

```html

<div class='container'>
  <button class='one'>Play some <b>amazing</b> games</button>
  
  

```


CSS: 

```css

@charset "UTF-8";
@import url(https://fonts.googleapis.com/css?family=Oswald:400,700);
@import url(https://fonts.googleapis.com/css?family=Nunito:400,700);


.container {
  width: 334px;
  margin: 0 auto;
  position: absolute;
  top: 50%;
  left: 0;
  text-align: center;
  right: 0;
  -webkit-transform: translateY(-50%);
          transform: translateY(-50%);
}

body
{
  background:#333;
}
a {
  color: white;
  text-decoration: none;
}

h1, h2 {
  color: white;
  font-family: 'Oswald', sans-serif;
  font-weight: normal;
}

h2 {
  font-size: 14px;
  margin-bottom: 30px;
  color: #24E2B8;
}

.one {
  border: none;
  border-radius: 4px;
  text-shadow: 0px 0px 10px rgba(0, 0, 0, 0.48);
  overflow: hidden;
  padding: 20px 50px 20px 70px;
  margin-bottom: 20px;
  font-size: 20px;
  position: relative;
  color: white;
  outline: none;
  cursor: pointer;
  width: 100%;
  -webkit-transition: background-position .7s,box-shadow .4s;
  transition: background-position .7s,box-shadow .4s;
  background-size: 110%;
  font-family: 'Oswald', sans-serif;
}
.one:hover {
  background-position: 0% 30%;
}
.one:hover:after {
  right: -40px;
  -webkit-transition: right .4s,-webkit-transform 30s .2s linear;
  transition: right .4s,-webkit-transform 30s .2s linear;
  transition: right .4s,transform 30s .2s linear;
  transition: right .4s,transform 30s .2s linear,-webkit-transform 30s .2s linear;
}
.one:before, .one:after {
  font-family: FontAwesome;
  display: block;
  position: absolute;
}
.one:before {
  -webkit-transition: all 1s;
  transition: all 1s;
  font-size: 30px;
  left: 25px;
  top: 19px;
}
.one:after {
  -webkit-transition: right .4s, -webkit-transform .2s;
  transition: right .4s, -webkit-transform .2s;
  transition: right .4s, transform .2s;
  transition: right .4s, transform .2s, -webkit-transform .2s;
  font-size: 100px;
  opacity: .3;
  right: -120px;
  top: -17px;
}

.one {
  box-shadow: 0px 0px 0px 2px rgba(255, 255, 255, 0.16) inset, 0px 0px 10px 0px #782CDA;
  background-image: -webkit-gradient(linear, left top, left bottom, from(#782CDA), to(rgba(126, 94, 162, 0.51))), url("http://gearnuke.com/wp-content/uploads/2015/11/1280x720-cuU.jpg");
  background-image: linear-gradient(to bottom, #782CDA, rgba(126, 94, 162, 0.51)), url("http://gearnuke.com/wp-content/uploads/2015/11/1280x720-cuU.jpg");
}
.one:hover {
  box-shadow: 0px 0px 0px 2px rgba(255, 255, 255, 0.16) inset, 0px 0px 30px 0px #782CDA;
}
.one:hover:after {
  -webkit-transform: scale(1);
          transform: scale(1);
}
.one:hover:before {
  -webkit-transform: scale(1.2);
          transform: scale(1.2);
}
.one:after, .one:before {
  content: "";
}
.one b {
  color: #DDA6FF;
  font-weight: 700;
}

```

4. Gradient Text

```css
.text-gradient {
  color: #e4bb67;
  background-image: linear-gradient(90deg, #00d2ff 0%, #3a47d5 100%);
  background-clip: text;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  display: inline-block;
font-weight: 700
}
```

What it does: Applies a linear gradient inside your text for a polished, modern feel.
Use for: Hero headings, logo text, section titles.

💡 Tips:

Works best with bold fonts (font-weight: 700+).
Use https://cssgradient.io/ for pre-generated gradients!

Try changing the gradient angle to 45deg for a diagonal shimmer.

5. Floating image

```css

.floating-image {
  display: inline-block;
  animation: float 3s ease-in-out infinite;
  transition: transform 0.3s ease;
}

@keyframes float {
  0% {
    transform: translateY(0px);
  }
  50% {
    transform: translateY(-10px);
  }
  100% {
    transform: translateY(0px);
  }
}


```

6. On load animation

```css
.fade-in {
  opacity: 0;
  transform: translateY(20px);
  animation: fadeUp 1s forwards;
}

@keyframes fadeUp {
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

```

What it does: Fades and slides elements into view as users scroll.
Use for: Section reveals, testimonials, stats panels.
Result: Adds subtle movement and polish.


6. Custom Scrollbars

```css
   
  * {
    scrollbar-width: auto;
    scrollbar-color: #8f54a0 #ffffff;
  }

  /* Chrome, Edge, and Safari */
  *::-webkit-scrollbar {
    width: 16px;
  }

  *::-webkit-scrollbar-track {
    background: #ffffff;
  }

  *::-webkit-scrollbar-thumb {
    background-color: #8f54a0;
    border-radius: 10px;
    border: 3px solid #ffffff;
  }

```

What it does: Makes your scrollbar match your brand theme.
Use for: Long content sections or dashboards.
Result: Instantly looks custom and cohesive.
Use this for easy customisable code: https://codepen.io/stephenpaton-tech/full/JjRvGmY


7. Glassmorphic Navbar

```css
.navbar {
  background: rgba(255,255,255,0.85);
  backdrop-filter: blur(8px);
  box-shadow: 0 2px 10px rgba(0,0,0,0.05);
}
.nav-link:hover {
  color: #0078D4;
  text-decoration: underline;
}

```

What it does: Gives your navigation that translucent, frosted-glass look.
Use for: Top bars, sticky headers, footers.
Pro tip: Combine with a light gradient background for extra elegance.







