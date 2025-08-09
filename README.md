#  AI Model for Predicting Airfoil Noise

Ever waited hours for a CFD simulation to finish?  
Yeah… I’m not about that life.  

This project is my proof-of-concept where an **AI neural network** predicts aerodynamic noise from an airfoil in **milliseconds** — skipping the painfully slow CFD wait time (and the multiple cups of coffee).  

---

## 🚀 Why I Made This

In aerospace/mechanical design, you change one parameter… then wait **forever** for simulations.  
My thought: **“What if AI could just guess the result instantly?”**  

With this model, you can:  
- Test **thousands** of design ideas in seconds  
- Throw out the bad ones immediately  
- Only run expensive CFD sims on the winners  

Think of it like a fast, lazy best friend for your design process.

---

## 🛠 Tech Stack

- **Python** – the brain 🧠  
- **TensorFlow / Keras** – AI shiii  
- **Pandas** – data wrangling like a pro 
- **Scikit-learn** – preprocessing sidekick
- **Matplotlib** – making graphs look pretty   
- **Jupyter Notebook** 

---

## 📊 Dataset

Trained on the *Airfoil Self-Noise* dataset (wind tunnel tests).  

**Inputs:**  
- `f`: Frequency (Hz)  
- `alpha`: Angle of attack (°)  
- `c`: Chord length (m)  
- `U_infinity`: Free-stream velocity (m/s)  
- `delta`: Suction side displacement thickness (m)  

**Output:**  
- `SSPL`: Scaled sound pressure level (dB) — basically, loudness.

---

## 🖥 How to Run

1️⃣ **Clone the repo**  
```bash
git clone https://github.com/achadevansh/fuild_ai_project2.git
cd fuild_ai_project2

# Install dependencies and run the notebook
pip install -r requirements.txt && jupyter notebook notebooks/run_global_prediction.ipynb
