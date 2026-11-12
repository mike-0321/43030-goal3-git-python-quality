# Goal 3: Git Workflow and Python Software Quality

Practise Git-based development, Python quality checks and regression testing
with a small handwritten-digits API.

Use Python 3.12 and run these commands from a Git checkout:

```sh
python3.12 -m venv .venv
.venv/bin/python -m pip install -r requirements.lock
.venv/bin/python -m learning_service.train
.venv/bin/python scripts/quality.py
.venv/bin/python -m pytest -v
.venv/bin/python serve_demo.py
```

Training creates the model and example request before testing or serving.
The server prints a temporary key and interactive API URL. On Windows, use
`.venv\Scripts\python.exe`.

Dataset: Alpaydin, E., & Kaynak, C. (1998). *Optical recognition of handwritten
digits*. UCI Machine Learning Repository. https://doi.org/10.24432/C50P49
