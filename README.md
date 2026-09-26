Sure 👍 Here is the **clean, portfolio-ready README only**. You can copy-paste it directly into GitHub.

# 🚀 GitHub Actions CI/CD Pipeline

A containerized Flask application with an automated CI/CD pipeline using **GitHub Actions**.

## 🏗️ Project Flow

```text
👨‍💻 Code Push
     ↓
🐙 GitHub
     ↓
⚙️ GitHub Actions
     ↓
📦 Install Dependencies
     ↓
🧪 Run Pytest
     ↓
🐳 Build Docker Image
     ↓
✅ Pipeline Success
```

## 🛠️ Technologies

* 🐍 Python 3.12
* 🌐 Flask
* 🧪 Pytest
* 🐳 Docker
* ⚙️ GitHub Actions
* 🔧 Git & GitHub

## ✨ What This Project Does

The GitHub Actions workflow automatically runs when code is pushed to `main` or when a pull request targets `main`.

The pipeline:

1. 📥 Checks out the code
2. 🐍 Sets up Python 3.12
3. 📦 Installs dependencies
4. 🧪 Runs automated tests
5. 🐳 Builds the Docker image
6. ✅ Reports the pipeline result

## 🧪 Testing

Run the tests locally:

```bash
PYTHONPATH=. pytest
```

### ✅ Test Result

```text
2 passed
```

## 🐳 Docker

### Build the Image

```bash
docker build -t github-actions-cicd:1.0 .
```

### Run the Container

```bash
docker run -d \
  --name github-actions-cicd \
  -p 8000:8000 \
  github-actions-cicd:1.0
```

### Test the Application

```bash
curl http://localhost:8000/health
```

Expected response:

```json
{"status":"healthy"}
```

## 📂 Project Structure

```text
github-actions-cicd/
├── .github/
│   └── workflows/
│       └── ci.yml
├── app/
│   ├── __init__.py
│   └── app.py
├── tests/
│   └── test_app.py
├── Dockerfile
├── requirements.txt
├── .gitignore
└── README.md
```

## ⚙️ GitHub Actions Workflow

The workflow is defined in:

```text
.github/workflows/ci.yml
```

It runs automatically on:

* 📤 Push to `main`
* 🔀 Pull requests targeting `main`

### Pipeline Stages

```text
📥 Checkout Code
       ↓
🐍 Setup Python 3.12
       ↓
📦 Install Dependencies
       ↓
🧪 Run Pytest
       ↓
🐳 Build Docker Image
       ↓
✅ Pipeline Complete
```

## 🎯 Skills Demonstrated

**CI/CD • GitHub Actions • Docker • Python • Flask • Pytest • Git • GitHub • Automation**

## 🧠 What I Learned

* 🔄 CI/CD fundamentals
* ⚙️ GitHub Actions workflows
* 🧪 Automated testing with Pytest
* 🐳 Docker containerization
* 🔧 Git and GitHub workflows
* 📦 Dependency management
* 🚀 Automating application validation and Docker builds

## 👨‍💻 Author

**Shubham Gorule**

BCA Student | Aspiring Cloud Engineer | AWS | Linux | Networking | DevOps

---

⭐ **Built as part of my Cloud & DevOps project portfolio.**
