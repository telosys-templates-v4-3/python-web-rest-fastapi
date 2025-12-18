# python-web-rest-fastapi

Telosys templates for Python REST web application based on **FastAPI framework**.

This bundle provides templates to generate a REST controller for each entity.

To launch the server after code generation, run "fastapi dev main.py"

## This bundle in short
- Target language: **Python** (with type hints)  
- Layers:  REST - Domain - Database (ORM)
- Technical stack:  
  - Validation: **Pydantic**     
  - REST: **FastAPI**  
  - ORM: **SQLAlchemy**   
  - Database: **PostgreSQL**  

## Project structure generated 
- db/
  - records/
  - repositories/
- domain/
  - model/
  - services/
- rest/
  - dto/
  - routers/
- main.py


## Requirements : 
- Telosys ver 4.3.0 or +


## Variables : 
This bundle requires the following variables :
- REST_API_ROOT  ( example : ProjectVariable.REST_API_ROOT=/myapi/v2 )  default= /api/v1
- For a PostgreSQL database:
  - DB_SCHEMA
  - DB_USER
  - DB_PASSWORD
  - DB_HOST
  - DB_PORT
  - DB_NAME



## Dependencies : 
pip install "fastapi[standard]"
pip install sqlalchemy

For PostgreSQL a driver is needed :
- For sync SQLAlchemy:   pip install psycopg[binary]
- For async SQLAlchemy:  pip install psycopg[async]


## Launching the application with Uvicorn
> fastapi dev main.py  
> Server URL: http://127.0.0.1:8000  
> API docs:   http://127.0.0.1:8000/docs   