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
```
