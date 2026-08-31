## Installation

### 1. Clone the repository

```bash
Then.........
cd RICE-CARE
```

### 2. Create a virtual environment

**Windows (PowerShell):**

```powershell
python -m venv .venv
```

**Linux/macOS:**

```bash
python3 -m venv .venv
```

### 3. Install dependencies

You can install the dependencies directly using the Python interpreter inside the virtual environment.

**Windows (PowerShell):**

```powershell
.\.venv\Scripts\python.exe -m pip install -r requirements.txt
```

**Linux/macOS:**

```bash
./.venv/bin/python -m pip install -r requirements.txt
```

### 4. Configure environment variables

Create a `.env` file in the project root directory using `.env.example` as a template.

**Windows (PowerShell):**

```powershell
Copy-Item .env.example .env
```

**Linux/macOS:**

```bash
cp .env.example .env
```

Then open `.env` and add your API credentials:

```text
OPENAI_API_KEY=your_openai_api_key
HF_API_Read=your_huggingface_token
```

**Do not share or commit your `.env` file or API keys.**

### 5. Run the application

**Windows (PowerShell):**

```powershell
.\.venv\Scripts\python.exe -m streamlit run app.py
```

**Linux/macOS:**

```bash
./.venv/bin/python -m streamlit run app.py
```

After starting the application, Streamlit will display the local URL in the terminal. Typically:

```text
http://localhost:8501
```
