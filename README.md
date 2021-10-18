
<h1 align="center">⛅ React Weather Forecast</h1>

- [English documentation](#english-documentation)
- [Documentação em português](#documentação-em-português)

____
# English Documentation
## 📜 Table of content
<!--ts-->
- [About the project](#-about-the-project)
- [Back-end](#back-end)
	- [Features](#-features)
	- [External APIs](#-external-apis)
	- [Technologies](#-technologies)
	- [How to set up](#-how-to-set-up)
- [Front-end](#front-end)
- [Full stack](#full-stack)
- [Inspirations](#-inspirations)
- [Live demo](#-live-demo)
- [Author](#-author)
<!--te-->
 
## 💻 About the project

This is a **weather forecast** application, that delivers a simple, clean and minimalist layout, projected for desktop and phone screens. This app was built using *React* and *Node*. The current repository/documentation explanate about the **back-end** section of this project, however, you can also check out the [front-end](#-front-end) and [full stack](#-full-stack) repositories.

The main goal with this project was to **release a simple yet complete** weather forecast app. In a way that I couldn't over engineer it or put way too much time on it, I decided to release the application at it's current state. In conclusion, for now I consider the **Weather Forecast** completed, but more features could be added later on.

##  Back-end
The back-end consists in a server developed with Express Framework for Node, which listens to request triggered by the the front-end layer of the application.

### 🔎 Features
This Node server has a sole endpoint that returns a set of weather data and user's specific location:

* **/previsao**: expects two parameters as *query string*:
	- **lat:** user´s latitude
	- **long:** user´s longitude

* Returns:
	- User's current city and district through reverese geolocation
	- Current weather conditions, like temperature, wind speed and humidity
	- Detailed weather forecast for the current date
	- Minimal and maximum temperature for the next days

Example:
> /previsao?lat=-23.5549053&long=-46.4673641

### 💱 External APIs

The following third party APIs were used to create Weather Forecast's API responses:
- [Open Weather Map](https://openweathermap.org/) for weather data
- [LocationIQ](https://locationiq.com/) for reverse geolocation
 
### 🔨 Technologies

The following techlogies were used to build Weather Forecast server:
- [Cors](https://www.npmjs.com/package/cors)
- [Express](https://www.npmjs.com/package/express)
- [Axios](https://github.com/axios/axios)

### ❓ How to set up
If you wish to fork this server you'll need to set up the following environment variables:
- **API_GEO** (LocationIQ API key)
- **API_WEATHER** (Open Weather Map API key)
- **PORT** (Desired port to run express)

##  Front-end
The front-end section of **Weather Forecast** was built with React. You can read more about it on its own [GitHub repository](https://github.com/livramatheus/weather-forecast-front).

##  Full Stack
You can also check out the front and back-end sections of **Weather Forecast** bundled in a single [GitHub repository](https://github.com/livramatheus/weather-forecast).

### 😁 Inspirations

Weather Forecast was inspired by the following projects on Figma:
- [Weather Icons | Flat & Outline](https://www.figma.com/community/file/955978734883254712)
- [Weather Forecast App](https://www.figma.com/file/fXpD0piPYygazRk9mAXQH9/Weather-Forecast-App-(Community))

### 🌐 Live demo

Check out this project running on [Netlify + Heroku](https://livramento-weather.netlify.app/)

Edit this Node server on CodeSandbox.

[![Edit Weather Forecast (Back)](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/weather-forecast-back-z8nuo?fontsize=14&hidenavigation=1&theme=dark)

### 👩‍🦲 Author
Full stack developed by **Matheus do Livramento**.

[GitHub](https://github.com/livramatheus) | [LinkedIn](https://www.linkedin.com/in/matheus-livramento-623590209/)

____
# Documentação em português
