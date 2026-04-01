# 🛡️ CheckCam: AI Omni-Scanner & Surveillance
> **The future of web-based vision. Scan, Track, and Shop in real-time.**



![Scanning Status](https://img.shields.io/badge/SCANNER-ACTIVE-00e5ff?style=for-the-badge&logo=target)
![AI Engine](https://img.shields.io/badge/ENGINE-TENSORFLOW.JS-orange?style=for-the-badge&logo=tensorflow)
![Deployment](https://img.shields.io/badge/DEPLOYED-GITHUB_PAGES-2ea44f?style=for-the-badge&logo=github)

---

## 📽️ UI Animation & Experience
CheckCam isn't just a tool; it's an experience. The interface features:
* **The Neon Pulse:** A constant laser-line scan that pulses across the camera feed.
* **Dynamic HUD:** Real-time data overlays that change color based on target type (Security Green for humans, Retail Blue for objects).
* **Smooth Transitions:** Reporting cards that slide into the sidebar with CSS motion effects.

---

## 🚀 Key Features

* **📡 Real-time Neural Scanning:** Identifies 80+ object classes directly in the browser.
* **🌊 Laser Wave Animation:** A sleek, CSS-animated scanning bar that gives the visual feel of high-end hardware.
* **👥 Presence Tracking:** Specialized logic to detect when a **Human** or **Animal** enters or departs.
* **📊 Retail Intelligence:** Automatically generates Google Shopping links for detected objects.
* **📑 Activity Logging:** A sidebar "Session Report" that timestamps every event.

---

## 🛠️ Technology Stack

| Component | Technology |
| :--- | :--- |
| **Frontend** | HTML5, CSS3 (Keyframe Animations), JS |
| **AI Engine** | [TensorFlow.js](https://www.tensorflow.org/js) |
| **Model** | COCO-SSD (Object Detection) |
| **Search** | Google Shopping Integration |

---

## 📸 How It Works

1.  **Boot Sequence:** The user initializes the system via a glowing "ACTIVATE" button.
2.  **Neural Loop:** The system captures frames and runs them through the COCO-SSD model.
3.  **Surveillance:** * **Arrivals:** Logged when a new person is identified.
    * **Departures:** Logged when the person leaves the frame for > 2 seconds.
4.  **Retail:** Instant "Buy" links appear for inanimate objects.

---

## 📂 Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/xkrishmishra/CheckCam.git](https://github.com/xkrishmishra/CheckCam.git)
    ```
2.  **Run Local Server:**
    * **VS Code:** Use the **Live Server** extension.
    * **Python:** `python -m http.server 8000`
3.  **Live Site:** [Visit CheckCam](https://xkrishmishra.github.io/CheckCam/)

---

## 📝 Configuration

Adjust the **Detection Sensitivity** in your script to fine-tune the AI:

```javascript
if (prediction.score > 0.65) { 
    // 0.65 is the "Sweet Spot" for animation stability
}
