# TOTAL RANDOM TARIFA

> Get off your phone. Go outside. Let the dice decide.

---

## File structure

```
total-random-tarifa/
├── index.html        ← Main website (don't edit unless you know HTML)
├── headlines.js      ← ✏️ EDIT: your rotating slogans
├── data/
│   ├── outdoor.js    ← ✏️ EDIT: outdoor / trekking activities
│   ├── sport.js      ← ✏️ EDIT: sport activities (kitesurf, windsurf...)
│   ├── food.js       ← ✏️ EDIT: food & drink activities
│   ├── culture.js    ← ✏️ EDIT: culture & history activities
│   └── hidden.js     ← ✏️ EDIT: hidden gems
└── README.md
```

---

## Editing activities

Open the relevant file in `/data`. Each activity looks like this:

```js
{
  name: "Playa de los Lances",
  desc: "Walk the wildest stretch of Atlantic beach...",
  category: "outdoor",     // must match the file's category — don't change this
  duration: "1–3 h",
  tip: "Go at sunset.",
  link: "https://maps.google.com/?q=Playa+de+Los+Lances,+Tarifa"
}
```

### The `link` field — this is the "Start Your Unbowed Adventure" button

Set this to whatever you want the button to open:
- A **Google Maps link** → `https://maps.google.com/?q=PLACE+NAME`
- A **business website** → e.g. `https://www.tarifakitesurf.com`
- A **booking page** → for kite lessons, restaurant reservations, tours, etc.

Just copy a block, paste it before the closing `]`, and edit name/desc/duration/tip/link.

---

## "Not for me" button

When a user clicks **Not for me**, that activity is hidden for the rest of their
session (stored in their browser only — nothing is sent anywhere). Clicking
**Reveal Another** picks a new one excluding anything marked "not for me".
If a whole category gets marked "not for me", the list resets automatically.

---

## Editing headlines

Open `headlines.js`. One slogan per line. Add, remove, or edit freely.

---

## Deploy to GitHub Pages (free)

1. Create a free account at https://github.com
2. **New repository** → name it `total-random-tarifa` → Public → Create
3. Click **uploading an existing file**
4. Drag in: `index.html`, `headlines.js`, `README.md`, and the whole `data` folder
   (drag the folder itself — GitHub preserves the structure)
5. Click **Commit changes**
6. Go to **Settings → Pages** → Branch: `main`, folder `/ (root)` → **Save**
7. Live in ~1 minute at:
   `https://YOUR-USERNAME.github.io/total-random-tarifa`

### Updating later
Click any file → pencil icon ✏️ → edit → **Commit changes**. Live within ~60 seconds.

---

*Built with love for Tarifa. No algorithms. Just the unknown.*
