# Melanoma Cancer Detection - Jupyter Notebook

This project demonstrates a CNN-based solution for melanoma cancer detection using medical images. The notebook contains multiple model architectures and training approaches for skin cancer classification.

## 📋 Prerequisites

### System Requirements
- **OS**: Linux (WSL2 recommended for Windows users)
- **Python**: 3.10 or 3.12 (as tested in the notebook)
- **GPU**: NVIDIA GPU with CUDA support (RTX 4070 SUPER tested)
- **RAM**: Minimum 8GB, recommended 16GB+
- **Storage**: At least 5GB free space for dataset and models

### Hardware Requirements
- **GPU**: NVIDIA GPU with CUDA 12.x support
- **VRAM**: Minimum 4GB, recommended 8GB+
- **CPU**: Multi-core processor (for CPU fallback)

## 🚀 Installation Guide

### 1. Clone the Repository
```bash
git clone <repository-url>
cd <repository>
```

### 2. Create Virtual Environment
```bash
# Create virtual environment
python3 -m venv .venv

# Activate virtual environment
source .venv/bin/activate  # Linux/Mac
# or
.venv\Scripts\activate     # Windows
```

### 3. Install Dependencies

#### Option A: Install with CUDA Support (Recommended for GPU)
```bash
# Install TensorFlow with CUDA support
python3 -m pip install tensorflow[and-cuda]

# Install other dependencies
pip install -r requirements.txt
```

#### Option B: Install CPU-only Version
```bash
# Install TensorFlow CPU version
pip install tensorflow

# Install other dependencies
pip install -r requirements.txt
```

### 4. Verify Installation
```bash
# Verify TensorFlow installation
python3 -c "import tensorflow as tf; print('TensorFlow version:', tf.__version__)"

# Verify GPU detection (if using GPU)
python3 -c "import tensorflow as tf; print('GPU devices:', tf.config.list_physical_devices('GPU'))"
```