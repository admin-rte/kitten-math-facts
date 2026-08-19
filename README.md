# 🐱 Kitten Math Facts

A cheerful, self-contained math-facts practice app for kids. Answer randomly
generated arithmetic problems and a cute cartoon kitten celebrates every correct
answer (and gently cries at a wrong one). No accounts, no scores to chase — just
endless friendly practice.

Everything lives in a single HTML file: the kitten is drawn as inline SVG and the
sounds are synthesized in the browser, so there are **no external files, no build
step, no server, and no internet connection required.** Double-click and play.

**▶️ Play it online: https://admin-rte.github.io/kitten-math-facts/**

---

## 🚀 Getting started

Open **`index.html`** in any modern browser — double-click it,
or drag it onto a browser window. That's the whole app.

It's designed for phones and tablets (big on-screen number pad), but works just as
well on a desktop, where the physical keyboard works too.

### 📲 Install it like an app (iOS)

Open `index.html` in Safari, then tap **Share → Add to Home
Screen**. It launches full-screen like a native app.

---

## ✨ Features

### Practice modes
- **➕ Add** and **➖ Sub** — answers capped at a configurable maximum (default 20).
  Trivial "+0 / +1" style problems are mostly filtered out so practice stays meaty.
- **✖️ Mult** and **➗ Div** — built from the times tables you choose (1–12).
  Division always comes out to a whole number.
- **🔀 Mix** — combines operations. Defaults to Add + Sub, but you can enable any
  mix of all four in Settings.
- Problems appear **horizontally or vertically** at random (division stays horizontal).
- Switch modes at any time — there's no "finish," just more problems.

### Answering
- Big, touch-friendly **on-screen number pad** with Clear and backspace.
- Submit with the green **✓ Enter** key or the physical **Enter** key.
- A **physical keyboard** also works throughout (digits, Enter, Backspace, Esc to clear).

### Feedback
- ✅ **Correct** → a happy, wiggling kitten and a cheerful chime.
- ❌ **Wrong** → a crying kitten and a soft buzz; you must enter the correct answer
  to move on.
- 🎉 **Surprise celebrations** (~1 in 5 correct answers) — the kitten gets a fish
  treat, chases a mouse, wears a mouse on its head, or throws a mini party.
- 🔊 Sound can be toggled off.

### 🚀 Space mode (optional)

Tap the **🚀** button to blast off into a dark, star-studded theme. The kitten
becomes a rocket pilot flying through space with **three hearts**:
- ✅ **Correct** → the pilot dodges an incoming asteroid or blasts it with lasers.
- ❌ **Wrong** → the rocket collides with the asteroid and loses a heart.
- ⏱ **Out of time** (when timed mode is on) → the asteroid crashes into the ship
  and costs a heart too.
- 💥 Lose all three hearts and it's **game over** (with a defeat sound) — tap
  **Try Again** to start a fresh run with full hearts.

Space mode layers on top of whichever math mode you've picked (and works with
timed mode), so you can practice addition, times tables, or anything else while
flying.

### ⏱ Timed mode (optional, off by default)
- A countdown bar races you to answer (default 15 seconds, adjustable 3–60).
- The **first problem of a session is never timed** — a gentle warm-up.
- Run out of time and the correct answer is revealed; press **Enter** to continue.

### 📜 History & stats
- Every response is logged — correct, wrong (showing what was entered), or timed out.
- Summary stats at a glance: **accuracy %**, plus **average / fastest / slowest**
  solve time.
- History and all settings are **saved in the browser** between sessions, with a
  one-tap **Clear history** button.

---

## ⚙️ Settings reference

Open with the **⚙️** button (top-right).

| Setting | Default | Notes |
| --- | --- | --- |
| Biggest answer (Add/Sub) | 20 | Any value 5–999 |
| Times tables (× and ÷) | 1–12 all on | Pick which tables to practice |
| Mix mode includes | Add + Sub | Toggle any of Add / Sub / Mult / Div |
| Timed mode | Off | On/off |
| Seconds per problem | 15 | 3–60, used when timed mode is on |

---

## 🛠 How it works

- **One file, no dependencies.** Structure (HTML), styling (CSS), and behavior
  (JavaScript) are all inline.
- **The kitten is SVG** — drawn with vector shapes, so it stays crisp at any size,
  and celebration variants layer in animated emoji.
- **Sounds are synthesized** with the Web Audio API — no audio files to load.
- **Settings and history persist** via the browser's `localStorage`.

> Note: browsers block audio until the first tap/click, so the first interaction
> "unlocks" sound. This is a browser rule, not a bug.

---

## 📦 Repository

- `index.html` — the app (single self-contained file)
- `README.md` — this file
- `LICENSE` — MIT License

Contributions/changes are tracked with git for progress and backups.

---

## 📄 License

Released under the [MIT License](LICENSE) — free to use, modify, and share.
