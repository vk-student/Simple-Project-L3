# Interacțiuni cu AI — Laborator 3

Acest fișier documentează **doar** partea de AI din laboratorul 3: cum a fost folosit un asistent AI
pentru a genera și rafina codul.

## Scop
- Folosirea AI ca **asistent colaborativ**, nu „generează tot”.
- Obținerea de cod **targetat** (HTML/CSS) și un text de **documentație** (acest README).

## Flux de lucru (scurt)
1. `git checkout main && git pull upstream main`
2. `git checkout -b feature/ai-readme` (ramură dedicată AI)
3. Conversații iterative cu AI → generare și rafinare cod
4. Commit & push pe ramura de AI, apoi PR (dacă este necesar)

## Ce a generat AI
- Secțiunea **„Despre Mine”** în `index.html` (structură semantică + conținut scurt).
- Stiluri în `styles.css`:
  - Layout pe **CSS Grid** (2 coloane, 1 coloană sub 600px).
  - Elemente tip „chip”.
- Acest **README** cu pașii și prompturile-cheie.

## Prompturi folosite (exemple)
- **Rol:**
  - „Acționează ca un dezvoltator front-end expert în HTML5 și CSS modern.”
- **Context:**
  - „Lucrez la `index.html`. În `<main>` vreau o secțiune `#despre` după conținutul existent.”
- **Sarcină clară (HTML):**
  - „Generează doar HTML pentru `<section id="despre">` cu titlu, două coloane (Abilități/Stack) și o listă.”
- **Sarcină clară (CSS):**
  - „Generează doar CSS pentru `#despre`: grid 2 coloane, gap 1.25rem, chip-uri rotunjite; fără `float`.”
- **Rafinare (responsive):**
  - „Adaugă media query: sub 600px, grila devine 1 coloană.”
- **Documentare:**
  - „Scrie un README scurt care descrie exclusiv faza de AI (scop, pași, rezultate, prompturi).”

## Bune practici folosite
- Prompturi **specifice**, cu **restricții** („doar HTML”, „doar CSS”).
- **Iterații scurte**: cereri mici → feedback → ajustări.
- Separare pe ramură dedicată (`feature/ai-readme`) pentru claritate în PR.

## Reproducere rapidă
1. Deschide proiectul în editor.
2. Trimite către AI numai porțiunile relevante (ex.: `<main>` sau blocul CSS țintă).
3. Cere cod **minimal** și **constrâns**, apoi ajustează în pași mici.
4. Testează în browser, apoi `git add/commit/push` pe ramura de AI.

---

Autor: Volodymyr Khailov • Semigrupa: 3112b
