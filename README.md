# Domain Adaptation with CNN Feature Extractors (DANN, CDAN+E)

This GitHub repository showcases source pretraining and domain adaptation experiments conducted using six selected Convolutional Neural Networks (CNNs) as feature extractors. Two adversarial domain adaptation algorithms are employed: **DANN** (Domain-Adversarial Neural Network) and **CDAN+E** (Conditional Adversarial Domain Adaptation with Entropy Conditioning).

---

## 📁 Main Notebooks (CNN Feature Extractors + DA)

These notebooks implement both source training and domain adaptation using the respective CNNs:

1. **[`EfficientNet-B0(Main).ipynb`](./EfficientNet-B0(Main).ipynb)**  
   → Implements experiments using EfficientNet-B0.

2. **[`Efn-V2-s(Main).ipynb`](./Efn-V2-s(Main).ipynb)**  
   → Uses EfficientNet-V2-S as the feature extractor.

3. **[`MobileNetV2(Main).ipynb`](./MobileNetV2(Main).ipynb)**  
   → Experiments with MobileNetV2.

4. **[`ResNet-50(Main).ipynb`](./ResNet-50(Main).ipynb)**  
   → Implements experiments using ResNet-50.

5. **[`VGG19(Main).ipynb`](./VGG19(Main).ipynb)**  
   → Uses the classical VGG-19 architecture.

6. **[`VE_25_(Main)_aka_VefNet.ipynb`](./VE_25_(Main)_aka_VefNet.ipynb)**  
   → Code for the **proposed VEfNet CNN**, former working title was "VE-25". *Note: internal functions still retain the old name.*

---

## 🔗 Google Drive Resources

### 1. 📊 **Results Folder**  
[📎 Click to access → `Results`](https://drive.google.com/drive/folders/1sUrG91pbynsXKwgW9rdNwG9o7pSBQorj?usp=sharing)

#### ─ Source Training:
- `Checkpoints/` → `.pth` files for all optimizers and epochs (excluding top-5 selected ones).
- `Performance Metrics/` → Excel sheets summarizing training and test accuracies.
- `Confusion Matrices/` → `.png` images of confusion matrices at epoch 40 for all optimizers.

#### ─ Domain Adaptation:
- `DANN/` and `CDAN+E/` → Algorithm-specific subfolders:
  - `Confusion Matrices/` → `.png` images across lambdas and top-5 source checkpoints.
  - `Performance Metrics/` → Excel files and inference time summaries.
- `Source Checkpoints/` → `.pth` files for the top-5 CNN checkpoints used in DA.

---

### 2. ⚙️ **Code Execution Files**  
[📎 Click to access → `Executions`](https://drive.google.com/drive/u/1/folders/1lwaAJ4xk0awj1sBNyT4gjSDLr9uHE1H6)

- `CNN(Main).ipynb` → Full training + adaptation pipeline for each CNN.
- `CNNInftimesfor100imgs.ipynb` → Measures inference latency across 100 images.

---

### 3. 🧪 **Dataset Selection Codes**  
[📎 Click to access → `Data Selection`](https://drive.google.com/drive/folders/1VVcgzQeZUrD_yDdqH0WvBCrc0jUlpESX?usp=sharing)

- `Set-2/` → Code for Dataset 2 preparation.
- `Set-3/` → Code for Dataset 3 preparation.
- `Set-4/` → Final dataset (Dataset 4) preparation.

> ⚠️ *Dataset 1 (used in Trimester-2) underwent only size and channel conversions. So, it is ignored here.*

---

### 4. 📈 **Data Analysis Notebooks & Reports**  
[📎 Click to access → `Data Analysis`](https://drive.google.com/drive/folders/1XbScRt2e3-lQRTLE_oeYbsFaX-mtMrNC?usp=sharing)

- `DANN/` → Top-5 CNN performance evaluations based on DANN results.
- `CDAN+E/` → Analysis focused on CDAN+E results.
- `Overall Analysis/` → Trends, dataset selection logic, and comparison with earlier trimester outcomes.

---


All supplementary data, visualizations, and raw model checkpoints are accessible via the above Drive links.
