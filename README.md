
# Excel Local Analyzer

A local-based data analysis application designed to help users explore, analyze, clean, and visualize spreadsheet data more efficiently. It combines statistical analysis, interactive visualizations, AI-powered insights, and automated report generation in one application.

## Overview

Excel Local Analyzer transforms raw spreadsheet data into meaningful information through an intuitive interface. Users can upload datasets, explore statistical summaries, identify data quality issues, generate visualizations, and interact with AI to gain deeper insights into their data.

The application is designed to run locally, providing a practical and accessible data analysis workflow without requiring users to rely entirely on cloud-based services.

## Features

- **Data Upload & Exploration** — Upload Excel and CSV files, preview datasets, and explore columns and data types.
- **Automated Statistical Analysis** — Generate descriptive statistics, distributions, and summaries automatically.
- **Data Cleaning** — Identify missing values, duplicate records, and potential data quality issues.
- **Interactive Visualizations** — Explore data through charts and graphical representations.
- **AI Insights** — Get AI-assisted interpretations, summaries, and insights from analyzed datasets.
- **AI Chat** — Interact with your data using natural language.
- **Dashboard Builder** — Create customizable dashboards based on selected datasets and visualizations.
- **Custom KPI Analysis** — Define key performance indicators based on your data.
- **Correlation Analysis** — Explore relationships between numerical variables.
- **Outlier Detection** — Identify potential anomalies using statistical methods.
- **PDF Report Generation** — Export structured analysis reports containing statistics, visualizations, and insights.
- **Analysis History** — Access previously saved analysis sessions.
- **Local Processing** — Designed to process data locally for greater privacy and control.

## Tech Stack

### Frontend
- Next.js
- React
- TypeScript
- Tailwind CSS
- Recharts

### Backend
- Python
- FastAPI
- Pandas
- NumPy
- Matplotlib
- Seaborn
- ReportLab

### AI
- Ollama
- Local Large Language Models (LLMs)

### Database
- SQLite

## Application Architecture

The application uses a frontend-backend architecture.

- **Frontend:** Handles the user interface, data exploration, dashboards, charts, and interactions.
- **Backend:** Processes uploaded datasets, performs statistical analysis, manages data operations, and generates PDF reports.
- **AI Integration:** Uses locally running AI models through Ollama to provide contextual insights and conversational analysis.
- **Database:** SQLite is used to store application-related data and analysis history.

## Getting Started

### Prerequisites

Make sure you have installed:

- Node.js
- npm
- Python 3.10+
- Git
- Ollama (optional, for AI-powered features)

### Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/excel-local-analyzer.git
cd excel-local-analyzer
```

### Backend Setup

Navigate to the backend directory:

```bash
cd backend
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate the virtual environment.

**Windows:**

```bash
venv\Scripts\activate
```

**Linux / macOS:**

```bash
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the backend server:

```bash
uvicorn main:app --reload
```

> Adjust the entry point if your FastAPI application uses a different module name.

### Frontend Setup

Open another terminal and navigate to the frontend directory:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

Open the application in your browser:

```text
http://localhost:3000
```

### AI Setup (Optional)

Install and run Ollama, then download a model compatible with your system.

Example:

```bash
ollama pull llama3.1
```

Start Ollama and configure the application to use the installed model.

AI-powered features may depend on the availability of the Ollama service and the selected model.

## How to Use

1. Start the backend and frontend servers.
2. Open Excel Local Analyzer in your browser.
3. Upload an Excel or CSV dataset.
4. Explore the dataset using the statistical analysis and visualization tools.
5. Clean and inspect data quality issues if necessary.
6. Generate insights using AI or interact with the AI chat.
7. Build a custom dashboard using selected metrics and charts.
8. Export your analysis into a PDF report.

## Project Structure

```text
excel-local-analyzer/
│
├── frontend/
│   ├── app/
│   ├── components/
│   ├── public/
│   └── ...
│
├── backend/
│   ├── main.py
│   ├── report_generator.py
│   ├── ...
│   └── requirements.txt
│
├── README.md
└── ...
```

*The project structure may evolve as new features are added.*

## Privacy

Excel Local Analyzer is designed with a local-first approach. Data processing and analysis are intended to run on the user's local environment.

When local AI models are used through Ollama, AI inference can also be performed locally without sending prompts to an external AI provider, depending on the application's configuration.

Users should always verify their configuration before processing sensitive datasets.

## Future Improvements

- More advanced statistical analysis
- Additional visualization types
- Improved AI-generated insights
- More customizable report templates
- Expanded data cleaning tools
- Performance optimization for larger datasets
- Additional file format support

## Author

Developed as a personal project to explore data analysis, full-stack development, AI integration, and practical software engineering.

---

If you find this project interesting, feel free to explore the repository.
