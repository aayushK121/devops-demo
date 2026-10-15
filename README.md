# Jenkins GitHub Integration Demo

A simple local project for DevOps Assignment 6.

## Files
- `index.html` — a small web page
- `app.py` — Python script used as a Jenkins build/test step
- `requirements.txt` — no third-party dependencies required

## Run locally
```bash
python3 app.py
```

Expected output:
```text
Hello from Jenkins CI/CD!
Project build check passed.
```

## Jenkins
Configure a Freestyle project to check out this repository from GitHub.
Under **Build Steps → Execute shell**, use:
```bash
echo "Repository cloned successfully"
ls -l
python3 app.py
```
