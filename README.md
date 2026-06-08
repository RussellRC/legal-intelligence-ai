# Udacity Google Agentic AI Engineer Nanodegree - Prompting for Effective LLM Reasoning Project

This repository contains the implementation for the Project of **Course 1: Prompting for Effective LLM Reasoning**,
of the **Udacity Google Agentic AI Engineer** Nanodegree program.

## Getting Started

### Dependencies

* **Python 3.14+**
* **venv**: For isolated virutal environment and dependency management
* **Env Keys**:
    * PROJECT_ID: Google Cloud Project ID
    * GOOGLE_APPLICATION_CREDENTIALS: Path to IAM Service Account Credentials

### Installation

**1\. Clone the repository**

**2\. Install dependencies**\
Use `venv` to create a virtual environment and install the required packages.\
From the root project directory, run the following commands:
```shell
python -m venv .venv
.venv/bin/pip install -r project/requirements.txt
```

**3\. Add a `.env` file** inside the `/project/solution` directory.\
File must have the following variables:
```dotenv
# Google Cloud Configuration
PROJECT_ID=your-project-id
MODEL=gemini-2.5-flash

# Service Account Authentication
GOOGLE_APPLICATION_CREDENTIALS=path/to/service-account-key.json

# Application Settings
DEBUG=false
LOG_LEVEL=INFO
PORT=8000
```

## Project Structure

The project is organized into the following key directories and files:

*   **`project/`**: The root directory for the project, containing:
    *   **`PROJECT_OVERVIEW.md`**: Project Overview from the Udacity project page.
    *   **`README.md`**: Provided `README.md` file from the Udacity project page.
    *   **`requirements.txt`**: Lists all Python dependencies required for the project.

*   **`project/starter/`**: Contains the original, **untouched** starter template code.

*   **`project/solution/`**: Houses the developed solution, including:
    *   **`main.py`**: The primary application entry point (provided).
    *   **`test_setup.py`**: A utility script to verify the environment configuration (provided).
    *   **`src/`**: Contains the developed core implementation logic and source code.
    *   **`tests/`**: Includes all test files for the solution (provided).

*   **`project/outputs/`**: Stores evidence of successful application executions and test runs:
    *   **`test_todos_output.*`**: Output from successful execution of `test_todos.py`.
    *   **`main.png`**: Screenshot or evidence of the main application running successfully.
    *   **`scenario_N - *`**: Request and response files generated when running the application with scenarios from `test_scenarios.json`.

## Prerequisites
Activate the environment with `venv`
```shell
source .venv/bin/activate
```

Before starting, ensure the environment is properly configured:
```shell
cd project/solution
python test_setup.py
```
This should show:
* ✅ Environment file exists
* ✅ Project ID is set
* ✅ Service account key exists
* ✅ Vertex AI API is enabled

## Running the application
```shell
cd project/solution
python main.py
```

## Running tests
```shell
cd project/solution
python tests/test_todos.py
```

## License
[LICENSE.md](./LICENSE.md)