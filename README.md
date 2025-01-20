# DVC Repository Setup and Usage

## **Introduction**
Data Version Control (DVC) is a powerful tool for managing and versioning data, models, and machine learning pipelines.

---

## **Setup Instructions**

### 1. Create a Virtual Environment
Create an isolated Python environment to work with DVC:
```bash
conda create -p venv python==3.9 -y
conda activate venv/
```

### 2. Initialize Git and DVC
Set up Git and initialize DVC for your project:
```bash
git init
dvc init
```

### 3. Install DVC
Install the DVC package using pip:
```bash
pip install dvc
```

---

## **Basic Commands**

### 1. Track Data Files with DVC
Add a file or dataset to DVC for version control:
```bash
dvc add data/data.txt
```

### 2. Track Changes with Git
Track the DVC metadata and other relevant files with Git:
```bash
git add data/data.txt.dvc
git add data/.gitignore
```
Commit the changes:
```bash
git commit -m "Initialize DVC tracking"
```

### 3. View Repository Status
Check the current status of your repository:
```bash
git status
git log
```

---

## **Switching Between Versions**

### 1. Checkout a Specific Version
To revert to a specific version of your project:
```bash
git checkout <commit-hash>
dvc checkout
```

### 2. Return to the Latest Version
Switch back to the main branch:
```bash
git checkout master
dvc checkout
```

---

## **Tips**
- Always ensure your virtual environment is activated before running DVC commands.
- Use descriptive commit messages to track changes effectively.
- Regularly push your Git and DVC changes to a remote repository for backup and collaboration.

---

## **Resources**
- [DVC Documentation](https://dvc.org/doc)
- [Git Documentation](https://git-scm.com/doc)

---

