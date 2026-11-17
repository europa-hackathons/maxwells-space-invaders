# 👾 Maxwell's Space Invaders

A Space Invaders arcade game made by **Maxwell (age 8)** and his mamma, built step by step by asking Claude for one new feature at a time.

**▶️ Play it here:** https://europa-hackathons.github.io/maxwells-space-invaders/

The whole game is one file, `index.html`. It works on computers, phones and tablets. You can also open it straight from your computer in any web browser, with nothing to install.

---

## 🎮 How to Play

| | Computer | Phone / Tablet |
|---|---|---|
| Move | ⬅️ ➡️ Arrow keys | Hold the ◀ ▶ buttons |
| Shoot | Space | Tap the FIRE button |
| Play again | R | Tap the game screen |

- Shoot all the aliens to move on to the next level.
- **Red aliens shoot back!** Only 3 aliens in the bottom row can shoot, so try to get them first.
- You start with **3 lives** (♥♥♥) and can have up to **5**.
- **Catch the falling pink hearts** to get a free life. Every level drops one, and blown-up aliens sometimes drop one too.
- After you get hit, your ship blinks. While it blinks, you can't be hit again.
- If the aliens reach your ship, or you run out of lives, it's game over.

## 🗺️ Levels and Bosses

There are 9 levels, and a boss shows up every 3 levels.

| Level | What happens |
|---|---|
| 1–2 | White aliens |
| **3** | 🟣 **Boss: ZORG THE PURPLE.** Takes 15 hits, shoots one laser at a time |
| 4–5 | Light blue aliens (a bit faster) |
| **6** | 🟢 **Boss: OCTO-BLASTER.** Takes 20 hits, shoots 2 lasers at once |
| 7–8 | Yellow aliens (even faster) |
| **9** | 🟠 **FINAL BOSS: MEGA KING.** Takes 25 hits, shoots 3 lasers in a fan shape |

Beat MEGA KING to **save the galaxy!** 🏆

## ⭐ Scoring

| What you do | Points |
|---|---|
| Blow up an alien | 10 |
| Hit a boss | 5 |
| Beat a boss | 500 |

## 🔊 Sounds

The game makes its own retro arcade sounds as it plays: a *pew* when you shoot, explosions, a *ta-da* when you catch a heart, and the classic *dum-dum-dum-dum* marching beat that speeds up as fewer aliens are left.
Sound starts after your first key press or tap, because browsers don't let a page play sound until you press something. On an iPhone, turn off silent mode to hear it.

## 🛠️ Change the Game Yourself!

Open `index.html` in a text editor. The **SETTINGS** section at the top has numbers you can change. Save the file, then reload the page in your browser to see what happens.

| Setting | What it changes |
|---|---|
| `SHIP_SPEED` | How fast your ship moves |
| `ALIEN_SPEED` | How fast the aliens march on level 1 |
| `SPEED_UP_PER_LEVEL` | How much faster the aliens get each level |
| `ALIEN_ROWS` / `ALIEN_COLS` | How many aliens there are |
| `START_LIVES` / `MAX_LIVES` | How many lives you start with, and the most you can have |
| `HEART_DROP_CHANCE` | How often blown-up aliens drop hearts (`0.1` = 1 in 10) |
| `ALIEN_SHOOT_CHANCE` | How often the red aliens shoot |
| `BOSSES` | Each boss's name, color, health, speed, how often it shoots, and its picture |

**Draw your own aliens!** In the pixel art sections (`SHIP_ART`, `ALIEN_ART`, `HEART_ART` and each boss's `art`), every `1` is a colored square and every `0` is empty. Swap them around to draw a new picture.

> **Mac tip:** If TextEdit shows the game page instead of the code, go to **TextEdit → Settings → Open and Save** and tick **"Display HTML files as HTML code instead of formatted text."**

## 🧑‍💻 How It's Built

- One HTML file, using plain JavaScript and the HTML `<canvas>` to draw the game.
- The sounds are made by the computer as the game plays, using the browser's Web Audio API, so there are no sound files.
- On phones and tablets, the game shrinks to fit the screen and shows touch buttons.
- No libraries, nothing to download, and no internet connection needed.
- It's published with GitHub Pages, from the `main` branch.

---

Made with ❤️ by Maxwell, with help from Dad and Claude. Inspired by his friend Dina's Pac-Man game.
