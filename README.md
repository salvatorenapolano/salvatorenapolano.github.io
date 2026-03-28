# 🚀 Roadmap Ottimizzazione Portfolio

Questo documento descrive i prossimi miglioramenti da implementare nel portfolio per aumentare performance, qualità del codice e impatto visivo.

---

## 🎯 Obiettivi principali

* Migliorare le performance (Lighthouse score)
* Ridurre il tempo di caricamento (LCP)
* Ottimizzare le risorse
* Rendere il codice più pulito e mantenibile
* Migliorare UX/UI

---

## ⚡ 1. Ottimizzazione Performance (ALTA PRIORITÀ)

### 🔥 Rimuovere Font Awesome

**Problema:**

* Carica CSS + font pesanti (~250KB)
* Introduce richieste bloccanti
* Peggiora LCP

**Soluzione:**

* ❌ Eliminare completamente Font Awesome
* ✅ Sostituire tutte le icone con SVG inline

**Esempio:**

```html
<!-- PRIMA -->
<i class="fas fa-user"></i>

<!-- DOPO -->
<svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor">
  <path d="M12 12c2.7 0 5-2.3 5-5s-2.3-5-5-5-5 2.3-5 5 2.3 5 5 5zm0 2c-3.3 
  0-10 1.7-10 5v3h20v-3c0-3.3-6.7-5-10-5z"/>
</svg>
```

---

### 📦 Ridurre richieste esterne
---

### ⚡ Ottimizzare CSS

* Inline del CSS critico
* Minimizzare file CSS
* Rimuovere codice inutilizzato

---

### 🖼️ Ottimizzare immagini

* Usare formati moderni (`webp`)
* Ridurre dimensioni
* Lazy loading:

```html
<img src="image.webp" loading="lazy">
```

---

### 🔄 Pulizia codice

* Rimuovere codice duplicato
* Usare classi riutilizzabili
* Migliorare leggibilità

---

## 🎨 3. UI / UX Improvements

### ✨ Migliorare design

* Spaziatura più consistente
* Tipografia più leggibile
* Miglior contrasto colori

---

### 🧩 Micro-interazioni

* Hover effects
* Transizioni fluide

```css
button {
  transition: all 0.3s ease;
}
```

---

## 📱 4. Responsive Design

* Test su mobile
* Migliorare layout su schermi piccoli
* Evitare overflow

---

## 🔍 5. SEO Base

* Meta tag corretti

```html
<meta name="description" content="Portfolio di ...">
```

* Titoli semanticamente corretti (`h1`, `h2`...)

---

## 🧪 6. Testing

* Lighthouse audit
* Test su:

  * Mobile
  * Desktop
  * Connessione lenta

---

## 🏁 7. Extra (facoltativi ma consigliati)

* Dark mode 🌙
* Animazioni leggere
* Sezione progetti migliorata
* Aggiunta favicon

---

## 📊 Checklist Finale

* [ ] Rimosso Font Awesome
* [ ] Convertite icone in SVG inline
* [ ] Ridotte richieste HTTP
* [ ] Ottimizzate immagini
* [ ] Migliorato CSS
* [ ] Test Lighthouse > 90
* [ ] Responsive completo

---

## 💡 Note

L'ottimizzazione delle icone (SVG inline) è uno dei miglioramenti con maggiore impatto immediato sulle performance.

---

## 👨‍💻 Autore

Salvatore Napolano

---
