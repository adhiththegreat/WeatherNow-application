# WeatherNow-application
☀️ A simple desktop weather app built with Python, PyQt5, and the OpenWeatherMap API.
# PyQt5 Weather App ☀️

A simple, stylish desktop weather application built with Python, PyQt5, and the OpenWeatherMap API. It allows you to enter a city name and get the current temperature, weather description, and a corresponding emoji.

## Screenshot


<img width="402" height="527" alt="image" src="https://github.com/user-attachments/assets/0f24e67e-9a42-4881-9219-e9ddd19262dc" />


## Features

* **Current Weather:** Get the temperature (in Fahrenheit), a short description, and the city name.
* **Weather Emoji:** Displays a dynamic emoji (e.g., ☀️, ☁️, 🌧️, ❄️) that matches the current weather conditions.
* **Clean UI:** A simple and clean user interface built with PyQt5 and styled with QSS (Qt Style Sheets).
* **Error Handling:** Provides user-friendly messages for common errors, such as:
    * Invalid city name (404 Not Found)
    * Invalid API key (401 Unauthorized)
    * Network/connection issues

## Technologies Used

* **Python 3**
* **PyQt5:** For the graphical user interface (GUI).
* **Requests:** For making HTTP requests to the weather API.
* **OpenWeatherMap API:** As the source of weather data.

## Setup and Installation

Follow these steps to get the application running on your local machine.

### 1. Clone the Repository

```bash
git clone [https://github.com/your-username/pyqt-weather-app.git](https://github.com/your-username/pyqt-weather-app.git)
cd pyqt-weather-app
```
(Replace `your-username/pyqt-weather-app` with your actual repository URL.)

### 2. Create a Virtual Environment (Recommended)

```bash
# For Windows
python -m venv venv
.\venv\Scripts\activate

# For macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies

This project depends on `PyQt5` and `requests`. You can install them directly or from a `requirements.txt` file.

**Recommended:** Create a file named `requirements.txt` in your project folder with the following content:
```
PyQt5
requests
```
Then, install the requirements:
```bash
pip install -r requirements.txt
```

### 4. Configure Your API Key (IMPORTANT!)

The app requires a free API key from OpenWeatherMap.

1.  Sign up for a free account at [OpenWeatherMap.org](https://openweathermap.org/).
2.  Go to your user dashboard and find your API key.
3.  Open the Python script (e.g., `main.py` or `app.py`).
4.  Find this line:
    ```python
    api_key = "0dca3ec1d43e25b3b06bc2f42194924b"
    ```
5.  **Replace the string** with your **own** personal API key.

> **Security Note:** It is not secure to hardcode API keys directly in your code, especially if the repository is public. For a more advanced project, consider using environment variables (`os.environ.get('API_KEY')`) to keep your key private.

## Usage

Once you have installed the dependencies and configured your API key, you can run the application:

```bash
python your_script_name.py
```
(Replace `your_script_name.py` with the name of your Python file.)

## License

This project is licensed under the MIT License.
