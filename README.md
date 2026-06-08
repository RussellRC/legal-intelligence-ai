# Udacity Google Agentic AI Engineer Nanodegree - Prompting for Effective LLM Reasoning Project

This repository contains the implementation for the Project of **Course 1: Prompting for Effective LLM Reasoning**,
of the **Udacity Google Agentic AI Engineer** Nanodegree program.

## Getting Started

### Dependencies

* **Python 3.14+**
* **Env Keys**:
    * PROJECT_ID: Google Cloud Project ID
    * GOOGLE_APPLICATION_CREDENTIALS: Path to IAM Service Account Credentials  

To install Poetry, follow the instructions: https://python-poetry.org/docs/

### Installation

**1\. Clone the repository**

**2\. Install dependencies**\
Use venv to create a virtual environment and install the required packages.\
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
`project` directory: Contains [Project Overview](project/PROJECT_OVERVIEW.md), [README.md](project/README.md), and `requirements.txt` files

`project/starter` directory: Contains the **untouched** starter template.

`project/solution/main.py`: Application entry point.

`project/solution/test_setup.py`: Provided test file that ensures that the environment is properly configured.

`project/solution/src` directory: Contains the implementation files

`project/solution/tests` directory: Contains provided test files

`project/outputs` directory: 

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
python main.py
```

## Running tests
```shell
cd project/solution
python tests/test_todos.py
```

## License
[LICENSE.md](./LICENSE.md)
