# VisIEon

## How to Run Locally (For Beginners)

1. Make sure all files are together:
   - `index.html`
   - `tm-my-image-model/` (with `model.json`, `metadata.json`, `weights.bin`)

2. Download and install Python:
   - Go to [python.org/downloads](https://www.python.org/downloads/)
   - Download and install Python (just click "Next" until done)

3. Open the folder with your files:
   - Find the folder with `index.html` and `tm-my-image-model`
   - Click the address bar, type `cmd`, and press Enter

4. Start the local server:
   - Type this and press Enter:
     ```sh
     python -m http.server
     ```

5. Open your browser and go to:
   - [http://localhost:8000](http://localhost:8000)

6. Allow camera access if prompted.

7. Click "Start Detection" to use the app!

---

## How to Deploy to Firebase Hosting

1. Create a Google Account if you don’t have one.
2. Go to [Firebase Console](https://console.firebase.google.com) and create a project.
3. Download and install [Node.js](https://nodejs.org) (LTS version).
4. Open your project folder in File Explorer, type `powershell` in the address bar, and press Enter.
5. Install Firebase CLI:
   ```powershell
   npm install -g firebase-tools
   ```
6. Login to Firebase:
   ```powershell
   firebase login
   ```
7. Initialize Firebase Hosting:
   ```powershell
   firebase init hosting
   ```
   - Choose your project
   - For "public" directory, type:
     ```
     .
     ```
   - Say "No" to single-page app rewrite
   - Say "No" to overwriting `index.html`
8. Deploy:
   ```powershell
   firebase deploy
   ```
9. Copy the Hosting URL shown in the terminal and share it!

---

If you get stuck, ask your team or supervisor for help.