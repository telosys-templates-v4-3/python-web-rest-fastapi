# python-web-rest-fastapi

Telosys templates for Python REST web application based on **FastAPI framework**.

This bundle provides templates to generate a REST controller for each entity.

To launch the server after code generation, run "fastapi dev main.py"

## This bundle in short
- Target language: **Python** (with type hints)  
- Layers:  
  - Domain  
  - REST  
  - DB/ORM  
- Technical stack:  
  - Validation: **Pydantic**     
  - REST: **FastAPI**  
  - ORM: **SQLAlchemy**   
  - Database: **PostgreSQ**  

## Requirements : 
- Telosys ver 4.3.0 or +

## Variables : 
This bundle requires the following variables :
- REST_URL_ROOT ( example : `ProjectVariable.REST_URL_ROOT=http://localhost:3000 ` )
- REST_API_ROOT ( example : `ProjectVariable.REST_API_ROOT=/api/v1  ` )


## Dependencies : 
pip install "fastapi[standard]"
pip install sqlalchemy

For PostgreSQL a driver is needed :
- For sync SQLAlchemy:   pip install psycopg[binary]
- For async SQLAlchemy:  pip install psycopg[async]


## Launching the application with Uvicorn
> fastapi dev main.py
Server URL: http://127.0.0.1:8000
API docs:   http://127.0.0.1:8000/docs

