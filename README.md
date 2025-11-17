# VENV

## When someone wants to clone my repo

## ✅ 1. Create project

```bash
django-admin startproject myproject
cd myproject
```

```
myproject/
│
├── manage.py
├── myproject/
│   ├── settings.py
│   ├── urls.py
│   └── ...
```

## ✅ 2. Create virtual environment

```bash
python -m venv venv

```

```
myproject/
│
├── venv/            <-- virtual environment
├── manage.py
└── myproject/
```

## ✅ 3. Activate it

### windows

```bash
venv\Scripts\activate

```

### Mac/Linus

```bash
source venv/bin/activate


```

## ✅ 4. Install packages

```bash
pip install django djangorestframework

```

## ✅ 5. Freeze dependencies

```bash
pip freeze > requirements.txt

```

```
myproject/
│
├── venv/
├── requirements.txt  <-- add this to git
├── manage.py
└── myproject/

```

## 🟥 6. Add .gitignore (IMPORTANT)

```bash
venv/
__pycache__/
*.pyc
db.sqlite3


```

## someone want to clone

git clone <repo>
cd myproject
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python manage.py runserver
