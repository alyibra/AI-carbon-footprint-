# AI Carbon Footprint

A polished project that estimates the carbon impact of GPT prompt usage and presents it in a responsive web interface.

This repository demonstrates a full-stack application with:
- Flask-powered backend calculation logic
- JavaScript-driven frontend for form interaction and chart visualization
- Realistic token-based CO₂ estimation using `tiktoken`
- Support for multiple models and regions

## Key features

- Single-interaction CO₂ estimation
- Equivalency display in car travel minutes
- Aggregated projections for 1 month, 6 months, 1 year, and 5 years
- Interactive chart comparing model emissions
- Validation and structured error handling for API inputs

## Tech stack

- Python 3.12
- Flask
- JavaScript + Chart.js
- `tiktoken`
- HTML / CSS

## Project structure

- `ai carbon/app.py` — Flask application and API endpoint
- `ai carbon/logic.py` — emission calculation and token processing
- `ai carbon/constant.py` — model and region constants
- `ai carbon/templates/index.html` — user interface template
- `ai carbon/static/js/app.js` — frontend interaction and chart rendering
- `ai carbon/static/css/styles.css` — application styling
- `ai carbon/requirements.txt` — Python dependencies
- `ai carbon/Dockerfile` — container instructions for deployment
- `ai carbon/tests/test_logic.py` — unit tests for application logic

## Run locally

1. Open a terminal and change into the project directory:
   ```bash
   cd 'ai carbon'
   ```
2. Install dependencies:
   ```bash
   python3 -m pip install --user -r requirements.txt
   ```
3. Start the app:
   ```bash
   python3 app.py
   ```
4. Open the browser:
   ```txt
   http://127.0.0.1:5000
   ```

## Quick start

From the repository root, run:
```bash
./run.sh
```

## Run tests

From the `ai carbon` directory:
```bash
python3 -m unittest discover -s tests
```

## Docker

To build and run the container, use:
```bash
cd 'ai carbon'
docker build -t ai-carbon-footprint .
docker run -p 5000:5000 ai-carbon-footprint
```

## Professional polish

- Added a project-level `.gitignore` to keep repositories clean.
- Added a launch script for easy local startup.
- Added unit tests for core logic and validation.
- Added Docker support for repeatable deployment.

## Opportunities for extension

- Add persistent data storage and user history
- Expand the model library with real API usage metrics
- Add production configuration for WSGI servers or cloud deployment
