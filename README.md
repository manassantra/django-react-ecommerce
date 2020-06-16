# Django React Ecommerce

[![alt text](https://github.com/justdjango/django-react-ecommerce/blob/master/thumbnail.png "Logo")](https://youtu.be/RG_Y7lIDXPM)

This repository contains a Django and React ecommerce project. Among other functionality, users can create their account, add items to their cart and purchase those items using Stripe.

[Watch the tutorials on how to build this project](https://youtu.be/RG_Y7lIDXPM)

## Backend development workflow

```json
virtualenv env
source env/bin/activate
pip install -r requirements.txt
python manage.py runserver
```
Next, set up a virtual environment and activate it:

python3 -m venv env && source env/bin/activate

Install required packages:

pip3 install -r requirements.txt

Next, perform migration:

python3 manage.py migrate --settings=src.settings.local

At this point, one may want to create a superuser account and create some products. One can also use sample data provided in products/fixtures.json by running:

python3 manage.py loaddata products/fixture.json --settings=src.settings.local

The backend is now ready. Run a local server with

python3 manage.py runserver --settings=src.settings.local

The backend should be available at localhost:8000.

## Frontend development workflow

```json
npm i
npm start
```

## For deploying

```json
npm run build
```
