# GWU CS6364 - Machine Learning

**Course Numbers:** CSCI-4364-87 / CSCI-6364-80

This repository contains executable Jupyter notebook lectures for CS6364 Machine Learning at The George Washington University (Fall 2025 edition).

## 📋 Course Information

For detailed course information including schedule, grading, and policies, please see [SYLLABUS.md](SYLLABUS.md).

## 📁 Repository Structure

```
.
├── README.md              # Setup instructions (this file)
├── SYLLABUS.md           # Complete course syllabus  
├── requirements.txt      # Python packages for pip
├── requirements.yml      # Python packages for conda
└── slides/
    ├── lecture1-introduction.ipynb
    ├── lecture2-machine-learning-setup.ipynb
    ├── ...               # More lectures will be added
    └── img/              # Images and figures used in lectures
```

## 🚀 Environment Setup

You have two options to set up your environment: **Anaconda** (recommended) or **virtualenv**.

### Option 1: Anaconda (Recommended)

1. **Install Anaconda** if you haven't already:
   - Download from [https://www.anaconda.com/download](https://www.anaconda.com/download)

2. **Create and activate the environment**:
   ```bash
   conda create --name gw-cs6364 --file requirements.yml
   conda activate gw-cs6364
   ```

3. **Install Jupyter kernel**:
   ```bash
   python -m ipykernel install --user --name=gw-cs6364
   ```

4. **Start Jupyter Lab/Notebook**:
   ```bash
   jupyter lab
   # or
   jupyter notebook
   ```

### Option 2: Virtual Environment

1. **Create and activate virtual environment**:
   ```bash
   python -m venv gw-cs6364
   source gw-cs6364/bin/activate  # On Windows: gw-cs6364\Scripts\activate
   ```

2. **Install packages**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Install Jupyter kernel**:
   ```bash
   python -m ipykernel install --user --name=gw-cs6364
   ```

4. **Start Jupyter Lab/Notebook**:
   ```bash
   jupyter lab
   # or
   jupyter notebook
   ```

## 📖 Running the Lectures

1. **Open Jupyter** using one of the methods above
2. **Navigate** to the `slides/` directory
3. **Select the kernel**: When opening a notebook, make sure to select the `gw-cs6364` kernel
4. **Run the cells**: Execute cells sequentially using `Shift+Enter`

## 🛠️ Troubleshooting

### Common Issues

**"Kernel not found" error:**
- Make sure you installed the Jupyter kernel: `python -m ipykernel install --user --name=gw-cs6364`
- Restart Jupyter and select the correct kernel

**Missing packages:**
- Activate your environment first: `conda activate gw-cs6364` or `source gw-cs6364/bin/activate`
- Reinstall requirements: `pip install -r requirements.txt`

**Images not displaying:**
- Ensure you're running Jupyter from the repository root directory
- Check that the `slides/img/` directory contains all necessary files

### Getting Help

1. Check the [course syllabus](SYLLABUS.md) for contact information
2. Ask questions during class or office hours
3. Post on the course discussion forum

## 🎯 Quick Start Checklist

- [ ] Clone/download the repository
- [ ] Set up your environment (conda or virtualenv)
- [ ] Install the Jupyter kernel
- [ ] Start Jupyter Lab/Notebook
- [ ] Open a lecture notebook
- [ ] Select the `gw-cs6364` kernel
- [ ] Run the first cell to test everything works

## 📚 Course Overview

This course covers the fundamentals of machine learning including:
- **Supervised Learning**: Regression, classification, SVMs
- **Unsupervised Learning**: Clustering, dimensionality reduction
- **Deep Learning**: Neural networks and modern architectures
- **Practical Applications**: Real-world ML implementation and evaluation

## 📚 Credits

Course materials are adapted from multiple sources including Cornell CS5785 (https://github.com/kuleshov/cornell-cs5785-2023-applied-ml), courtesy of Volodymyr Kuleshov.