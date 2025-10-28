# PPCC-2025---Power-Pages-CSS
Repository with code snippets from my PPCC 2025 Power Pages session!


# ✨ Simple CSS Tricks to Instantly Elevate Your Power Pages

> A quick and fun guide to making your **Power Pages** look like a million bucks —  

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

### 1️⃣ Hover Animations

'''css

.card:hover {
  transform: translateY(-6px);
  transition: 0.3s ease;
  box-shadow: 0 10px 25px rgba(0,0,0,0.1);
}

```css
.card:hover {
  transform: translateY(-6px);
  transition: 0.3s ease;
  box-shadow: 0 10px 25px rgba(0,0,0,0.1);
}

2️⃣ Box Shadows
.card {
  box-shadow: 0 4px 12px rgba(0,0,0,0.08);
  border-radius: 12px;
}


What it does: Adds depth and softness.
Use for: Sections, cards, modals.
Pro tip: Avoid dark, harsh shadows — subtle wins.




4️⃣ Gradient Text
.gradient-text {
  background: linear-gradient(90deg, #0078D4, #8A2BE2);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-weight: 700;
}


What it does: Applies a linear gradient inside your text for a polished, modern feel.
Use for: Hero headings, logo text, section titles.

💡 Tips:

Works best with bold fonts (font-weight: 700+).

Try changing the gradient angle to 45deg for a diagonal shimmer.

5️⃣ Scroll Animations
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


What it does: Fades and slides elements into view as users scroll.
Use for: Section reveals, testimonials, stats panels.
Result: Adds subtle movement and polish.


6️⃣ Custom Scrollbars
::-webkit-scrollbar {
  width: 8px;
}
::-webkit-scrollbar-thumb {
  background: linear-gradient(#0078D4, #8A2BE2);
  border-radius: 4px;
}


What it does: Makes your scrollbar match your brand theme.
Use for: Long content sections or dashboards.
Result: Instantly looks custom and cohesive.


8️⃣ Glassmorphic Navbar
.navbar {
  background: rgba(255,255,255,0.85);
  backdrop-filter: blur(8px);
  box-shadow: 0 2px 10px rgba(0,0,0,0.05);
}
.nav-link:hover {
  color: #0078D4;
  text-decoration: underline;
}


What it does: Gives your navigation that translucent, frosted-glass look.
Use for: Top bars, sticky headers, footers.
Pro tip: Combine with a light gradient background for extra elegance.







