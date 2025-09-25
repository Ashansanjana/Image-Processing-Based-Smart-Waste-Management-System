# ♻️ Image Processing Based Smart Waste Management System

An intelligent web application for automated waste classification using deep learning and real-time object detection. Users can upload images of waste items or use their camera for live detection, helping to identify recyclable and non-recyclable materials to streamline waste management and promote environmental sustainability.

---

## 🚀 Features

- **Image Classification:** Upload waste images to predict their category (e.g., plastic, metal, glass, trash, etc.).
- **Real-Time Detection:** Use your device camera for live waste detection with bounding boxes and labels.
- **Statistics Dashboard:** Visualize classification statistics with interactive charts. 
- **Downloadable Reports:** Export classification results as CSV or PDF for record-keeping and analysis.
- **Modern UI:** Clean, responsive interface powered by Bootstrap.

---

## 🏗️ How It Works

The system is powered by:
- **EfficientNet-B0 Keras Model:** For image classification of waste types.
- **YOLOv8 Model:** For real-time object detection using your camera.
- **Flask Web Server:** Handles user requests and serves the web app.
- **Matplotlib & FPDF:** For chart visualization and PDF report generation.

Waste items are categorized into recyclable (plastic, glass, metal, paper, cardboard) and non-recyclable (trash, biological, shoes) classes. The models are pre-trained and loaded at startup.

---

## 📦 Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/UdaraChamidu/Image-Processing-Based-Smart-Waste-Management-System.git
   cd Image-Processing-Based-Smart-Waste-Management-System/waste detection app
   ```

2. **Install dependencies:**
   > Create and activate a virtual environment for best results.
   ```bash
   pip install -r requirements.txt
   ```

3. **Model Files:**
   - Ensure the following model files exist at the specified paths in `app.py`:
     - EfficientNet model: `efficientnet_b0_best.keras`
     - YOLOv8 model: `best.pt`
   - Update the file paths in `app.py` as needed for your environment.

---

## 🖥️ Usage

1. **Run the Flask app:**
   ```bash
   python app.py
   ```

2. **Open your browser:**
   - Visit [Real time Smart Waste Classification](https://huggingface.co/spaces/UdaraChamidu/Image-Processing-Based-Smart-Waste-Management-System)

3. **Main Features:**
   - **Upload Image:** Classify waste by uploading an image.
   - **Camera Detection:** Click "Use Camera for Real-Time Detection" for live classification.
   - **View Statistics:** Check cumulative classification stats and download reports (CSV/PDF).

---

## 📁 Project Structure

```
waste detection app/
│
├── app.py                  # Main Flask backend
├── requirements.txt        # Python dependencies
├── efficientnet_b0_best.keras   # Keras classification model (not included)
├── best.pt                 # YOLOv8 detection model (not included)
├── templates/              # HTML templates for UI
│   ├── index.html
│   ├── camera.html
│   ├── result.html
│   └── report.html
├── static/
│   ├── uploads/            # Uploaded images
│   └── stats_chart.png     # Generated statistics chart
├── waste_log.csv           # Classification log (generated)
├── waste_report.pdf        # PDF report (generated)
```

---

## 🛠️ Requirements

- Python 3.8+
- See [requirements.txt](./requirements.txt) for all packages.

**Major libraries:**
- Flask
- TensorFlow / Keras
- OpenCV
- Ultralytics (YOLO)
- Matplotlib
- FPDF

---

## 📷 Screenshots

### 🏠 Home Page  

<p align="center">✨ User-friendly landing page with image upload and classification entry point.</p>

<p align="center">
  <img width="835" height="527" alt="image" src="https://github.com/user-attachments/assets/ad12d4c9-9ee5-44c1-8a78-f403f6131417" />
</p>

---

### 🧾 Classification Result  

<p align="center">🔍 Displays predicted disease type with probability scores and model insights.</p>

<p align="center">
  <img width="578" height="572" alt="image" src="https://github.com/user-attachments/assets/a386c08a-6f5b-476a-8b3b-14e289bb6c8b" />
</p>

---

### 📊 Statistics Dashboard  

<p align="center">📈 Interactive dashboard showing model performance metrics, accuracy distribution, and detailed statistics.</p>

<p align="center">
  <img width="787" height="850" alt="image" src="https://github.com/user-attachments/assets/5bead5a9-fbbf-470d-be6c-0ca24adab5ae" />
</p>


## 👤 Authors

Developed by [Udara Chamidu](https://github.com/UdaraChamidu) and [Ashan Sanjana](https://github.com/Ashansanjana)))

---

## 🤝 Contributing

Pull requests and suggestions are welcome! For major changes, open an issue first to discuss what you would like to change.

---

## ⚠️ Notes

- **Model files are not included due to size.** You must train or obtain your own models and update their paths in `app.py`.
- For best camera results, use Chrome or Firefox. Some browsers may restrict webcam access.
- For deployment, set `debug=False` in `app.py`.

---

## 📬 Contact

For questions, reach out via [GitHub Issues](https://github.com/UdaraChamidu/Image-Processing-Based-Smart-Waste-Management-System/issues).
