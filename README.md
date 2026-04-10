# 🏛️ GhiDoRo

**Ghidul tău complet pentru București** — descoperă cele mai frumoase locuri din capitala României, de la restaurante istorice la muzee emblematice și skybar-uri cu vedere panoramică.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-222?style=flat&logo=github&logoColor=white)

**Live:** [https://garconai93.github.io/ghidoras.ro/](https://garconai93.github.io/ghidoras.ro/)

---

## ✨ Features

- **Hero Carousel** — 5 imagini spectaculoase din București, auto-play la 4 secunde
- **5 categorii:** EAT, DRINK, STAY, VISIT, MUST SEE
- **Filtrare interactiva** — click pe o categorie pentru a filtra locatiile
- **15 locatii** — 3 per categorie, cu rating, descriere si pozele din Unsplash
- **Glassmorphism design** — efecte blur, glow si transparente
- **Mobile-friendly** — responsive pe toate dispozitivele
- **Dark mode** — design modern, prietenos cu ochii

---

## 🎛️ Functionalitati

### Carousel
- Auto-play la fiecare 4 secunde
- Indicatori dot interactivi (click pentru navigare manuala)
- Fade transition smooth intre slide-uri

### Filtru Categorii
- **Click** — afiseaza doar locatiile din categoria selectata
- **Double-click** — reseteaza si afiseaza toate locatiile

### Carduri Locatii
- Hover effect cu lift si glow cyan
- Rating cu stele
- Poza, categorie, titlu, rating si descriere
- **Link Google Maps** pentru fiecare locatie — click pe card si deschide locatia in Google Maps

---

## 🛠️ Tech Stack

| Tehnologie | Detalii |
|------------|---------|
| **HTML5** | Semantic, single-page structure |
| **CSS3** | Custom properties, glassmorphism, responsive |
| **JavaScript** | Vanilla ES6, no frameworks |
| **Fonts** | Google Fonts — Inter |
| **Images** | Unsplash (royalty-free) |
| **Maps** | Google Maps (link-uri directe) |
| **Hosting** | GitHub Pages |

---

## 📁 Project Structure

```
ghidoras.ro/
├── index.html     # Totul intr-un singur fisier — HTML + CSS + JS
├── trigger.txt    # (trigger info, nefolosit in productie)
└── README.md      # Documentatia proiectului
```

**De ce totul intr-un singur fisier?**
Minimalist si perfect pentru GitHub Pages — fara build step, fara dependente, fara configurare. Upload si gata.

---

## 🚀 Deployment

### GitHub Pages (Recomandat)

1. **Fork sau cloneaza** repo-ul
2. **Mergi la** Settings → Pages
3. **Source:** Selecteaza `main` branch si `/ (root)`
4. **Save** — site-ul va fi live in ~2 minute

```bash
# Cloneaza si modifica
git clone https://github.com/garconai93/ghidoras.ro.git
cd ghidoras.ro

# Dupa modificari, commit si push
git add .
git commit -m "Update README"
git push origin main
```

### Alternativ — Deschide direct

Poți deschide `index.html` direct in browser fara niciun server. Functioneaza 100% offline ( imaginile se incarca din Unsplash cand ai internet).

---

## 🎨 Customizare

### Adauga o categorie noua

1. **Adauga un buton** in `.category-buttons`
2. **Adauga carduri** cu `data-category="NUME_CATEGORIE"`
3. **Gata!** JavaScript-ul preia automat noile elemente

### Schimba culorile

Editeaza CSS variables din `<style>`:
```css
:root {
    --accent-cyan: #00f5ff;
    --accent-purple: #a855f7;
    --bg-dark: #0a0a0f;
}
```

---

## 📜 License

MIT License — foloseste liber pentru proiecte personale sau comerciale.

---

Creat cu 💜 de [Garcon](https://github.com/garconai93)
