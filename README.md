# NoCap – Capstone Motion Capture Project

NoCap is my experimental project and attempt in making motion capture more accessible, not a commercial product. The goal: let anyone capture body motion for animation or games with just a webcam and a browser, no special suits or expensive gear required.

---

## Project Overview

This project explores real-time, suitless motion capture using AI pose estimation in the browser. By leveraging open-source tools, NoCap enables users to record their movements and export them in formats suitable for animation or game development. It’s intended as a proof-of-concept and a learning experience in AI, web technologies, and interacting with hardware through the browser.

---

## Technologies Used

- **Frontend:** React + Vite (for quick development and hot-reloading)
- **Pose Tracking:** MediaPipe (Google’s real-time pose detection framework)
- **Styling:** CSS, with MUI for some UI elements (e.g., loading screens)
- **Export Formats:** JSON and BVH (for importing into most animation tools)

---

## Setup & Running Locally

If you’d like to try out NoCap or dig into the code:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/EverettHanke/NoCap.git
   cd NoCap
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Start the development server:**
   ```bash
   npm run dev
   ```

4. Open your browser to ```localhost:5173```

---

## How to Use

1. When prompted, allow the browser to access your camera.
2. Click "Enable Camera" to start tracking.
3. Move around in front of your webcam—your skeleton should be tracked in real time.
4. Stop recording and review your captured motion.
5. Export the animation data as JSON or BVH if you want to use it in other tools.

---

## Acknowledgments

- [MediaPipe](https://mediapipe.dev/) for pose detection

---

## Analysis of App’s Capabilities and Limitations

### Capabilities
- **Core Functionality:** The app successfully captures and keyframes animations via mediapipe and exports usable bvh files.
- **Usability:** Can easily record animations without spending a dime.
- **Integration:** Can be directly imported into any of your favorite animation studios (Blender, IClone, Rokoko, etc)

### Limitations
- **Feature Gaps:** Does not support more than one actor at a time.
- **Skill Gap:** Still requires you to manually add final touches. 

## Potential Future Improvements

**Expanded Feature Set:** 
- Implementing more accurate BVH data. Having the end product more retargetable to the UE skeleton without needing to modify bones
- Allowing users to select a skeleton heirarchy they wish to export to. (UE Maniquin, Mixamo skeleton, Unity skeleton, etc.)

---