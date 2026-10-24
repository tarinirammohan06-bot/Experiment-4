# Weather Information App 🌦️

## 📌 Aim
To develop a weather application using JavaScript ES6 features to fetch and display weather information.

## 📝 Description
This project is a weather information application that retrieves weather data for a specified city using the **OpenWeatherMap API**.

The backend is built using Node.js and Express.js. Axios is used to send HTTP requests to the weather API, while JavaScript Promises and `async/await` handle asynchronous operations.

The application returns the city's temperature in Celsius.

## ✨ Features
- Fetch weather information for a specified city.
- Retrieve real-time weather data from OpenWeatherMap.
- Display temperature in Celsius.
- Use `async/await` for asynchronous operations.
- Handle errors when weather data cannot be retrieved.
- Serve frontend files through Express.js.

## 🛠️ Technologies Used
- **HTML, CSS, JavaScript** — Frontend
- **Node.js** — JavaScript runtime
- **Express.js** — Backend server
- **Axios** — HTTP requests
- **OpenWeatherMap API** — Weather data provider
- **JavaScript ES6** — Promises and `async/await`

## 📂 Project Structure

```text
weather-information-app/
├── public/                 # Frontend files
│   ├── index.html
│   ├── style.css
│   └── script.js
├── server.js               # Backend server
├── package.json            # Project dependencies
├── package-lock.json       # Dependency lock file
├── approachofexperiment.md # Project guide
└── README.md               # Project documentation
```

*Note: The frontend filenames shown above are examples. Keep the actual filenames in your repository.*

## ⚙️ Installation and Setup

### Prerequisites
- Node.js and npm installed.
- An OpenWeatherMap API key.

### Step 1: Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

Replace `YOUR_GITHUB_REPOSITORY_URL` with your GitHub repository URL.

### Step 2: Navigate to the project folder

```bash
cd weather-information-app
```

### Step 3: Install dependencies

```bash
npm install
```

### Step 4: Configure the API key

Obtain an API key from [OpenWeatherMap](https://openweathermap.org/api).

Store your API key securely as an environment variable named `OPENWEATHER_API_KEY`. Update `server.js` to read the key from the environment instead of hardcoding it.

### Step 5: Start the backend server

```bash
node server.js
```

The server should display:

```text
Server running at http://localhost:3000
```

### Step 6: Open the application

Open the following address in your browser:

http://localhost:3000

You can also test the weather endpoint by visiting:

```text
http://localhost:3000/weather/London
```

Replace `London` with the name of another city.

## 🔌 API Endpoint

**Endpoint:** `/weather/:city`

**Method:** GET

**Example request:**

```text
GET /weather/London
```

**Example response:**

```json
{
  "temperature": 18.5
}
```

The temperature shown is an illustrative example; the actual value depends on the weather API response.

## 🔄 How It Works

1. The user requests weather information for a city.
2. The Express.js server receives the request.
3. Axios sends a request to the OpenWeatherMap API.
4. The API returns the weather data.
5. JavaScript `async/await` handles the asynchronous request.
6. The server extracts the temperature and returns it as JSON.
7. If an error occurs, the server returns an error response.

## 🎯 Learning Outcomes

- Understand JavaScript ES6 features.
- Learn how to use Promises and `async/await`.
- Understand REST API requests.
- Build a basic backend using Express.js.
- Use Axios to retrieve external API data.
- Handle errors in asynchronous applications.

## 🔮 Future Improvements

- Display humidity, wind speed, and weather conditions.
- Add a weather search interface.
- Improve error messages for invalid city names.
- Add responsive styling for mobile devices.
- Display weather icons and forecasts.


