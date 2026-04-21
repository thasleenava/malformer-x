# MalFormer-X: Malware Detection using Graph Neural Networks and Transformers

##  Overview
MalFormer-X is a hybrid deep learning framework designed for malware detection using memory analysis. The model combines Graph Neural Networks (GNNs) and Transformer architectures to capture both structural and sequential patterns in memory data.

##  Key Features
- Binary Classification: Benign vs Malware
- Multi-class Classification: Ransomware, Trojan, Spyware, Benign
- Graph-based feature representation
- Transformer-based sequence modeling
- Explainable AI:
  - SHAP (global feature importance)
  - LIME (local explanation)
  - Attention visualization

## Dataset
- CIC-MalMem-2022 (memory-based malware dataset)
- Features extracted from process, DLL, handles, and API behavior

##  Methodology
1. Data preprocessing and feature selection (Mutual Information + Top-K)
2. Graph construction from memory features
3. Hybrid model:
   - GAT + GIN (graph learning)
   - Transformer (sequence modeling)
   - Cross-attention fusion
4. Multi-task learning:
   - Binary detection
   - Multi-class classification

##  Results
- Binary F1-score: ~1.00
- Multi-class F1-macro: ~0.74
- AUC-ROC: up to 0.94+

##  Explainability
- SHAP: Global feature importance
- LIME: Instance-level explanations
- Attention maps: Model interpretability

##  Technologies
- Python
- PyTorch
- PyTorch Geometric
- Scikit-learn
- SHAP, LIME

##  How to Run
1. Open the notebook in Google Colab
2. Upload the CIC-MalMem dataset
3. Run all cells sequentially

##  Future Work
- Real-time malware detection
- Advanced XAI integration
- Deployment as a security tool

##  Author
Thasleena V A  
Research Scholar, Karunya Institute of Technology and Science
