# 🌍 Dude World — Free AI Tools Website

**YouTube:** [@dudegamer410](https://youtube.com/@dudegamer410)

---

## 📁 Project Structure

```
dude-world/
├── index.html              ← Homepage (সব tools এর list)
├── assets/
│   └── style.css           ← Shared theme (সব page এ একই look)
├── tools/
│   └── cv-builder.html     ← CV Builder tool
│   └── (নতুন tools এখানে আসবে)
└── README.md
```

---

## 🚀 Vercel এ Deploy করার Guide

### Step 1 — GitHub এ Upload করো
1. [github.com](https://github.com) এ account করো (থাকলে skip)
2. New Repository বানাও — নাম দাও `dude-world`
3. সব files upload করো (index.html, assets folder, tools folder)

### Step 2 — Vercel এ Connect করো
1. [vercel.com](https://vercel.com) এ GitHub দিয়ে login করো
2. "Add New Project" → তোমার `dude-world` repo select করো
3. Settings সব default রাখো → **Deploy** button চাপো
4. ✅ Done! তোমার website live হয়ে যাবে!

### Step 3 — Custom Domain (optional)
- Vercel free তে একটা domain দেয়: `dude-world.vercel.app`
- নিজের domain কিনতে চাইলে Namecheap বা GoDaddy থেকে কেনো

---

## ➕ নতুন Tool Add করার Guide

### মাত্র ২টা কাজ করতে হবে:

**কাজ ১ — নতুন tool এর HTML file বানাও**

`tools/` folder এ নতুন file বানাও, যেমন: `tools/bio-generator.html`

File এর শুরুতে এই দুটো line রাখো (CV Builder থেকে copy করো):
```html
<link rel="stylesheet" href="../assets/style.css">
```
Header এ back link রাখো:
```html
<a href="../index.html" class="dw-back">← Back to All Tools</a>
```

**কাজ ২ — index.html এ tool card add করো**

`index.html` খোলো, tools-grid এর ভেতরে এই block copy-paste করো:

```html
<!-- ── TOOL: Bio Generator ── -->
<a href="tools/bio-generator.html" class="tool-card">
  <div class="tool-icon">✍️</div>
  <div class="tool-name">Bio Generator</div>
  <div class="tool-desc">Social media bio তৈরি করো সেকেন্ডে।</div>
  <div class="tool-tag">✦ AI Powered</div>
  <div class="tool-arrow">→</div>
</a>
```

**ব্যস! GitHub এ push করো → Vercel auto-deploy করবে।**

---

## 🎨 Theme Colors

```css
--ink:        #0d0d0d   /* কালো */
--cream:      #f5f0e8   /* background */
--gold:       #c9a84c   /* accent */
--gold-light: #e8d49a   /* হালকা gold */
--paper:      #faf7f2   /* card background */
--muted:      #7a7060   /* secondary text */
```

---

## 📋 Planned Tools

- [x] CV & Cover Letter Builder
- [ ] Bio Generator
- [ ] Caption & Post Writer
- [ ] Email Writer
- [ ] আরো আসছে...

---

Made with ❤️ in Bangladesh 🇧🇩
