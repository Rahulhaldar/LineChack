# MyPartnerisBusy

## Getting Started

These instructions will help you set up and run the project on your local machine for development and testing purposes.

### Prerequisites

- Python (3.x recommended)
- pip (Python package installer)
- Virtualenv (optional but recommended)
- Twillio Account

### Installing

1. Clone the repository to your local machine:

2. Navigate to the project directory:

    ```bash
    cd mypartnerisbusy
    ```

3. Create a virtual environment (optional but recommended):

    ```bash
    python -m venv venv
    ```

4. Activate the virtual environment:

    - On Windows:

        ```bash
        venv\Scripts\activate
        ```

    - On macOS/Linux:

        ```bash
        source venv/bin/activate
        ```

5. Install project dependencies:

    ```bash
    pip install -r requirements.txt
    ```

### Database Setup

1. Apply database migrations:

    ```bash
    python manage.py migrate
    ```

2. Create a superuser account (for admin access):

    ```bash
    python manage.py createsuperuser
    ```

### Running the Server

Start the development server:

```bash
python manage.py runserver
  ```
### Finally Update The Settings.py 

TWILIO_ACCOUNT_SID = 'YOUR TWILIO ACCOUNT SID'
TWILIO_AUTH_TOKEN = 'YOUR TWILIO AUTH_TOKEN'
TWILIO_PHONE_NUMBER = 'YOUR TWILLIO PHONE NUMBER'

### Update Your Webhook URL in myapp/views.py line 46 You can use ngrok to generate a url

  status_callback='https://7264-103-212-158-183.ngrok-free.app/twilio_webhook/',



 


