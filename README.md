

<h1 align="center">⛅ React Weather Forecast (back-end)</h1>

- [English documentation](#english-documentation)
- [Documentação em português](#documentação-em-português)

____
# English Documentation
## 📜 Table of content
<!--ts-->
- [About the project](#-about-the-project)
- [Features](#-features)
- [Front-end](#front-end)
	- [Layout](#-layout)
	- [Technologies](#technologies-front)
- [Back-end](#back-end)
	- [External APIs](#-external-apis)
	- [Technologies](#technologies-back)
- [How to set up](#-how-to-set-up)
- [Inspirations](#-inspirations)
- [Live demo](#-live-demo)
- [Author](#-author)
<!--te-->
 
>**🤚 This repository is the server-side of Weather Forecast, if you are interested on client-side, check it's [own repository](https://github.com/livramatheus/weather-forecast-front)!**

## 💻 About the project

This is a **weather forecast** application, that delivers a simple, clean and minimalist layout, projected for desktop and phone screens. This app was built using *React* and *Node*.

The main goal with this project was to **release a simple yet complete** weather forecast app. In a way that I couldn't over engineer it or put way too much time on it, I decided to release the application at it's current state. In conclusion, **Weather Forecast** is considered completed as its current state.

## 🔎 Features

This application obtains user's current location and returns backto the client his city and district name, current weather conditions, detailed weather forecast for the current date and minimal and maximum temperature for the next days.

##  Front-end
The client side of **Weather Forecast** was built with React, resulting in the following layout:

### 📐 Layout
#### Mobile
<div style="display: flex">
	<img alt="Mobile 1" title="#1_m" src="https://github.com/livramatheus/weather-forecast-front/raw/main/src/assets/1_m.png" height="280"/>
	<img alt="Mobile 2" title="#2_m" src="https://github.com/livramatheus/weather-forecast-front/raw/main/src/assets/2_m.png" height="280"/>
</div>

#### Desktop
<div style="display: flex">
	<img alt="Desktop 1" title="#1_d" src="https://github.com/livramatheus/weather-forecast-front/raw/main/src/assets/1_d.png" height="280"/>
	<img alt="Desktop 2" title="#2_d" src="https://github.com/livramatheus/weather-forecast-front/raw/main/src/assets/1_d.png" height="280"/>
</div>

### <span id="technologies-front">🔨 Technologies</span>
The following techlogies were used to build Weather Forecast's front-end:
- [Axios](https://github.com/axios/axios)
- [Material UI](https://mui.com/)
- [React Loading Skeleton](https://www.npmjs.com/package/react-loading-skeleton)
- [React Router Dom](https://www.npmjs.com/package/react-router-dom)

##  Back-end
The back-end consists in a server developed with Express Framework for Node, which listens to request triggered by the the front-end layer of the application.

This Node server has a sole endpoint that returns a set of weather data and user's specific location:

* **/forecast**: expects two parameters as *query string*:
	- **lat:** user´s latitude
	- **long:** user´s longitude

* Returns:
	- User's current city and district through reverese geolocation
	- Current weather conditions, like temperature, wind speed and humidity
	- Detailed weather forecast for the current date
	- Minimal and maximum temperature for the next days

Example:
> /forecast?lat=-23.5549053&long=-46.4673641

### 💱 External APIs

The following third party APIs were used to create Weather Forecast's API responses:
- [Open Weather Map](https://openweathermap.org/) for weather data
- [LocationIQ](https://locationiq.com/) for reverse geolocation
 
### <span id="technologies-back">🔨 Technologies</span>

The following techlogies were used to build Weather Forecast server:
- [Cors](https://www.npmjs.com/package/cors)
- [Express](https://www.npmjs.com/package/express)
- [Axios](https://github.com/axios/axios)

### ❓ How to set up
If you wish to fork this project you'll need to set up the following environment variables:
#### Client-side:
- **REACT_APP_BACK_URL** (Server URL in order to send requests)

#### Server-side:
- **API_GEO** (LocationIQ API key)
- **API_WEATHER** (Open Weather Map API key)
- **PORT** (Desired port to run express)

### 😁 Inspirations

Weather Forecast was inspired by the following projects on Figma:
- [Weather Icons | Flat & Outline](https://www.figma.com/community/file/955978734883254712)
- [Weather Forecast App](https://www.figma.com/file/fXpD0piPYygazRk9mAXQH9/Weather-Forecast-App-(Community))

### 🌐 Live demo

Check out this project running on [Netlify + Heroku](https://livramento-weather.netlify.app/)

Edit this Node server on CodeSandbox.

#### Front-end:
[![Edit Weather Forecast (Front)](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/weather-forecast-front-465th?fontsize=14&hidenavigation=1&theme=dark)

#### Back-end:
[![Edit Weather Forecast (Back)](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/weather-forecast-back-z8nuo?fontsize=14&hidenavigation=1&theme=dark)

### 👩‍🦲 Author
Full stack developed by **Matheus do Livramento**.

[GitHub](https://github.com/livramatheus) | [LinkedIn](https://www.linkedin.com/in/matheus-livramento-623590209/)

____
# Documentação em português
