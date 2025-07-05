# Real-Time Age and Gender Detection Using OpenCV

This project performs **face detection**, and predicts **age** and **gender** of individuals in images using **OpenCV's deep learning module** (`cv2.dnn`). It uses pre-trained Caffe models for inference, making it fast and accurate even on local machines.

## 🧠 What It Does

- Detects human faces in an image
- Classifies age groups (e.g., 25–32, 38–43, etc.)
- Classifies gender (Male / Female)
- Annotates images with bounding boxes and predictions
- Can be adapted for webcam-based real-time detection

## 🖼️ Example Output

> ![Example](example_output.jpg)  
> _(Face with bounding box showing predicted age and gender)_

## 🗂️ Project Structure

```bash
📦 age-gender-detection/
├── san12.ipynb                # Main Jupyter notebook
├── age_deploy.prototxt        # Age model config
├── age_net.caffemodel         # Age model weights
├── gender_deploy.prototxt     # Gender model config
├── gender_net.caffemodel      # Gender model weights
├── opencv_face_detector.pbtxt # Face detector config
├── opencv_face_detector_uint8.pb # Face detector weights
├── _DSC0029.JPG               # Sample image (can be replaced)
├── requirements.txt           # Python dependencies
└── README.md                  # Project overview

🛠️ Installation
Install dependencies with pip:

pip install opencv-python opencv-contrib-python matplotlib numpy

 you're using Jupyter Notebook:

pip install notebook

🚀 How to Run

Clone the repository:

git clone https://github.com/your-username/age-gender-detection.git
cd age-gender-detection

Open the notebook:

bash
Copy
Edit
jupyter notebook san12.ipynb
Run all cells. Make sure the required model files (.prototxt, .caffemodel, etc.) are in the same folder.

You can replace the image _DSC0029.JPG with your own.

🧑 Age Categories Used
(0–2), (4–6), (8–12), (15–20)

(25–32), (38–43), (48–53), (60–100)

👩‍🦱 Gender Categories
Male

Female

💡 Future Improvements
Add webcam support for live detection

Create a simple web interface with Flask or Streamlit

Improve bounding box aesthetics and overlay styles

📝 License
This project is open source under the MIT License.

🙏 Acknowledgements
OpenCV DNN module

Pretrained models from LearnOpenCV

---

Would you also like me to generate a `requirements.txt` file and provide a `.gitignore` to make your repo cleaner?

