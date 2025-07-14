
# 🚆 RailSathiBE — FastAPI + PostgreSQL Microservice (Dockerized)

This is a backend microservice built with FastAPI and PostgreSQL, designed to manage railway complaints and related functionality. The entire project is containerized using Docker and Docker Compose, making it easy to set up and run locally.

---

## 🧰 Features

- FastAPI-based RESTful API
- Dockerized setup using Docker and Docker Compose
- PostgreSQL database container
- API documentation via Swagger UI
- Environment configuration with `.env` file





## 🗂 Project Structure

RailSathiBE/
├── __pycache__/                  # Compiled Python files
├── env/                          # Virtual environment (not committed)
├── templates/                    # Template files (if any)
├── utils/                        # Utility functions
│   ├── __pycache__/
│   └── email_utils.py            # Email handling logic
├── .env                          # Environment variables
├── .gitignore                    # Git ignore rules
├── database.py                   # Database connection setup
├── docker-compose.yml            # Docker Compose configuration
├── Dockerfile                    # Docker image build file
├── logger_config.py              # Logging configuration
├── mail_config.py                # Email service config
├── main.py                       # FastAPI application entrypoint
├── README.md                     # Project documentation
├── requirements.txt              # Python dependencies
├── services.py                   # Core business logic / services
└── test_email.py                 # Email sending test script



## 🚀 Getting Started

### 1. Clone the Repository


git clone https://github.com/ranjeet3345/RailSathiBE.git
cd RailSathiBE


### 2. Create `.env` File

ITS CONTENT: 

POSTGRES_DB=your_db_name
POSTGRES_USER=postgres
POSTGRES_PASSWORD=your_password
POSTGRES_HOST=db
POSTGRES_PORT=5432
MAIL_USERNAME=test@example.com
MAIL_PASSWORD=somepassword
MAIL_FROM=test@example.com


### 3. Run the Project

Make sure Docker is running, then:

```bash
docker-compose up --build


The API will be accessible at:
[http://localhost:8000/rs\_microservice/docs](http://localhost:8000/rs_microservice/docs)

---

## 🔌 API Endpoints

| Path                            | Method | Description                   |
| ------------------------------- | ------ | ----------------------------- |
| `/rs_microservice/docs`         | GET    | Swagger API documentation     |

## 🛠 Tech Stack

* Python 3.12
* FastAPI
* PostgreSQL
* Docker & Docker Compose
* dotenv for config management




##  Notes & Assumptions

* The project uses a custom path prefix `/rs_microservice` for APIs.



