# **DVC - Data Version Control Repository**

Welcome to Data Version Control (DVC)! This guide will help you set up and manage DVC.

---

## **Getting Started**

### 1. **Create and Activate a Virtual Environment**
- To isolate your project environment:

```bash
conda create -p venv python==3.9 -y
conda activate venv/
```

### 2. **Initialize Git and DVC**
- Set up version control for your project:

```bash
git init
dvc init
```
- Install the DVC package if it's not installed:
```bash
pip install dvc
```

### 3. **Track Data with DVC**
- Add your data files to DVC for version tracking:

```bash
dvc add data/data.txt
```
- This will generate a .dvc file to track your data.


### 4. **Commit Changes to Git**
- Track the DVC configuration and related files with Git:

```bash
git add data/data.txt.dvc
git add data/.gitignore
git commit -m "Initialize DVC and add data"
```

### 5. **Check Repository Status**
- Inspect the status of your Git repository and view commit logs:

```bash
git status
git log
```

### 6. **Checkout Specific Versions**
- To view a specific version of your data, use the commit hash:

```bash
git checkout <commit-hash>
dvc checkout
```

### 7. **Return to the Latest Version**
- Switch back to the master branch to access the most updated version:

```bash
git checkout master
dvc checkout
```
