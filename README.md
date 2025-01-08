
```markdown
# 🐦 Bird Species Classification - Kaggle Competition 2025

## Description
This repository contains my work for the Kaggle competition **[Bird Species Classification](https://www.kaggle.com/competitions/m-2-bdia-dlia-project-2025)**.
Project in Deep Learning for Image Analysis. The objective is to build and fine-tune models to classify bird species with the highest possible accuracy on a test dataset. The dataset used is a subset of the **Caltech-UCSD Birds-200-2011** dataset, limited to 30 categories.

---

## Dataset
The dataset consists of:
- **Training Set**: 2500+ images with labels.
- **Validation Set**: 240+ images with labels.
- **Test Set**: 600+ images for which categories are to be inferred.

---

## Models Trained
The following models were fine-tuned using PyTorch:
1. **EfficientNet-B4**
   - Best accuracy on validation: **82%**
2. **ResNet101**


---

## Results
| Model         | Validation Accuracy |
|---------------|---------------------|
| EfficientNet  | 82%                |
| ResNet101     | 88%                |

---

## Installation
Clone the repository and install the required dependencies:

```bash
git clone https://github.com/Rodmigniha/Bird-Species-Classification.git
cd Bird-Species-Classification
pip install -r requirements.txt
```

---

## Usage

1. **Download Dataset**  
   The dataset is hosted on Google Drive and can be downloaded and extracted using:
   ```python
   import gdown
   url = 'https://drive.google.com/uc?id=1k5_-HpkreEeIMMjlyW4JhuClyXJfhDDX'
   output = 'dataset.zip'
   gdown.download(url, output, quiet=False)
   !unzip dataset.zip -d ./data
   ```

2. **Run the Notebook**  
   Open and execute the Jupyter Notebook to train and evaluate the models:
   ```bash
   jupyter notebook Bird_Classification.ipynb
   ```

3. **Inference**  
   Generate predictions for the test set using the trained models. Sample inference script is provided for each model.

---

## File Structure
```
Bird-Species-Classification/
├── data/
│   ├── train_images/
│   ├── val_images/
│   ├── test_images/
│   └── class_indexes.csv
├── Bird_Classification.ipynb
├── kaggle-efficientnet.csv
├── kaggle-resnet101.csv
├── kaggle-resnet152.csv
├── README.md
├── requirements.txt
└── .gitignore
```

---

## Authors
- **Rodrigue MIGNIHA**

---

```

---

### **requirements.txt**

```
torch==2.0.1
torchvision==0.15.2
timm==0.6.13
pytorch-lightning==2.0.5
matplotlib==3.7.2
numpy==1.23.5
pandas==2.1.1
opencv-python==4.8.1
Pillow==9.5.0
tensorboard==2.14.1
gdown==4.7.1
```

---

### **.gitignore**
Pour ignorer les fichiers inutiles ou sensibles, utilisez le fichier `.gitignore` suivant :

```
# Byte-compiled / optimized / DLL files
__pycache__/
*.py[cod]
*.so

# Data files
data/
*.zip
*.csv

# Logs and TensorBoard files
logs/
runs/

# Virtual environment
.env/
.venv/

# Jupyter Notebook checkpoints
.ipynb_checkpoints/

# OS-specific files
.DS_Store
Thumbs.db
```

---

### Étapes pour tout mettre sur GitHub
1. **Ajoutez les nouveaux fichiers** :
   ```bash
   git add README.md requirements.txt .gitignore
   ```

2. **Committez les changements** :
   ```bash
   git commit -m "Add README, requirements, and .gitignore"
   ```

3. **Poussez les fichiers sur GitHub** :
   ```bash
   git push origin main
   ```

Feel free to adjust any parts based on the final results or your preferences. Let me know if you need any further help! 😊

🛠 Contributions

Les contributions sont les bienvenues ! Veuillez ouvrir une issue ou soumettre une pull request pour toute amélioration ou suggestion.

🌐 Contact

Pour toute question ou demande de partenariat, n’hésitez pas à me contacter :

Email : rodrigue.migniha@dauphine.tn , kidam.migniha@gmail.com , rodrigue.pro2020@gmail.com
GitHub : https://github.com/Rodmigniha/Bird-Species-Classification.git


```

