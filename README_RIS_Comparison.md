
# 📄 README: Comparison Between Single RIS and Dual RIS Performance

## 📘 Overview
This analysis compares the performance of a **Single RIS** (Reconfigurable Intelligent Surface) versus a **Dual RIS** communication system using three key performance graphs:

1. **Bit Error Rate (BER) vs Distance \( L \)**  
2. **BER vs Signal-to-Noise Ratio (SNR)**  
3. **Loss vs Epoch** during training (for deep learning-based RIS control)

---

## 📊 1. BER vs Distance \( L \)

### ✅ What it Shows:
- How the **Bit Error Rate (BER)** increases as the **user moves farther** from the Base Station (BS).

### 📈 Observation:
| Metric        | Single RIS                    | Dual RIS                         |
|---------------|-------------------------------|----------------------------------|
| BER Increase  | Moderate with distance         | Slower increase (flatter curve)  |
| Coverage      | Limited to medium range        | Extended range with good BER     |

### 🔍 Insight:
The **dual RIS system** maintains better signal strength and link quality over longer distances, thanks to **multiple reflection paths**, reducing BER even at 100+ meters.

---

## 📉 2. BER vs SNR

### ✅ What it Shows:
- How the system performs under **varying noise conditions** (measured in dB SNR)

### 📈 Observation:
| Metric         | Single RIS                 | Dual RIS                         |
|----------------|----------------------------|----------------------------------|
| BER Drop       | Sharp but saturates early  | Faster and deeper BER drop       |
| Low SNR Region | Higher BER                 | Significantly better BER         |

### 🔍 Insight:
With **dual RIS**, the system achieves **higher SNR diversity**, resulting in **more reliable communication** even under noisy environments.

---

## 🧠 3. Loss vs Epoch (Training Curve)

### ✅ What it Shows:
- How the training loss decreases over **epochs** during a neural network-based optimization of RIS phase shifts.

### 📈 Observation:
| Metric       | Single RIS              | Dual RIS                       |
|--------------|-------------------------|--------------------------------|
| Convergence  | Slightly slower         | Faster loss convergence        |
| Final Loss   | Higher loss floor       | Lower loss (better optimization) |

### 🔍 Insight:
Dual RIS setups benefit from **richer input-output signal interactions**, allowing deep learning models to **learn faster and generalize better**.

---

## ✅ Final Summary

| Feature                  | Single RIS               | Dual RIS                         |
|--------------------------|--------------------------|----------------------------------|
| BER vs Distance          | Good in medium range     | Best for long range              |
| BER vs SNR               | Moderate improvement     | Strong improvement at all SNRs   |
| Training Loss            | Decent convergence       | Faster, smoother convergence     |

---

## 📂 File References
- `ber_vs_distance.png`: Shows how BER increases with distance for each configuration  
- `ber_vs_snr.png`: Compares BER for varying SNR values  
- `loss_vs_epoch.png`: Visualizes training efficiency of DL models for RIS optimization

- A single RIS (Reconfigurable Intelligent Surface) system uses one intelligent surface to reflect and manipulate the wireless signals to improve communication quality, such as enhancing signal strength or reducing interference in a specific area. It is simpler to deploy and control, making it suitable for scenarios where signal enhancement is needed in a localized region. On the other hand, a 2 RIS system involves two separate intelligent surfaces placed at different locations. This setup allows for more advanced manipulation of wireless signals by reflecting them multiple times, which can extend coverage, improve signal reliability, and handle more complex environments where obstacles block direct communication paths. Although 2 RIS systems provide better overall performance through multi-hop signal reflection and increased control over the wireless environment, they are more complex to coordinate and manage compared to a single RIS. Therefore, single RIS is ideal for basic enhancements, while 2 RIS is better suited for more demanding use cases requiring extended range or improved connectivity.









