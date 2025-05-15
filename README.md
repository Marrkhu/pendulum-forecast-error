# pendulum-forecast-error

## **Overview**
This notebook discusses predicted vs. true trajectories of a double-pendulum model and analyses prediction error over varying horizons.

---

## **Objectives**
- Compare predicted and true (x, y) coordinates for both masses  
- Analyse amplitude and phase fidelity in oscillatory paths  
- Compute MSE across multiple forecast horizons (20–100 steps)  
- Identify trends and optimal horizons for accurate prediction

---

## **Methodology**
- **Visual Comparison:**  
  - Plot true vs. predicted x₁, x₂ and y₁, y₂ time-series  

- **Error Analysis:**  
  - Calculate MSE for horizons in defined range  
  - Summarise key dips and peaks in error curves  

- **Structured Discussion:**  
  - Highlight coordinate-specific accuracy (x vs. y)  
  - Note phase shifts, amplitude deviations, and overall trends

---

## **Key Results**
- **x-Coordinates:** Predicted with higher fidelity and smoother errors  
- **y-Coordinates:** Exhibited larger phase shifts and amplitude errors  
- **MSE Trends:**  
  - High initial error at 20 steps (> 1.2)  
  - Pronounced dip near 40 steps (< 0.7)  
  - Fluctuations thereafter, with errors settling near ~0.9 for longer horizons  

---

## **Limitations & Future Work**
- y-axis variability suggests need for richer input features  
- Longer horizons degrade accuracy; consider physics-informed or deeper models  
- Investigate regularisation and noise-robust training regimes

