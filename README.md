# Landscape Mini — Simple Colab Notebook

A compact, reproducible Google Colab project for **landscape image classification**. The notebook shows a clean end‑to‑end flow: dataset setup, training, evaluation, and quick demo exports/screenshots.

> **Notebook:** `LandScape_Mini_Colab.ipynb`

---

## ✨ Highlights

- **Self‑contained Colab**: one notebook to train, evaluate, and demo.
- **Reproducible**: deterministic seeds where feasible; pip cell lists all deps.
- **Portable**: works on Colab free tier; easy to adapt locally.
- **Visual results**: Gradio Deployment (see screenshots).

---

## 📁 Project Structure

```
.
├── LandScape_Mini_Simple_Colab.ipynb
├── README.md
└── images/
    ├── screenshot1.png         
    ├── screenshot2.png        
    └── screenshot3.png
```

> Put your screenshots in `images/` and keep the same names or update paths below.

---

## 🧰 Requirements

- **Google Colab** (recommended), or
- **Python 3.10+** with the libs used in the notebook (PyTorch/TensorFlow/etc. — see the first install cell in the notebook).

---

## 🚀 Getting Started (Colab)

1. Open the notebook directly in Colab:
   - From GitHub: `Open in Colab` → (or) upload the `.ipynb` to Colab.
2. Run the setup cells (they will install dependencies).
3. Provide or download the dataset as described in the notebook.
4. Run the training section and then evaluation.
5. Save screenshots for your results and place them under `images/` for the README.

---


## 🧪 Reproduce Locally (Optional)

If you prefer to run outside Colab:

```bash
# Create and activate a virtual environment (Unix/macOS)
python -m venv .venv
source ./.venv/bin/activate

# Windows (PowerShell)
# python -m venv .venv
# .\.venv\Scripts\Activate.ps1

# Install the notebook dependencies (copy from the first pip cell in the notebook)
pip install -r requirements.txt  # if you export one
# or paste the 'pip install ...' commands from the notebook
```

Then run Jupyter or VS Code and open `LandScape_Mini_Colab.ipynb`.

---

## 🧩 Tips

- Keep the dataset path configurable in a single cell.
- Use `torch.inference_mode()` / `model.eval()` for deterministic eval.
- Save `state_dict` for faster re‑runs.
- If you store many artifacts, consider `.gitignore` and/or Git LFS.

