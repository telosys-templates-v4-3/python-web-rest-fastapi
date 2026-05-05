# python-web-rest-fastapi

Telosys bundle of templates for Python REST web application based on **FastAPI framework** and **SQLAlchemy** .

This bundle provides templates to generate a REST controller for each entity.

To launch the server after code generation, run "fastapi dev main.py"

## This bundle in short
- Target language: **Python** 3.10 or higher (with type hints)  
- Layers:  REST - Domain - Database (ORM)
- Technical stack:  
  - Validation: **Pydantic**     
  - REST: **FastAPI**  
  - ORM: **SQLAlchemy**   
  - Database: **PostgreSQL** or **SQLite** (for testing) 

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
- REST_API_ROOT  (default is "/api/v1")
- TARGET_DATABASE = PostgreSQL or SQLite (default is SQLite)
- For a PostgreSQL database:
  - DB_USER
  - DB_PASSWORD
  - DB_HOST
  - DB_PORT
  - DB_NAME
  - DB_SCHEMA

## Generated application 
To install the required Python dependencies and run the generated application
see the generated README.md file in the project folder after code generation.
