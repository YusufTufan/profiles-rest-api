# 👤 Profiles REST API

This is a **User Profile REST API** built with **Django** and **Django REST Framework**. It handles user authentication, profile management, and feed updates. The project is configured to run in a virtualized environment using **Vagrant**.

## 🚀 Features

* 🔐 **User Authentication:** Create account, login, and token-based authentication.
* 👤 **Profile Management:** Create, view, and update user profiles.
* 📡 **Feed API:** Users can post status updates and view feeds.
* 🐳 **Virtualized Environment:** Fully configured **Vagrant** setup for consistent development.

## 🛠️ Tech Stack

* **Language:** Python 3
* **Framework:** Django & Django REST Framework
* **Virtualization:** Vagrant & VirtualBox
* **Database:** SQLite (Dev) / PostgreSQL (Prod ready)
* **Editor Used:** Atom

## ⚙️ Installation & Setup

This project uses **Vagrant** to create a reproducible development environment.

### Prerequisites
* [VirtualBox](https://www.virtualbox.org/)
* [Vagrant](https://www.vagrantup.com/)

### Running via Vagrant (Recommended)

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YusufTufan/profiles-rest-api.git](https://github.com/YusufTufan/profiles-rest-api.git)
   cd profiles-rest-api
   ```
2. Start the virtual machine:
   ```bash
   vagrant up
   ```
3. SSH into the server:
   ```bash
   vagrant ssh
   ```
4. Run the server (inside the VM):
   ```bash
   cd /vagrant
   python manage.py runserver 0.0.0.0:8000
   ```
   The API will be accessible at http://127.0.0.1:8000/.

Running Locally (Without Vagrant)
1. Create a virtual environment:
  ```bash
  python -m venv venv
  source venv/bin/activate  # On Windows: venv\Scripts\activate
  ```

2. Install dependencies:
  ```bash
  pip install -r requirements.txt
  ```

3. Run migrations and start server:
  ```bash
  python manage.py migrate
  python manage.py runserve
  ```

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

Copyright (c) 2025 YusufTufan
