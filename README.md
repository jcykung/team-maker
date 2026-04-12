# Team Maker

> Quickly make random teams, manage rosters, and design seating arrangements — great for **teachers**, **coaches**, and **event planners**.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Visit%20Site-A6E22E?style=for-the-badge&logo=github)](https://jcykung.github.io/team-maker)
[![License](https://img.shields.io/badge/License-MIT-66D9EF?style=for-the-badge)](LICENSE)
[![No Dependencies](https://img.shields.io/badge/Dependencies-None-AE81FF?style=for-the-badge)]()

---

## ✨ Features at a Glance

| Feature | Desktop | Mobile |
|---|---|---|
| 👥 Roster management | ✅ | ✅ |
| 🎲 Random team generation | ✅ | ✅ |
| 🔒 Pair constraints (together / apart) | ✅ | ✅ |
| 🪑 Seating plan designer | ✅ | ❌ |
| 📽️ Projector / fullscreen mode | ✅ | ✅ |
| 💾 Multi-file auto-save | ✅ | ✅ |
| 📤 Export to JPG / PDF | ✅ | ✅ |
| 🎱 Random name picker | ✅ | ✅ |

---

## 📸 Screenshots
<figure>
  <img width="600px" alt="Roster area for adding people." src="https://github.com/user-attachments/assets/f55a35a0-d1e0-4b0f-881f-af73b3cfb554" />
  <br>
  <figcaption>Import a roster from a .csv file or paste in the names.</figcaption>
</figure>
<br><br>
<figure>
  <img width="600px" alt="Teams area for generating teams." src="https://github.com/user-attachments/assets/f03f13ae-c101-4e15-8d89-e1a95c6ff808" />
  <br>
  <figcaption>In the Teams tab, add constraints and generate teams randomly or drag-and-drop names.</figcaption>
</figure>
<br><br>
<figure>
  <img width="600px" alt="Seating area for drawing seating plans and placing people." src="https://github.com/user-attachments/assets/d5b11555-0eed-4ffa-97ff-440baafc5783" />
  <br>
  <figcaption>In the Seating tab, create your own seating map and randomly populate seats or drag-and-drop names.</figcaption>
</figure>

---

## 📖 How to Use

### 👤 Step 1 — Build Your Roster

Go to the **Roster** tab. Paste a list of names (one per line) or upload a `.csv` file, then click **Load List**.

- Click a name chip to **edit** it inline
- Click **×** on a chip to remove someone
- The tool automatically strips quotes, converts `Last, First` → `First Last`, and skips duplicates
- 🎱 **Random Picker** — randomly calls on someone from your roster; tick *Remove after selection* so nobody is picked twice

---

### 🤝 Step 2 — Generate & Edit Teams

Go to the **Teams** tab. Choose *Members per Team* or *Number of Teams*, set the amount, then click **Generate Teams**.

- **Desktop:** drag name chips between team cards to reassign
- **Mobile:** tap a name to move it to a different team
- Add **free-floating text labels** to the canvas with the **Text Box** button
- Use **Constraints** to keep two people on the same team or always keep them apart — the algorithm tries up to 500 arrangements to honour every rule

#### 📽️ Projector Mode (Teams)

Press the fullscreen ⛶ button to go fullscreen. Teams are automatically **centred and zoomed** to fill the screen.

| Action | How |
|---|---|
| Pan | Drag the canvas or use **←↑↓→** arrow keys |
| Zoom | `−` / `+` controls (bottom-right) or **Ctrl+scroll** |
| Re-centre | Click the ⊡ **fit button** in the zoom controls |
| Exit | **Esc** or the **Exit** button in the zoom controls |

> 🔒 Projector mode is **read-only** — cards and chips cannot be edited or moved.

---

### 🪑 Step 3 — Create a Seating Plan _(desktop only)_

Go to the **Seating** tab. Draw a room layout and place people in seats.

#### Drawing seats

| Tool | Key | What it does |
|---|---|---|
| Select / Move | `V` | Select, move, resize, or rotate a seat |
| Square seat | `S` | Click to place; click-and-drag to paint a row |
| Circle seat | `C` | Click to place; click-and-drag to paint a row |
| Label □ | `U` | Named shape (e.g. "Teacher's Desk") — not assigned to anyone |
| Label ○ | `O` | Named circle shape |
| Text Box | `T` | Free-floating text label anywhere on the canvas |
| Delete | `D` | Click seats to erase them |
| Delete selected | `Del` / `⌫` | Remove the selected seat or text box |
| Undo | `Ctrl+Z` | |
| Redo | `Ctrl+Y` | |

#### Assigning seats

1. Click **Load Roster** to bring your member list into the sidebar
2. Click **Assign Seats** to auto-assign everyone (respects Constraints)
3. **Drag** name chips between seats to adjust manually
4. Click **×** on a chip to return that person to the sidebar

#### Advanced seating features

- **Split into sections** — right-click any seat → *Split into seats* to divide a large table into multiple named sections; drag chips freely within the table
- **Rotate individual seats** — use the Select tool (`V`) to reveal corner resize handles and a top rotation handle (saved with your layout)
- **Rotate the entire plan** — rotate button beside the zoom controls; rotates and saves everything on the canvas
- **Snap to grid** — toggle **Snap On** to keep seats aligned
- **Save layouts** — click the 💾 save icon next to "Seating Plan" to save and load named layouts (great for multiple classes or rooms)

#### 📽️ Projector Mode (Seating)

Same as Teams projector mode, plus:

| Action | How |
|---|---|
| Rotate view | 🔄 **Rotate** button — spins the layout so students read the map from their side of the room; **auto-recentres** after each rotation |
| Re-centre | ⊡ **Fit button** in the zoom controls |
| Exit | **Esc** or the **Exit** button |

> 🔒 Projector mode is **read-only**. All rotation is **temporary** — it never affects your saved layout and resets on exit.

---

### 📤 Step 4 — Export

Go to the **Export** tab for a clean, light-mode preview ready for printing or sharing.

| Button | What it does |
|---|---|
| 🟢 **Save JPG** | High-resolution image |
| 🟠 **Save PDF** | Print-ready PDF |
| 🔴 **Save Backup** | Downloads your data as a `.json` file you can restore later |

---

### 📁 Step 5 — Files & Auto-Save

Everything **saves automatically** as you work — no save button needed.

Click **Files** in the header to manage multiple files — useful if you have multiple classes, teams, or events. Each file has its own roster, teams, and seating layout.

> ⚠️ **Important:** Data is stored in your **browser only** — it is not backed up to the cloud and will be lost if you clear your browser data or switch devices. Use **Save Backup** on the Export tab regularly and keep the `.json` file somewhere safe.

---

## 🏗️ Tech Stack

| | |
|---|---|
| **Framework** | None — plain HTML, CSS, and vanilla JavaScript |
| **Styling** | [Tailwind CSS](https://tailwindcss.com/) (CDN) |
| **Fonts** | [Inter](https://fonts.google.com/specimen/Inter) + [Fira Code](https://fonts.google.com/specimen/Fira+Code) (Google Fonts) |
| **PDF export** | [jsPDF](https://github.com/parallax/jsPDF) |
| **Image export** | [html2canvas](https://html2canvas.hertzen.com/) |
| **Touch drag-and-drop** | [DragDropTouch polyfill](https://github.com/bernardo-castilho/dragdroptouch) |
| **Theme** | Custom dark colour scheme |
| **Storage** | Browser `localStorage` |

---

## 🌐 Browser Support

| Browser | Supported |
|---|---|
| Chrome / Edge | ✅ Fully supported |
| Firefox | ✅ Fully supported |
| Safari (macOS) | ✅ Fully supported |
| Safari (iOS) | ✅ Teams; Seating desktop-only |
| Android Chrome | ✅ Teams; Seating desktop-only |

---

## ☕ Support

If you find this useful, consider buying me a coffee!

[![Ko-fi](https://img.shields.io/badge/Ko--fi-Support%20this%20project-F92672?style=for-the-badge&logo=ko-fi)](https://ko-fi.com/coolpuddytat)

---

## 📄 License

MIT — free to use, modify, and distribute. Attribution appreciated but not required.

---

_Built with ❤️ by [Jonathan Kung](https://ko-fi.com/coolpuddytat)_
