# 🎮 Day 20 — Face Puzzle Game

A fully interactive **Face Puzzle Game** built as a single self-contained HTML application using **HTML, CSS, and JavaScript**.

The game uses the device webcam to capture a face photo and converts it into an interactive puzzle with multiple difficulty levels.

## ✨ Features

* 📷 Webcam access using `getUserMedia()`
* 🤳 Live front-camera preview
* 📸 Capture a photo directly from the camera
* 🧩 3×3, 4×4, and 5×5 puzzle difficulties
* 🔀 Randomly scrambled puzzle pieces
* 🖱️ Mouse drag-and-drop support
* 📱 Touch drag support for mobile/tablet
* 🎯 Automatic snapping and piece swapping
* 🟢 Correctly positioned piece highlighting
* ⏱️ Live timer in `mm:ss.t` format
* 🔢 Move counter
* ✅ Correctly placed pieces counter
* 🏆 Automatic win detection
* 🎉 Results screen after completing the puzzle
* 💾 Top 5 scores saved using `localStorage`
* 📊 Leaderboard with time, moves, difficulty, and date
* 🔄 Retake Photo option
* ▶️ Play Again option
* 🆕 New Photo option
* 📱 Responsive mobile-friendly interface
* 🌐 Compatible with modern Chrome, Firefox, and Safari
* 🔒 Camera access supported over HTTPS or localhost
* ⚠️ Graceful handling of denied camera permissions

## 🛠️ Technologies Used

* HTML5
* CSS3
* JavaScript
* WebRTC `getUserMedia()` API
* HTML5 Canvas API
* Browser Local Storage API
* Pointer/Touch interaction APIs

## 🎯 How It Works

1. Allow camera permission when prompted.
2. The application displays a live webcam preview.
3. Click **Take Photo** to capture your face.
4. Select a puzzle difficulty:

   * **3×3** — Easy
   * **4×4** — Medium
   * **5×5** — Hard
5. The captured image is divided into equal puzzle pieces.
6. The pieces are randomly scrambled.
7. Drag and drop pieces to swap their positions.
8. Correctly positioned pieces are highlighted.
9. The timer tracks completion time while the move counter records moves.
10. Once every piece reaches its correct position, the game automatically detects the win.
11. Your result is displayed with:

    * Final time
    * Number of moves
    * Difficulty
12. The best five results are stored locally and displayed on the leaderboard.



## 🚀 How to Run

### Option 1 — GitHub Pages

Upload `face-puzzle-game.html` to your GitHub repository and enable **GitHub Pages**.

Open the deployed page in a browser and allow camera permission.

### Option 2 — Localhost

Run the HTML file through a local development server.

For example, using VS Code Live Server:

```text
Right Click → Open with Live Server
```

Then open the generated localhost URL in your browser.

> Camera access generally requires **HTTPS or localhost**. Opening the HTML directly using `file://` may prevent webcam access in some browsers.

## 📸 Testing Checklist

* [ ] Webcam permission request
* [ ] Live camera preview
* [ ] Photo capture
* [ ] Retake Photo functionality
* [ ] 3×3 puzzle generation
* [ ] 4×4 puzzle generation
* [ ] 5×5 puzzle generation
* [ ] Puzzle scrambling
* [ ] Mouse drag-and-drop
* [ ] Touch interaction
* [ ] Piece swapping
* [ ] Correct-position highlighting
* [ ] Timer functionality
* [ ] Move counter
* [ ] Correct-piece counter
* [ ] Automatic win detection
* [ ] Results overlay
* [ ] Leaderboard
* [ ] LocalStorage score persistence
* [ ] Play Again functionality
* [ ] New Photo functionality
* [ ] Responsive mobile layout
* [ ] Camera permission denial handling

## 🧠 Key Learnings

### 1. Webcam Integration

Learned how to use the browser's `getUserMedia()` API to request camera access and display a live video stream.

### 2. Canvas Image Processing

The captured webcam image is drawn onto a canvas and divided into equal sections to create puzzle pieces.

### 3. Drag-and-Drop Interaction

Implemented interactive puzzle movement using pointer/touch events so the game can work across desktop and mobile devices.

### 4. Puzzle State Management

Each tile maintains its original position and current position, making it possible to determine whether a piece is correctly placed.

### 5. Game Logic

The application tracks:

* Current puzzle state
* Number of moves
* Correctly positioned pieces
* Elapsed time
* Selected difficulty
* Game completion

### 6. LocalStorage

The leaderboard demonstrates how browser `localStorage` can be used to persist game results without requiring a backend database.

### 7. Responsive UI

The interface was designed to adapt to different screen sizes, making the game usable on desktops, tablets, and smartphones.

## 💡 Future Improvements

* 🏅 Difficulty-specific leaderboards
* 👤 Face detection using a browser-based AI model
* 🔊 Sound effects
* 🎵 Background music
* 🌟 More animation effects
* 🎨 Custom puzzle themes
* 📈 Player statistics
* 🔥 Streak system
* 🌍 Global online leaderboard
* 👥 Multiplayer mode
* 🧠 AI-generated puzzle difficulty
* 🏆 Achievement and badge system

## 📌 Project Goal

The goal of this project was to build an engaging browser-based game while practicing:

**Webcam APIs + Canvas + JavaScript Game Logic + Drag & Drop + Touch Interaction + LocalStorage + Responsive UI**

This project was completed as part of **ABTalks Day 20**.

## 👩‍💻 Author

**Neha Duggal**

B.Tech CSE — AI & ML
Interested in Web Development, AI/ML, Data Analytics, and Generative AI.

## ⭐ Project Highlights

> Capture your face → Choose difficulty → Solve the puzzle → Beat your best time! 🎯

**Day 20 successfully completed 🚀**

