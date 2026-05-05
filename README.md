# <img src="/assets/favicon.ico" width="36" height="36" align="absmiddle" alt=""> Who's That Pokémon?

<div align="center">

![Pokédex](https://img.shields.io/badge/Pok%C3%A9dex-Gen%20I--IX-E3350D?style=for-the-badge)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-2ecc71?style=for-the-badge&logo=github)
![Vanilla](https://img.shields.io/badge/Vanilla-HTML%2FCSS%2FJS-FFCB05?style=for-the-badge)
![PokéAPI](https://img.shields.io/badge/Powered%20by-PokéAPI-3B4CCA?style=for-the-badge)

**A strategic Pokémon guessing game with 31 unlockable hints, a scoring system, and all 1000+ Pokémon.**

[▶ Play Now](https://litools-lab.github.io/whos-that-pokemon) · [Report a Bug](../../issues) · [Request a Feature](../../issues)

</div>

---

## 📖 About

*Who's That Pokémon?* is a browser-based guessing game inspired by the iconic TV segment. A random Pokémon from the entire National Pokédex (Generations I–IX) is selected, and your goal is to identify it using as few hints as possible.

Every hint has a **point cost** — the more you reveal, the lower your final score. Think strategically: is it worth uncovering the type early, or can you deduce it from the stats alone?

---

## 🕹️ How to Play

1. **A random Pokémon is chosen** from all 1000+ species in the National Pokédex.
2. **Click any hint button** to reveal a clue — each one adds to your points-used counter.
3. **Type your guess** in the input field. Autocomplete suggests valid Pokémon names as you type.
4. **Submit your guess.** Wrong answers are counted but don't end the round — keep trying.
5. **Your final score** is calculated when you guess correctly or give up.

---

## 🧠 Scoring System

The score starts at **1000** and is reduced by penalties, then bonuses are added.

| Factor | Effect |
|--------|--------|
| Hints used | `−(hint cost × 10)` per hint |
| Wrong guesses | `−25` for 1st, `−50` for 2nd, `−75` for 3rd… (escalating) |
| Time taken | `−2 pts/second` (capped at −200) |
| 0 hints used | `+200` bonus |
| 1–2 hints used | `+120` bonus |
| 3–4 hints used | `+60` bonus |
| 0 wrong guesses | `+100` bonus |
| 1 wrong guess | `+50` bonus |

> Score cannot go below 0. Giving up awards no score.

### 🏆 Ranks

| Score | Rank |
|-------|------|
| 900+ | 🏆 Master Trainer |
| 750+ | 🔥 Elite Four |
| 600+ | ⚡ Gym Leader |
| 450+ | 👍 Trainer |
| <450 | 🌱 Beginner |

---

## 💡 Hints

32 hints across 4 tiers. Higher cost = more revealing.

### 🔴 Tier S — Game-Breaking (10–20 pts)

| Hint | Cost | What it shows |
|------|------|----------------|
| 👤 Silhouette | 20 pts | Official artwork as a black silhouette |
| 📖 Pokédex Entry | 14 pts | A random in-game flavour text (name redacted) |
| 🔊 Cry | 12 pts | Playable audio cry |
| 🔥 Type(s) | 12 pts | One or two types with colour-coded pills |
| 🔢 Pokédex Number | 10 pts | National Dex ID |

### 🟠 Tier A — Very Revealing (8–9 pts)

| Hint | Cost | What it shows |
|------|------|----------------|
| 🏷️ Species | 9 pts | The species descriptor (e.g. "Mouse Pokémon") |
| ⚠️ Type Weaknesses | 9 pts | ×2 and ×4 weaknesses |
| 🛡️ Type Resistances | 9 pts | ×0, ¼, and ½ resistances/immunities |
| 🌱 Evolution Stage | 8 pts | Stage number and total chain length |
| 🔀 Scrambled Name | 8 pts | Letters of the name in random order |

### 🟡 Tier B — Useful (5–7 pts)

| Hint | Cost |
|------|------|
| 📅 Generation | 7 pts |
| 🗺️ Region | 7 pts |
| 🔄 Evolution Method (into this) | 7 pts |
| ➡️ Evolution Method (from this) | 7 pts |
| 🎨 Pokédex Color | 6 pts |
| 🔷 Body Shape | 6 pts |
| 📈 Full Stat Spread | 6 pts |
| ✨ Abilities | 6 pts |
| 🇯🇵 Japanese Name | 6 pts |
| 🌿 Habitat | 5 pts |
| 🔤 First Letter | 5 pts |
| ⛓️ Evolution Count | 5 pts |
| 🥚 Egg Group(s) | 5 pts |
| 💪 EV Yield | 5 pts |

### 🔵 Tier C — Supporting (3–4 pts)

| Hint | Cost |
|------|------|
| 📊 Base Stat Total | 4 pts |
| 📏 Height & Weight | 4 pts |
| ⚥ Gender Ratio | 4 pts |
| ⭐ Base Experience | 4 pts |
| 🎯 Catch Rate | 3 pts |
| 💛 Base Friendship | 3 pts |
| 📉 Growth Rate | 3 pts |
| 🏆 Legendary Status | 3 pts |

---

## 🛠️ Tech Stack

- **Pure HTML / CSS / JavaScript** — zero dependencies, zero build step
- **[PokéAPI](https://pokeapi.co/)** — open Pokémon REST API (species, stats, evolutions, types…)
- **[PokeAPI/cries](https://github.com/PokeAPI/cries)** — Pokémon audio cries
- **[Google Fonts](https://fonts.google.com/)** — Press Start 2P + DM Sans

---

## 🤝 Contributing

Contributions are welcome! If you have ideas for new hints, scoring tweaks, or UI improvements:

1. Fork the repository
2. Create a branch: `git checkout -b feature/my-idea`
3. Make your changes and open a Pull Request

---

## ⚖️ Legal

Fan-made project for educational and entertainment purposes. Pokémon and all related names, images, and content are trademarks and © of Nintendo / Game Freak / The Pokémon Company. Not affiliated with or endorsed by any of these companies.

Game data is sourced from [PokéAPI](https://pokeapi.co/).

---

## 📄 License

MIT License — see [`LICENSE`](LICENSE) for details.

---

<div align="center">

Made with ❤️ and way too much Pokémon knowledge · *Gotta guess 'em all!*

</div>
