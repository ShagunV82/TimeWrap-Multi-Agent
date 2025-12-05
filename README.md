## TimeWrap Multi-Agent System

A multi-agent LLM workflow for automated time-series analysis, insight generation, and executive reporting.

## Project Overview

- Transforms complex time-series data into actionable intelligence using a four-agent workflow
  (Data Retrieval → Data Analysis → Insight → Report)
- Uses Gemini via Google ADK for LLM-powered reasoning and narrative summaries.
- Evaluates trends, anomalies, and news sentiment to generate a final recommendation and confidence score.
- Designed to be modular so each agent can be improved or replaced independently.

## Key Features

- **Automated Time-Series Analysis:** Collects stock data and calculates moving averages, volatility, and key metrics.
- **Anomaly Detection:** Statistically identifies unusual price movements using Z-scores.
- **Sentiment Integration:** Incorporates recent news headlines to contextualize numerical trends.
- **Confidence Scoring:** Provides a dynamic confidence score for the final recommendation, reflecting the quality and completeness of the data and analysis.
- **Executive Reporting:** Compiles all findings into a professional, stakeholder-ready HTML report.

## Tech Stack

- **Language:** Python 3  
- **LLM & Orchestration:** Gemini, Google ADK (`google-adk`, `google-genai`)  
- **Data & Evaluation:** Pandas, time-series analysis utilities  
- **Environment:** Jupyter Notebook (Kaggle / local)

## Files

- `timewrap-agent.ipynb` – Main notebook containing the multi-agent workflow and evaluation logic.
- `TimeWrap-Agent-_writeup.pdf` – Short write-up describing the system, design choices, and results.
- `requirements.txt` – Core Python dependencies to run the notebook.

## Setup

1. Install dependencies:  
   `pip install -r requirements.txt`
2. Set `GOOGLE_API_KEY` as an environment variable.
3. Launch Jupyter and open `timewrap-agent.ipynb`.

## How to Run

1. Run the notebook cells from top to bottom.  
2. The notebook will:
   - Validate that `GOOGLE_API_KEY` is set.
   - Initialize ADK agents and runner.
   - Execute the multi-agent workflow on example time-series + news data.
   - Produce an executive-style report with trends, anomalies, news highlights, and a recommendation.
   
   
## Output


<img width="761" height="582" alt="Screenshot 2025-12-05 at 6 21 08 PM" src="https://github.com/user-attachments/assets/a09acb3a-406b-4fda-b197-23c1b060b44c" />


<img width="728" height="609" alt="Screenshot 2025-12-05 at 6 21 45 PM" src="https://github.com/user-attachments/assets/8b230641-a1da-4d91-8ab6-aa1b63185c63" />

