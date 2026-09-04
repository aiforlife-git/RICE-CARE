## Installation

### 1. Clone or download the repository

```bash
After that.........
cd RICE_CARE
```

### 2. Create a virtual environment

**Windows (PowerShell):**

```powershell
python -m venv .venv
```

### 3. Install dependencies

You can install the dependencies directly using the Python interpreter inside the virtual environment.

**Windows (PowerShell):**

```powershell
.\.venv\Scripts\python.exe -m pip install -r requirements.txt
```

### 4. Configure environment variables

Create a `.env` file in the project root directory using `.env.example` as a template.

**Windows (PowerShell):**

```powershell
Copy-Item .env.example .env
```

Then open `.env` and add your API credentials:

```text
OPENAI_API_KEY=your-openai-api-key
HF_API_Read=your-huggingface-token
QDRANT_API_KEY=your-qdrand-api-key #if you are using cloud
QDRANT_URL=qdrant-url #if you are using cloud
```

**Do not share or commit your `.env` file or API keys.**

### 5. Run the application

**Windows (PowerShell):**

```powershell
.\.venv\Scripts\python.exe -m streamlit run app.py
```

After starting the application, Streamlit will display the local URL in the terminal. Typically:

```text
http://localhost:8501
```
