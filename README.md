# On-road Vehicle Breakdown Assistance Finder

This is a Django-based web application to help users find vehicle breakdown assistance services nearby.

## Features
- User registration and login
- Mechanic registration
- Service request management
- Profile management with profile picture upload
- Payment integration (Stripe)

## Setup Instructions

### Prerequisites
- Python 3.8 or higher installed on your system
- Git installed (for cloning the repository)

### Step-by-Step Setup

1. **Clone the repository:**
   ```sh
   git clone https://github.com/Hruthikgowdahk/On-road-vehicle-breakdown-assistance-finder.git
   ```

2. **Navigate to the project directory:**
   ```sh
   cd On-road-vehicle-breakdown-assistance-finder
   ```

3. **Create a virtual environment (recommended):**
   
   **Windows:**
   ```sh
   python -m venv venv
   ```
   
   **macOS/Linux:**
   ```sh
   python3 -m venv venv
   ```

4. **Activate the virtual environment:**
   
   **Windows (PowerShell):**
   ```sh
   .\venv\Scripts\Activate.ps1
   ```
   
   **Windows (Command Prompt):**
   ```sh
   venv\Scripts\activate.bat
   ```
   
   **macOS/Linux:**
   ```sh
   source venv/bin/activate
   ```
   
   **Note:** If activation doesn't work on Windows, you can use the Python executable directly (see step 6).

5. **Install dependencies:**
   ```sh
   pip install -r requirements.txt
   ```
   
   **Note:** If Pillow installation fails, try: `pip install Pillow --upgrade`
   **Note:** psycopg2-binary is optional (only needed for PostgreSQL). If it fails, you can skip it as the project uses SQLite by default.

6. **Run database migrations:**
   ```sh
   python index.py migrate
   ```
   
   **Windows (if activation didn't work):**
   ```sh
   .\venv\Scripts\python.exe index.py migrate
   ```

7. **Create a superuser (optional, for admin access):**
   ```sh
   python index.py createsuperuser
   ```
   
   **Windows (if activation didn't work):**
   ```sh
   .\venv\Scripts\python.exe index.py createsuperuser
   ```

8. **Start the development server:**
   ```sh
   python index.py runserver
   ```
   
   **Windows (if activation didn't work):**
   ```sh
   .\venv\Scripts\python.exe index.py runserver
   ```

9. **Access the application:**
   - Open your browser and navigate to: **http://127.0.0.1:8000/** or **http://localhost:8000/**

## Usage
- Access the app at [http://127.0.0.1:8000/](http://127.0.0.1:8000/)
- Register as a user or mechanic
- Request or provide breakdown assistance

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details. 