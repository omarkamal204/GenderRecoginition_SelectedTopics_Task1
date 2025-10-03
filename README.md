# Gender Classification Model

A simple **gender classification model** built with **Teachable Machine** and **TensorFlow.js**.  
Runs directly in the browser using webcam input.

## How it works
- Trained with Teachable Machine (Image Model).
- Exports are stored in `my_model/` (`model.json`, `metadata.json`, weights).
- HTML + JavaScript frontend loads the model and predicts in real-time.

## Run Locally
- With **Node.js** (from project folder):
    
    ```bash
    npx serve
    ```

- Or with **Python** (from project folder):

    ```bash
    python -m http.server 8000
    ```

Then open in browser:
http://localhost:3000/index.html

(Replace `index.html` with your actual HTML filename if different.)

## Features
- Real-time webcam input.
- Live prediction showing class name & probability.
- 100% client-side (runs in the browser, no backend required).

## Files
- `index.html` — frontend that loads the model and shows predictions.  
- `my_model/` — exported model directory (`model.json`, `metadata.json`, weights files).

## Notes
- Serve the project via a local server (don't open the HTML via `file://`) so the model files load correctly.
- The page will request camera permission when you click **Start**.
- If model fails to load, check browser console for CORS/path errors and ensure `my_model/` is next to the HTML file.

---

## Course Info
- **4th Year - Computer Science Department**  
- **Selected Topics Course**  
- **Supervised by:** Dr. Ahmed Tolba
