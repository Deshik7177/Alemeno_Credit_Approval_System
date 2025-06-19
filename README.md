# Credit Approval System

Welcome, your no-nonsense credit approval system that’s all about deciding if someone’s ready to get that loan or nah — based on their past loan moves. Think of it as the gatekeeper that checks the receipts before saying yes or no.

## What This Does

- Add new customers — build that squad in the database.
- Check loan eligibility — crunches the credit score to see if you’re good to go.
- Process new loans — if you’re eligible, boom, the loan’s in motion.
- View loan & customer details — get the full tea on loans and who's got 'em.
- See all active loans by customer — track the hustle customer-wise

## Tech Stack

- Django
- PostgreSQL
- Docker
- Docker Compose

## API Endpoints

All APIs run under `/`:
1. `/register/`: Add a new customer.
2. `/check-eligibility/`: Check loan eligibility based on credit score.
3. `/create-loan/`: Process a new loan based on eligibility.
4. `/view-loan/loan_id/`: View loan details and customer details by loan ID.
5. `/view-loans/customer_id/`: View all current loan details by customer ID.

Note: Make sure to add a slash ('/') at the end of the API.

## Pre-requisites

- python
- docker
- Docker Desktop
- docker-compose

## How To Run This Thing — Step by Step

>Clone this Repo
```bash
git clone https://github.com/Deshik7177/Alemeno_Credit_Approval_System.git

>Make sure your Docker engine’s running—open Docker Desktop or start it using your OS’s way.

>Run Docker Compose
```bash
docker-compose up
```
>Hit the APIs:
```bash
http://localhost:8000/
```

## Testing the project
Use this Postman collection with existing APIs to test the project


## Adding production secrets
Create a ```.env``` file in the root directory of this project & add a [SECRET_KEY](https://docs.djangoproject.com/en/5.0/ref/settings/#secret-key) for django to use.
>Run the following command in your Django project's Python shell to generate a secret key
```bash
from django.core.management.utils import get_random_secret_key
get_random_secret_key()
```
>Copy the new SECRET_KEY that is generated & paste it to your .env file.
```
SECRET_KEY=your_secret_key_here
```
Follow example.env

## Author
Paila Dhana Deshik (www.linkedin.com/in/paila-dhana-deshik-b4986a293, pdhanadeshik7177@gmail.com)
