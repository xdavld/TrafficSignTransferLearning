# Transfer Learning for Different Traffic Signs

This notebook investigates the effectiveness of transfer learning for traffic sign recognition across different geographic domains. Specifically, it explores how well a model trained on the German GTSRB dataset transfers to the U.S.-based LISA dataset.

## 🧪 Experiment Setup

- **Base architecture:** ResNet-50
- **Pretraining:** ImageNet
- **Source dataset:** GTSRB (Germany)
- **Target dataset:** LISA (USA)
- **Approaches compared:**
  - Training from scratch on LISA with varying data fractions
  - Head-only fine-tuning using a ResNet-50 pretrained on GTSRB

## 📊 Evaluation

- Performance evaluated at 1%, 5%, 10%, 25%, 50%, 75%, and 100% of LISA training data.
- Metrics:
  - Overall test accuracy
  - Per-class accuracy
  - Comparative heatmaps
- Results highlight the effectiveness of transfer learning under low-data regimes (up to 5%), and the advantage of full training as data increases.

## 🚀 Requirements

- Python 3.9+
- PyTorch
- torchvision
- matplotlib
- pandas
- numpy

## 🔍 Usage

Run the notebook to:
- Train ResNet-50 models on LISA from scratch and via transfer learning
- Analyze performance trends under varying data availability
- Visualize class-level differences in transfer effectiveness

## 📝 Citation

If you use this notebook for academic or educational purposes, please consider citing the datasets:

- GTSRB: [Stallkamp et al., 2011](https://benchmark.ini.rub.de/?section=gtsrb&subsection=dataset)
- LISA: [Mogelmose et al., 2012](https://cvrr.ucsd.edu/LISA/lisa-traffic-sign-dataset.html)

## 📬 Contact

Feel free to reach out if you have questions or suggestions!
