# AI Lab — Conda Environment

A reproducible Conda environment for AI/ML development with Python 3.12 and a broad set of tools for machine learning, deep learning, data science, NLP, computer vision, RAG, experimentation, and deployment.

## What's included

- **Python 3.12**
- **Machine Learning:** Scikit-learn, LightGBM, NumPy, SciPy, Pandas
- **Deep Learning:** TensorFlow (CPU), PyTorch (CPU), Keras
- **Graph ML:** PyTorch Geometric
- **NLP / Transformers:** Hugging Face Transformers, Tokenizers, Sentence Transformers
- **Computer Vision:** OpenCV
- **RAG / Vector Search:** ChromaDB, PyMuPDF, rank-bm25
- **Data & Visualization:** Matplotlib, Seaborn, Plotly, OpenPyXL, PyArrow
- **Development:** JupyterLab, IPython, debugging and notebook tooling
- **AI APIs:** OpenAI, Google GenAI
- **Web / Apps:** Streamlit, Uvicorn and related packages

## Requirements

- Miniconda or Anaconda
- Linux is recommended for the environment as exported
- Internet connection for package installation

## Installation

Clone the repository:

```bash
git clone https://github.com/JEFFIN-alt/ai-lab.git
cd ai-lab
```

Create the environment:

```bash
conda env create -f environment.yml
```

Activate it:

```bash
conda activate ai-lab
```

Verify the installation:

```bash
python --version
```

Expected Python version:

```
Python 3.12.x
```

## Updating the environment

If the repository's `environment.yml` changes:

```bash
conda env update -f environment.yml --prune
```

## Notes

This environment was exported from a working `ai-lab` Conda environment using:

```bash
conda env export --no-builds > environment.yml
```

The environment contains a large pip-managed dependency set, so installation may take some time and package resolution can vary slightly across operating systems or architectures.

The exported environment includes CPU builds of TensorFlow and PyTorch. GPU-specific CUDA packages are not assumed.

For a clean reproduction, use the same Python major/minor version and preferably Linux.

## Purpose

This repository is intended to make the AI/ML development environment portable so another machine can recreate the same general toolchain without uploading the actual Conda environment directory.

## License

MIT
