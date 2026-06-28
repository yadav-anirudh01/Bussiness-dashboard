# 🎨 CSS Animations & Customization Cheat Sheet

## 📍 Where to Find CSS in Code

**File**: `business_analytics_elite.py`
**Lines**: 17-350 (ELITE_CSS_ANIMATIONS block)

---

## 🎯 Quick Customizations

### **1. Change Primary Brand Color**

**Current**: `#6366F1` (Indigo)

**Find & Replace These:**
```python
# Line 40: Button gradient
background: linear-gradient(135deg, #6366F1 0%, #7C3AED 100%)

# Line 45: Button shadow
box-shadow: 0 10px 25px rgba(99, 102, 241, 0.3)

# Line 240: Border colors
border: 1px solid rgba(99, 102, 241, 0.15)
```

**Popular Color Options:**

```css
/* Tech Blue (Professional) */
Primary: #0066FF
RGB: rgba(0, 102, 255, 0.3)
Gradient: #0066FF → #003D99

/* Emerald Green (Natural) */
Primary: #10B981
RGB: rgba(16, 185, 129, 0.3)
Gradient: #10B981 → #047857

/* Purple Premium (Luxury) */
Primary: #8B5CF6
RGB: rgba(139, 92, 246, 0.3)
Gradient: #8B5CF6 → #7C3AED

/* Cyan Modern (Tech) */
Primary: #0891B2
RGB: rgba(8, 145, 178, 0.3)
Gradient: #0891B2 → #06B6D4

/* Red Energy (Bold) */
Primary: #EF4444
RGB: rgba(239, 68, 68, 0.3)
Gradient: #EF4444 → #DC2626
```

---

## ⏱️ Animation Speed Control

### **Default Speeds**
```css
/* Find these and modify */
animation: fadeInUp 0.8s ease-out !important;    /* Main entrance */
animation: liquidGradient 15s ease-in-out 
           infinite;                               /* Background */
@keyframes pulseGlow { /* 2s cycle */ }           /* Hover glow */
```

### **Speed Presets**

**Ultra Fast** (Snappy, energetic)
```css
animation: fadeInUp 0.3s ease-out !important;
animation: liquidGradient 8s ease-in-out infinite;
@keyframes pulseGlow { ... }  /* 1s */
```

**Fast** (Responsive)
```css
animation: fadeInUp 0.5s ease-out !important;
animation: liquidGradient 12s ease-in-out infinite;
@keyframes pulseGlow { ... }  /* 1.5s */
```

**Standard** (Default)
```css
animation: fadeInUp 0.8s ease-out !important;
animation: liquidGradient 15s ease-in-out infinite;
@keyframes pulseGlow { ... }  /* 2s */
```

**Slow** (Elegant, premium)
```css
animation: fadeInUp 1.2s ease-out !important;
animation: liquidGradient 20s ease-in-out infinite;
@keyframes pulseGlow { ... }  /* 3s */
```

**Ultra Slow** (Luxury, minimal motion)
```css
animation: fadeInUp 1.5s ease-out !important;
animation: liquidGradient 25s ease-in-out infinite;
@keyframes pulseGlow { ... }  /* 4s */
```

---

## 🌈 Color Palette Reference

### **Complete Professional Palette**

```css
/* Backgrounds */
--bg-primary: #0F172A;      /* Deep navy (main BG) */
--bg-secondary: #1E293B;    /* Slate blue (cards) */
--bg-tertiary: #334155;     /* Lighter slate */

/* Text Colors */
--text-primary: #F8FAFC;    /* White text */
--text-secondary: #CBD5E1;  /* Light gray */
--text-tertiary: #94A3B8;   /* Medium gray */
--text-disabled: #64748B;   /* Dark gray */

/* Accent Colors */
--accent-primary: #6366F1;  /* Indigo */
--accent-green: #10B981;    /* Green (success) */
--accent-amber: #F59E0B;    /* Amber (warning) */
--accent-red: #EF4444;      /* Red (danger) */
--accent-cyan: #A5F3FC;     /* Cyan (highlight) */

/* Transparency Levels */
rgba(99, 102, 241, 0.15);   /* Very subtle */
rgba(99, 102, 241, 0.3);    /* Subtle */
rgba(99, 102, 241, 0.5);    /* Medium */
rgba(99, 102, 241, 0.7);    /* Strong */
```

---

## 🎭 Hover & Interaction Effects

### **Standard Hover (Default)**
```css
[data-testid="stMetric"]:hover {
    transform: translateY(-8px) !important;
    box-shadow: 0 20px 50px rgba(99, 102, 241, 0.25), 
                0 10px 30px rgba(0, 0, 0, 0.3) !important;
}
```

### **Aggressive Hover (More lift)**
```css
[data-testid="stMetric"]:hover {
    transform: translateY(-15px) scale(1.02) !important;
    box-shadow: 0 30px 70px rgba(99, 102, 241, 0.4) !important;
}
```

### **Subtle Hover (Minimal movement)**
```css
[data-testid="stMetric"]:hover {
    transform: translateY(-2px) !important;
    box-shadow: 0 10px 25px rgba(99, 102, 241, 0.2) !important;
}
```

### **Glow Hover (No lift)**
```css
[data-testid="stMetric"]:hover {
    box-shadow: 0 0 30px rgba(99, 102, 241, 0.4) !important;
}
```

---

## 📐 Card & Container Styling

### **Glassmorphism Intensity**

**Heavy Glass** (Maximum blur, opacity)
```css
.glass-card {
    background: rgba(15, 23, 42, 0.3) !important;      /* More transparent */
    backdrop-filter: blur(20px) !important;            /* More blur */
    border: 1px solid rgba(99, 102, 241, 0.25) !important;
}
```

**Standard Glass** (Balanced)
```css
.glass-card {
    background: rgba(15, 23, 42, 0.6) !important;
    backdrop-filter: blur(10px) !important;
    border: 1px solid rgba(99, 102, 241, 0.15) !important;
}
```

**Light Glass** (Minimal blur, visible)
```css
.glass-card {
    background: rgba(15, 23, 42, 0.8) !important;      /* Opaque */
    backdrop-filter: blur(5px) !important;             /* Light blur */
    border: 1px solid rgba(99, 102, 241, 0.1) !important;
}
```

**Solid** (No glass effect)
```css
.glass-card {
    background: #1E293B !important;                    /* Solid */
    backdrop-filter: none !important;                  /* No blur */
    border: 1px solid #334155 !important;
}
```

---

## 🌊 Background Effects

### **Current Animated Gradient** (Default)
```css
@keyframes liquidGradient {
    0% { background: linear-gradient(135deg, #0F172A 0%, #1E293B 25%, #0F172A 50%, #1E293B 100%); }
    50% { background: linear-gradient(135deg, #1E293B 0%, #0F172A 25%, #1E293B 50%, #0F172A 100%); }
    100% { background: linear-gradient(135deg, #0F172A 0%, #1E293B 25%, #0F172A 50%, #1E293B 100%); }
}
```

### **Static Gradient** (No animation)
```css
[data-testid="stAppViewContainer"] {
    background: linear-gradient(135deg, #0F172A 0%, #1E293B 50%, #0F172A 100%);
    background-size: 200% 200%;
}
```

### **Solid Background** (No gradient)
```css
[data-testid="stAppViewContainer"] {
    background: #0F172A;
}
```

### **Diagonal Stripe Pattern**
```css
[data-testid="stAppViewContainer"] {
    background: 
        repeating-linear-gradient(
            45deg,
            #0F172A,
            #0F172A 10px,
            #1E293B 10px,
            #1E293B 20px
        );
}
```

### **Radial Glow Effect**
```css
[data-testid="stAppViewContainer"] {
    background: 
        radial-gradient(circle at 50% 50%, #1E293B 0%, #0F172A 100%);
}
```

---

## 🔤 Typography Customization

### **Font Sizing**

**Current (Default)**
```css
h1 { font-size: 32px; }
h2 { font-size: 28px; }
h3 { font-size: 24px; }
p { font-size: 16px; }
```

**Larger (Bold, prominent)**
```css
h1 { font-size: 48px; font-weight: 800; }
h2 { font-size: 36px; font-weight: 700; }
```

**Smaller (Compact, minimal)**
```css
h1 { font-size: 24px; }
h2 { font-size: 20px; }
```

### **Font Families**

**System Default** (Current)
```css
font-family: 'Segoe UI', Roboto, 'Helvetica Neue', sans-serif;
```

**Elegant** (Google Fonts)
```css
font-family: 'Inter', 'Helvetica Neue', sans-serif;
```

**Modern** (Tech companies)
```css
font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
```

**Classic** (Professional)
```css
font-family: 'Georgia', 'Times New Roman', serif;
```

---

## 💫 Advanced Effects

### **Text Glow Effect**

**Enable neon text**
```css
h1, h2, h3, h4 {
    animation: neonGlow 2s ease-in-out infinite !important;
}

@keyframes neonGlow {
    0%, 100% {
        text-shadow: 0 0 10px rgba(99, 102, 241, 0.5);
    }
    50% {
        text-shadow: 0 0 20px rgba(99, 102, 241, 0.8);
    }
}
```

### **Floating Animation**

**Cards float gently**
```css
[data-testid="stMetric"] {
    animation: float 3s ease-in-out infinite !important;
}

@keyframes float {
    0%, 100% { transform: translateY(0px); }
    50% { transform: translateY(-10px); }
}
```

### **Blur on Scroll**

**Cards blur when scrolling**
```css
[data-testid="stMetric"] {
    transition: filter 0.3s ease;
}

[data-testid="stMetric"]:hover {
    filter: blur(0px);
}
```

---

## 🎨 Color Scheme Presets

### **Dark Professional** (Current)
```css
--primary-color: #6366F1;
--bg-color: #0F172A;
--secondary-bg: #1E293B;
--text-color: #F8FAFC;
```

### **Light Professional**
```css
--primary-color: #4F46E5;
--bg-color: #FFFFFF;
--secondary-bg: #F3F4F6;
--text-color: #1F2937;
```

### **Dark Green** (Eco-friendly)
```css
--primary-color: #10B981;
--bg-color: #064E3B;
--secondary-bg: #065F46;
--text-color: #ECFDF5;
```

### **Dark Purple** (Creative)
```css
--primary-color: #A855F7;
--bg-color: #3B0764;
--secondary-bg: #581C87;
--text-color: #F3E8FF;
```

### **Dark Red** (Energy)
```css
--primary-color: #EF4444;
--bg-color: #7F1D1D;
--secondary-bg: #991B1B;
--text-color: #FEE2E2;
```

---

## 📊 Button Customization

### **Current Style**
```css
button[kind="primary"] {
    background: linear-gradient(135deg, #6366F1 0%, #7C3AED 100%);
    border-radius: 10px;
    padding: 12px 24px;
}
```

### **Rounded Buttons** (Maximum border radius)
```css
button[kind="primary"] {
    border-radius: 50px;  /* Fully rounded */
}
```

### **Sharp Buttons** (No rounding)
```css
button[kind="primary"] {
    border-radius: 2px;  /* Minimal rounding */
}
```

### **Large Buttons** (More padding)
```css
button[kind="primary"] {
    padding: 16px 32px;  /* Larger */
    font-size: 16px;
}
```

### **Small Buttons** (Compact)
```css
button[kind="primary"] {
    padding: 8px 16px;   /* Smaller */
    font-size: 13px;
}
```

---

## 🔗 Useful CSS Resources

| Resource | URL |
|----------|-----|
| CSS Animations | https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Animations |
| Easing Functions | https://easings.net |
| Color Picker | https://htmlcolorcodes.com |
| Gradient Generator | https://www.colorgradient.io |
| Shadow Generator | https://www.box-shadow.art |
| Animation Timeline | https://codepen.io/topics/animation |

---

## 🎯 Pro Tips

### **Tip 1: Test Changes Locally**
```bash
# After editing CSS, restart Streamlit
streamlit run business_analytics_elite.py
```

### **Tip 2: Use Browser Dev Tools**
1. Right-click → Inspect
2. Find element in DevTools
3. Edit CSS live to test
4. Copy working CSS to file

### **Tip 3: Create a CSS Backup**
```bash
# Before making changes
cp business_analytics_elite.py business_analytics_elite.backup.py
```

### **Tip 4: Combine Multiple Effects**
```css
/* Add multiple animations */
animation: 
    fadeInUp 0.8s ease-out,
    float 3s ease-in-out infinite;
```

### **Tip 5: Performance First**
```css
/* Use transform/opacity (GPU accelerated) */
transform: translateY(-8px);
opacity: 0.8;

/* Avoid (CPU intensive) */
/* top: -8px; */
/* filter: opacity(0.8); */
```

---

## ✅ Customization Checklist

- [ ] Changed primary color from #6366F1 to your brand color
- [ ] Adjusted animation speeds to match brand feel
- [ ] Customized card hover effects
- [ ] Modified button styling
- [ ] Updated background gradient (optional)
- [ ] Adjusted typography sizes
- [ ] Tested all pages
- [ ] Verified performance (60 FPS)
- [ ] Deployed to Streamlit Cloud

---

**Happy Customizing! 🎨✨**

Need help? Check SETUP_GUIDE.md for detailed instructions.
