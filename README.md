# 🚀 Moon Orbital Distance Prediction with PyTorch

This project uses a basic neural network built in **PyTorch** to predict the orbital distance of natural satellites (moons) based on input features like diameter and host planet mass.

## 🧠 What This Is

This is a minimal machine learning model that demonstrates:

- Data preprocessing with `pandas`
- Tensor conversion and normalization
- A simple `torch.nn.Sequential` model
- A full PyTorch training loop
- Visualization of training loss with `matplotlib`

## 🌌 Dataset (Toy)

A small dataset was constructed with orbital and physical data from:

| Moon          | Diameter (km) | Host Planet | Planet Mass (kg) | Orbital Distance (km) |
|---------------|---------------|-------------|------------------|------------------------|
| Phobos        | 22.4          | Mars        | 6.39e23          | 9,376                  |
| Deimos        | 12.4          | Mars        | 6.39e23          | 23,463                 |
| Earth’s Moon  | 3475          | Earth       | 5.97e24          | 384,400                |

All values were normalized for training.

## 🔁 Training Details

- Framework: PyTorch
- Epochs: `80,000` for fine-tuning small-scale convergence
- Loss Function: Mean Squared Error (`MSELoss`)
- Optimizer: Adam (`lr = 0.01`)
- Final output: normalized orbital distances

## 📉 Sample Loss Plot

Training loss is visualized with `matplotlib` to track convergence:

![loss_plot](./images/loss_plot.png)

## ✨ Future Improvements

- Add real planetary datasets from NASA/JPL
- Introduce classification (e.g. predict moon type)
- Expand to exomoons or asteroid data
- Add Streamlit app for live prediction

## 🛠 How to Run

```bash
pip install torch pandas matplotlib
python moon_orbit_predictor.py

