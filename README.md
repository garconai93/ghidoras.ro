# 🏛️ GhiDoRo

**Ghidul tău complet pentru București** — descoperă cele mai frumoase locuri din capitala României, de la restaurante istorice la muzee emblematice și skybar-uri cu vedere panoramică.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-222?style=flat&logo=github&logoColor=white)

**🚀 Live:** [https://garconai93.github.io/ghidoras.ro/](https://garconai93.github.io/ghidoras.ro/)

---

## ✨ Features

- **Hero Carousel** — 5 imagini spectaculoase din București, auto-play la 4 secunde
- **5 categorii:** EAT, DRINK, STAY, VISIT, MUST SEE
- **Filtrare interactivă** — click pe o categorie pentru a filtra locațiile
- **15 locații** — 3 per categorie, cu rating, descriere și pozele din Unsplash
- **Glassmorphism design** — efecte blur, glow și transparente
- **Mobile-friendly** — responsive pe toate dispozitivele
- **Dark mode** — design modern, prietenos cu ochii

---

## 🎛️ Funcționalități

### Carousel
- Auto-play la fiecare 4 secunde
- Indicatori dot interactivi (click pentru navigare manuală)
- Fade transition smooth între slide-uri

### Filtru Categorii
- **Click** — afișează doar locațiile din categoria selectată
- **Double-click** — resetează și afișează toate locațiile

### Carduri Locații
- Hover effect cu lift și glow cyan
- Rating cu stele (★★★★☆)
- Poză, categorie, titlu, rating și descriere

---

## 🛠️ Tech Stack

| Tehnologie | Detalii |
|------------|---------|
| **HTML5** | Semantic, single-page structure |
| **CSS3** | Custom properties, glassmorphism, responsive |
| **JavaScript** | Vanilla ES6, no frameworks |
| **Fonts** | Google Fonts — Inter |
| **Images** | Unsplash (royalty-free) |
| **Hosting** | GitHub Pages |

---

## 📁 Project Structure

```
ghidoras.ro/
├── index.html     # Totul într-un singur fișier — HTML + CSS + JS
├── trigger.txt    # (trigger info, nefolosit în producție)
└── README.md      # Documentația proiectului
```

**De ce totul într-un singur fișier?**
Minimalist și perfect pentru GitHub Pages — fără build step, fără dependențe, fără configurare. Upload și gata.

---

## 🚀 Deployment

### GitHub Pages (Recomandat)

1. **Fork sau clonează** repo-ul
2. **Mergi la** Settings → Pages
3. **Source:** Selectează `main` branch și `/ (root)`
4. **Save** — site-ul va fi live în ~2 minute

```bash
# Clonează și modifică
git clone https://github.com/garconai93/ghidoras.ro.git
cd ghidoras.ro

# După modificări, commit și push
git add .
git commit -m "Update README"
git push origin main
```

GitHub Pages va servi automat `index.html` din root.

### Alternativ — Deschide direct

Poți deschide `index.html` direct în browser fără niciun server. Funcționează 100% offline ( imaginile se încarcă din Unsplash când ai internet).

---

## 🎨 Customizare

### Adaugă o categorie nouă

1. **Adaugă un buton** în `.category-buttons`:
```html
<button class="category-btn" data-category="shop">
    <span class="icon">🛍️</span>
    <span class="label">SHOP</span>
</button>
```

2. **Adaugă carduri** cu `data-category="shop"`

3. **Gata!** JavaScript-ul preia automat noile elemente

### Schimbă culorile

Editează CSS variables din `<style>`:
```css
:root {
    --accent-cyan: #00f5ff;    /* Glow/hover effects */
    --accent-purple: #a855f7;  /* Gradient highlights */
    --bg-dark: #0a0a0f;        /* Fundal principal */
}
```

### Adaugă slide nou în carousel

```html
<div class="carousel-slide">
    <img src="YOUR_IMAGE_URL" alt="Descriere">
    <div class="carousel-overlay"></div>
</div>
```
 apoi un dot indicator:
```html
<span class="carousel-dot" data-index="5"></span>
```

---

## 📜 License

MIT License — folosește liber pentru proiecte personale sau comerciale.

---

Creat cu 💜 de [Garcon](https://github.com/garconai93)
