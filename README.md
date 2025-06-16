# Telusko Django Travel App

The **Telusko Django App** is a travel booking platform where users can explore destinations, view details about places, and discover special offers on travel packages. It is built using Django and PostgreSQL, with a clean interface for both users and admins.

---

## ✈️ Features

- **Add & View Destinations**  
  Admins can add travel destinations with descriptions, images, and pricing. Users can browse through a list of places to visit.

- **Place Name & Descriptions**  
  Each destination includes:
  - Name of the place
  - Image of the location
  - Short description
  - Price or cost per package

- **Special Offers**  
  Highlight travel destinations with special discounts. Offers can be marked and displayed on the homepage.

- **Dynamic Homepage**  
  Homepage displays a list of available travel spots with promotional banners and trending places.

- **Admin Panel**  
  A powerful admin panel to add/edit/delete:
  - Travel destinations
  - Special offers
  - User management

---

.

---

## 🔧 Tech Stack

- **Backend:** Django (Python)
- **Frontend:** HTML, CSS, Bootstrap
- **Database:** PostgreSQL
- **Admin Tools:** Django Admin

---
## How to Run the Project Locally

### Step 1: Clone the Repository
Clone the repository and navigate to the project directory:
```bash
git clone https://github.com/Malan-J/Travelapp-Django.git
cd Travelapp-Django
```

### Step 2: Create a Virtual Environment
Create and activate a virtual environment:

**For Windows:**
```bash
python -m venv venv
venv\Scripts\activate
```

**For macOS/Linux:**
```bash
python3 -m venv venv
source venv/bin/activate
```

You should now see something like `(venv)` at the beginning of your command line prompt.

### Step 3: Install Django
Once the virtual environment is activated, install Django and go to the project folder:
```bash
pip install django
cd telusko
```

### Step 4: Install PostgreSQL
Make sure PostgreSQL is installed and **pgAdmin is running** in the background.

### Step 5: Create a Database in pgAdmin
- Open pgAdmin  
- Create a new database named `malan`  
- Set the PostgreSQL password to `1234`  
- If you use a different name or password, update the `DATABASES` section in `settings.py` accordingly

### Step 6: Connect Django to PostgreSQL and Set Up the Project
Run the following commands one by one:
```bash
pip install psycopg2
pip install Pillow
python manage.py makemigrations
python manage.py migrate
```

### Step 7: Run the Django Server
Start the development server:
```bash
python manage.py runserver
```

### Access the App
Open your browser and go to:
```
http://127.0.0.1:8000
```

You can now use the Django project locally.
