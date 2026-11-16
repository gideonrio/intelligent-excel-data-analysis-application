# 📊 Intelligent Excel Data Analyst (IEDA)

An intelligent desktop application developed using **Python, PyQt5, Machine Learning, and Large Language Models (LLMs)** that transforms raw Excel data into meaningful insights.

The application provides interactive dashboards, automated Excel operations, ML-powered predictions, PDF report generation, and conversational data analysis through Ollama integration.

---

## ✨ Features

### 📁 1. Excel File Management
- Load and manage multiple Excel files (`.xlsx`, `.xls`) simultaneously.
- Preview the first 10 rows of Excel data.
- View complete sheets in a pop-up dialog.
- Track loaded DataFrames with shape, column information, and metadata.

### 📊 2. Interactive Dashboard
- Generate different chart types:
  - Line Chart
  - Bar Chart
  - Pie Chart
  - Scatter Plot
  - Histogram
- Filter data by column values before visualization.
- Select multiple columns for comparison charts.
- Customize chart titles and histogram bin counts.
- Automatically save charts as PDF reports.

### 🔧 3. Excel Operations
- Merge DataFrames using Inner, Left, Right, and Outer Joins.
- Filter data using conditions:
  - `==`
  - `!=`
  - `>`
  - `<`
  - `>=`
  - `<=`
  - `contains`
- Filter data by row index.
- Search and highlight specific values across columns.
- Display operation results in pop-up dialogs.
- Save processed results as downloadable files.

### 📈 4. Data Analysis
- Generate descriptive statistics:
  - Mean
  - Standard Deviation
  - Minimum and Maximum
  - Quartiles
- Analyze missing values.
- Calculate missing value counts and percentages.
- Generate frequency distributions using Value Counts.
- Export analysis results as formatted PDF reports.

### 🤖 5. Machine Learning Prediction
- **Linear Regression:** Predict numerical values.
- **Decision Tree Classifier:** Perform categorical classification.
- Evaluate models using:
  - R² Score
  - Mean Squared Error (MSE)
  - Mean Absolute Error (MAE)
  - Accuracy
  - Classification Report
- Optional feature scaling using StandardScaler.
- Enter new values and receive live predictions.
- Get plain-language explanations of model results using an LLM.

### 💬 6. LLM Chat – Ollama Integration
- Conversational AI powered by Ollama.
- Uses the `phi3` language model.
- Supports Excel data context injection for data-aware responses.
- Maintains chat history.
- Provides chat history clearing functionality.

### 🤖 7. Automation Bot
- Google Drive integration.
- Authenticate and fetch Excel files directly from Google Drive.
- Automate Excel operations.
- Clear missing values.
- Generate dashboard and analysis reports.
- Schedule daily automation tasks.
- Automatically generate and save PDF reports.

### 📂 8. Files & Reports
- Centralized location for generated files.
- Manage PDF reports and Excel exports.
- Download generated files to your computer.
- Send reports through email using SMTP integration.

---

## 🛠️ Tech Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| GUI Framework | PyQt5 |
| Data Processing | Pandas, NumPy |
| Data Visualization | Matplotlib |
| Machine Learning | Scikit-learn |
| LLM Integration | Ollama (phi3) |
| Report Generation | FPDF |
| Cloud Storage | PyDrive2, Google Drive API |
| Email Integration | SMTP, smtplib |
| Task Scheduling | Schedule |
| UI Styling | Custom QSS Dark Theme |

---

## 📁 Project Structure

```text
intelligent-excel-data-analysis-application/
│
├── IEDA/
│   └── excel_llm_desktop/
│       ├── main_app.py
│       ├── AutomatedBotTab.py
│       ├── analysis_tab.py
│       ├── dashboard_tab.py
│       ├── prediction_tab.py
│       ├── merge_tab.py
│       ├── llm_chat_tab.py
│       ├── llm_worker.py
│       ├── checked.png
│       ├── unchecked.png
│       ├── down_arrow.png
│       └── other project files
│
├── .gitignore
└── README.md
```

---

## 🚀 Getting Started

### 1. Prerequisites

Make sure you have installed:

- Python 3.9 or above
- Git
- Visual Studio Code
- Ollama (for LLM features)

### 2. Clone the Repository

```bash
git clone https://github.com/gideonrio/intelligent-excel-data-analysis-application.git
```

Navigate to the project directory:

```bash
cd intelligent-excel-data-analysis-application
```

Navigate to the application folder:

```bash
cd IEDA/excel_llm_desktop
```

### 3. Install Dependencies

```bash
python -m pip install PyQt5 pandas numpy matplotlib scikit-learn ollama fpdf pydrive2 schedule openpyxl xlrd
```

### 4. Set Up Ollama

Install Ollama:

https://ollama.com/

Download the required model:

```bash
ollama pull phi3
```

Make sure Ollama is running before using the LLM Chat functionality.

### 5. Set Up Google Drive Integration

To use the Automation Bot:

1. Open Google Cloud Console.
2. Create a Google Cloud project.
3. Enable the Google Drive API.
4. Configure OAuth credentials.
5. Download the required `client_secrets.json` file.
6. Place the credentials file in the location expected by the application.

Google Cloud Console:

https://console.cloud.google.com/

PyDrive2 Documentation:

https://docs.iterative.ai/PyDrive2/quickstart/#authentication

### 6. Run the Application

Execute:

```bash
python main_app.py
```

The Intelligent Excel Data Analyst desktop application should now launch.

---

## 🎨 UI Theme

The application features a modern dark-themed interface using custom QSS styling.

### Design Highlights

- Deep navy background (`#1a1a2e`)
- Purple accent buttons (`#3e2f5b`)
- Rounded component borders.
- Custom checkbox icons.
- Custom dropdown arrow icons.
- Dark-mode-compatible Matplotlib charts.

---

## 📋 How to Use

1. **Load Data:** Import one or more Excel spreadsheets.
2. **Dashboard:** Create interactive charts and visualizations.
3. **Analysis:** Explore descriptive statistics and missing values.
4. **Prediction:** Train machine learning models and generate predictions.
5. **Merge:** Combine multiple DataFrames.
6. **LLM Chat:** Ask questions about your Excel data.
7. **Automation:** Configure automated tasks and scheduled reports.
8. **Files & Reports:** Download or email generated reports.

---

## 🔐 Security Notes

- Never upload Google Drive credentials such as `client_secrets.json` to a public repository.
- Do not store personal email passwords directly in source code.
- Use environment variables for sensitive credentials.
- Keep API keys and authentication files private.

---

## 🤝 Contributing

Suggestions, feedback, and improvements are welcome.

1. Fork the repository.
2. Create a new branch.
3. Make your changes.
4. Commit your changes.
5. Submit a Pull Request.

---

## 📝 License

This project is available under the MIT License, subject to the license included in the repository.

---

## 👨‍💻 Developer

**Gideon**

B.Tech – Information Technology

Interested in Software Development, Artificial Intelligence, Machine Learning, and Data Analytics.

- GitHub: https://github.com/gideonrio

---

⭐ If you find this project interesting, consider giving the repository a star!
