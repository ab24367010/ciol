# Background Images Guide

Энэ хуудас нь таны website дээр өөр өөр background зургууд ашиглах заавар юм.

## 📁 Зургуудын бүтэц

`images` folder дотор дараах зургуудыг нэмж болно:

```
images/
├── background.jpeg              (одоогийн desktop light mode)
├── background-dark.jpeg         (desktop dark mode)
├── background-tablet.jpeg       (tablet light mode)
├── background-tablet-dark.jpeg  (tablet dark mode)
├── background-mobile.jpeg       (mobile light mode)
└── background-mobile-dark.jpeg  (mobile dark mode)
```

## 🎨 Хэрхэн ашиглах вэ?

### 1. Desktop Dark Mode Background

**script.js** файлын 24 болон 30 мөрүүд дээрх `//`-г устга:

```javascript
// Өмнө:
// document.body.style.backgroundImage = "url('images/background-dark.jpeg')";

// Дараа:
document.body.style.backgroundImage = "url('images/background-dark.jpeg')";
```

### 2. Tablet Backgrounds (768px хүртэл)

**styles.css** файлын 354-362 мөрүүдийн `/* */`-г устга:

```css
/* Өмнө:
body {
    background-image: url(images/background-tablet.jpeg);
}

body.dark-mode {
    background-image: url(images/background-tablet-dark.jpeg);
}
*/

/* Дараа: */
body {
    background-image: url(images/background-tablet.jpeg);
}

body.dark-mode {
    background-image: url(images/background-tablet-dark.jpeg);
}
```

### 3. Mobile Backgrounds (480px хүртэл)

**styles.css** файлын 390-398 мөрүүдийн `/* */`-г устга:

```css
body {
    background-image: url(images/background-mobile.jpeg);
}

body.dark-mode {
    background-image: url(images/background-mobile-dark.jpeg);
}
```

## 💡 Зөвлөмж

- **Desktop**: 1920x1080 эсвэл илүү
- **Tablet**: 1024x768
- **Mobile**: 750x1334 (iPhone хэмжээ)
- **Формат**: JPEG эсвэл WebP (илүү хурдан)
- **Файлын хэмжээ**: 200KB хүртэл (optimize хийсэн байх)

## 🚀 Одоогийн байдал

Одоогоор:
- ✅ Desktop light mode: `background.jpeg` ашиглаж байна
- ✅ Dark mode: Ижил зураг + 40% хар overlay
- ✅ Responsive: Зураг баруун тийш шахагдана (65-70%)

Өөр зургууд нэмэхийг хүсвэл дээрх заавруудыг дага!
