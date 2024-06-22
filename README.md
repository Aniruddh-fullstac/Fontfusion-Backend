# FontFusion Backend

The backend for the FontFusion application is designed to handle all font blending, Google Fonts integration, and funky font management services. This guide will walk you through the steps to set up and run the backend server locally, and how to expose it to the internet using Ngrok.

## Getting Started

### Prerequisites
- Python 3.8+
- pip (Python package installer)
- Ngrok (for exposing the local server)

### Installation

1. **Clone the Repository:**
    ```sh
    git clone https://github.com/Aniruddh-fullstac/Fontfusion-Backend.git
    cd FontFusion-backend
    ```

2. **Install Dependencies:**
    ```sh
    pip install -r requirements.txt
    ```

### Running the Server

1. **Start the Django Server:**
    ```sh
    python manage.py runserver
    ```

    This will start the server at `http://127.0.0.1:8000/`.

2. **Expose Local Server to the Internet using Ngrok:**
    - Download and install Ngrok from [ngrok.com](https://ngrok.com/).
    - Run Ngrok to expose your local server:
      ```sh
      ngrok http 8000
      ```

    Ngrok will provide you with a URL that tunnels to your local server, such as `http://abc123.ngrok.io`.

3. **Copy the Ngrok URL:**
    - Note the URL provided by Ngrok.
    - Include the Ngrok URL and API key in your application configuration.

### Configuration

1. **Environment Variables:**
    - Set up any required environment variables for the application, such as database credentials, secret keys, etc.

2. **API Key Configuration:**
    - Ensure that the application is configured to use the Ngrok URL along with the required API key for secure access.

## Project Structure

Here's a brief overview of the project structure:

```
FontFusion-backend/
│
├── manage.py
├── requirements.txt
├── FontFusion/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
│   └── asgi.py
├── Fusion1/
│   ├── __init__.py
│   ├── views.py
│   ├── models.py
│   ├── serializers.py
│   └── urls.py
└── ...
```

## API Endpoints

Here are some key API endpoints provided by the FontFusion backend:

- **Font Blending:** `/image_process_api/`

- **Fontastic Fonts:** `funky-font/`

_For detailed API documentation, refer to the API documentation provided in the repository._
and check urls.py for more API's

## Contributing

We welcome contributions to the FontFusion backend! If you have any ideas, bug fixes, or improvements, feel free to open an issue or submit a pull request.

### Steps to Contribute
1. **Fork the Repository**
2. **Create a Feature Branch**
    ```sh
    git checkout -b feature/AmazingFeature
    ```
3. **Commit Your Changes**
    ```sh
    git commit -m 'Add some AmazingFeature'
    ```
4. **Push to the Branch**
    ```sh
    git push origin feature/AmazingFeature
    ```
5. **Open a Pull Request**

## License

Distributed under the MIT License. See `LICENSE` for more information.


Get started with FontFusion backend and power your font innovation today!
