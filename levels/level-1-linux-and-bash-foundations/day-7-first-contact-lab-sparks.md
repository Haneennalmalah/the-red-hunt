# 🧷 Day 7 — Into the Wire

> “The wires hum. Each challenge a whisper, each file a riddle. Aroha stepped forward... and the game began.”

---

## 🎮 Missions: Bandit 0–4 — OverTheWire

Today, Aroha jacked into the first five stages of the **OverTheWire: Bandit** wargame — a classic battleground for young hunters.

- ✅ **Level 0**
- ✅ **Level 1**
- ✅ **Level 2**
- ✅ **Level 3**
- ✅ **Level 4**

Each level demanded precision, patience, and familiarity with how Linux hides and reveals the truth. The world behind the shell grew stranger.

---

## ⚔️ New Commands in Her Arsenal

| Command | Purpose |
|--------|---------|
| `more` | Paginate file content — slow and steady read. |
| `file ./*` | Identify file types, even of mysterious or hidden files. |
| `find` | Search through the digital mist to discover buried secrets. |
| `ls -lah` | The veil-lifter — reveals hidden `.files`. |
| `cat` | Still the go-to blade for revealing contents. |

---

## 📓 Notes from the Battlefield

### 🫥 Hidden Files (Linux Stealth)

- **To hide** a file:  
  Prefix it with a dot.  
  Example: `.file.txt`

- **To find** hidden files:  
  Use: `ls -lah`

- **To access** a hidden file directly:  
  Just type its name like any other file:  
  `cat .file.txt`

- **To unhide**:  
  Rename it without the dot.  
  Example:  
  `mv .file.txt file.txt`

---

### ⚠️ Tricky Filenames (with spaces)

- If a file has **spaces in its name**, escape the spaces with backslashes:
  
  Example:  
  ```bash
  cat the\ aroha\ game
