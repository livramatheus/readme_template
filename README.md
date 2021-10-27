

<h1 align="center">⛅ React Weather Forecast (back-end)</h1>

- [English documentation](#english-documentation)
- [Documentação em português](#documentação-em-português)

____
<h1 id="english-documentation">English Documentation</h1>
<h2>📜 Table of content</h2>

<ul>
	<li><a href="#about-the-project">About the project</a></li>
	<li><a href="#features">Features</a></li>
	<li><a href="#front-end">Front-end</a></li>
	<ul>
		<li><a href="#layout">Layout</a></li>
		<li><a href="#technologies-front">Technologies</a></li>
	</ul>
	<li><a href="#back-end">Back-end</a></li>
	<ul>
		<li><a href="#external-apis">External APIs</a></li>
		<li><a href="#technologies-back">Technologies</a></li>
	</ul>
	<li><a href="#database">Database</a></li>
	<li><a href="#how-to-set-up">How to set up</a></li>
	<li><a href="#inspirations">Inspirations</a></li>
	<li><a href="#live-demo">Live demo</a></li>
	<li><a href="#author">Author</a></li>
</ul>
 
><b>🤚 This repository is the server-side of Weather Forecast, if you are interested on client-side, check <a href="https://github.com/livramatheus/weather-forecast-front">this repository</a>!</b>
<h2 id="about-the-project">💻 About the project</h2>

This is a <b>weather forecast</b> application, that delivers a simple, clean and minimalist layout, projected for desktop and phone screens. This app was built using <em>React</em> and <em>Node</em>.

The main goal with this project was to <b>release a simple yet complete</b> weather forecast app that delivery essential information without transmitting an empty feeling.

<h2 id="features">🔎 Features</h2>

This application obtains user's current location and returns back to the client his city and district name, current weather conditions, detailed weather forecast for the current date and minimal and maximum temperature for the next days.

<h2 id="front-end">Front-end</h2>

The client-side of <b>Weather Forecast</b> was built with React, resulting in the following layout:

<h3 id="layout">📐 Layout</h3>

<h4>Mobile</h4>
<div style="display: flex">
	<img alt="Mobile 1" title="#1_m" src="https://github.com/livramatheus/weather-forecast-front/raw/main/src/assets/1_m.png" height="280"/>
	<img alt="Mobile 2" title="#2_m" src="https://github.com/livramatheus/weather-forecast-front/raw/main/src/assets/2_m.png" height="280"/>
</div>

<h4>Desktop</h4>
<div style="display: flex">
	<img alt="Desktop 1" title="#1_d" src="https://github.com/livramatheus/weather-forecast-front/raw/main/src/assets/1_d.png" height="280"/>
	<img alt="Desktop 2" title="#2_d" src="https://github.com/livramatheus/weather-forecast-front/raw/main/src/assets/1_d.png" height="280"/>
</div>

<h3 id="technologies-front">🔨 Technologies</h3>

The following techlogies were used to build Weather Forecast's front-end:
<ul>
	<li><a href="https://github.com/axios/axios">Axios</a></li>
	<li><a href="https://mui.com/">Material UI</a></li>
	<li><a href="https://www.npmjs.com/package/react-loading-skeleton">React Loading Skeleton</a></li>
	<li><a href="https://www.npmjs.com/package/react-router-dom">React Router Dom</a></li>
</ul>

<h2 id="back-end">Back-end</h2>

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

<h3 id="external-apis">💱 External APIs</h3>
	
The following third party APIs were used to create Weather Forecast's API responses:
- [Open Weather Map](https://openweathermap.org/) for weather data
- [LocationIQ](https://locationiq.com/) for reverse geolocation
 
<h3 id="technologies-back">🔨 Technologies</h3>

The following techlogies were used to build Weather Forecast server:
- [Cors](https://www.npmjs.com/package/cors)
- [Express](https://www.npmjs.com/package/express)
- [Axios](https://github.com/axios/axios)

<h2 id="database">Database</h2>

MWG's database of choice was [MySql](https://www.mysql.com). Check out a brief description of the tables:
- **tbexercise:** stores a wide set of available exercies;
- **tbgroup:** stores muscle group divisions;
- **tblevel:** stores possible user's level;
- **tbstimulus:** stores advanced variations for a exercise;
- **tbworkout:** stores generated workouts basic info;
- **tbworkoutexercise:** sotres relations between a workout and exercise. Many-to-many table.

<h3 id="how-to-set-up">❓ How to set up</h3>

If you wish to fork this project you'll need to set up the following environment variables:

#### Client-side:
- **REACT_APP_BACK_URL** (Server URL in order to send requests)

#### Server-side:
- **API_GEO** (LocationIQ API key)
- **API_WEATHER** (Open Weather Map API key)
- **PORT** (Desired port to run express)

<h3 id="inspirations">😁 Inspirations</h3>

Weather Forecast was inspired by the following projects on Figma:
- [Weather Icons | Flat & Outline](https://www.figma.com/community/file/955978734883254712)
- [Weather Forecast App](https://www.figma.com/file/fXpD0piPYygazRk9mAXQH9/Weather-Forecast-App-(Community))

<h3 id="live-demo">🌐 Live demo</h3>

Check out this project running on [Netlify + Heroku](https://livramento-weather.netlify.app/)

You can also edit and view this project on Code Sand Box:

#### Front-end:
[![Edit Weather Forecast (Front)](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/weather-forecast-front-465th?fontsize=14&hidenavigation=1&theme=dark)

#### Back-end:
[![Edit Weather Forecast (Back)](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/weather-forecast-back-z8nuo?fontsize=14&hidenavigation=1&theme=dark)

<h3 id="author">👩‍🦲 Author</h3>

Full stack developed by **Matheus do Livramento**.

[GitHub](https://github.com/livramatheus) | [LinkedIn](https://www.linkedin.com/in/livramatheus)

____
# Documentação em português
<h2>📜 Tabela de conteúdo</h2>

<!--ts-->
<ul>
	<li><a href="#about-the-project-br">Sobre o projeto</a></li>
	<li><a href="#features-br">Funcionalidades</a></li>
	<li><a href="#front-end-br">Front-end</a></li>
	<ul>
		<li><a href="#layout-br">Layout</a></li>
		<li><a href="#technologies-front-br">Tecnologias</a></li>
	</ul>
	<li><a href="#back-end-br">Back-end</a></li>
	<ul>
		<li><a href="#external-apis-br">APIs externas</a></li>
		<li><a href="#technologies-back-br">Technologies</a></li>
	</ul>
	<li><a href="#database-br">Banco de dados</a></li>
	<li><a href="#how-to-set-up-br">Como configurar</a></li>
	<li><a href="#inspirations-br">Inspirações</a></li>
	<li><a href="#live-demo-br">Live demo</a></li>
	<li><a href="#autor-br">Autor</a></li>
</ul>
<!--te-->
 
>**🤚 🤚 Este repositório é do lado do servidor da Previsão do Tempo, se você estiver interessado no lado do cliente, verifique [este repositório](https://github.com/livramatheus/weather-forecast-front)!**

<h2 id="about-the-project-br">💻 Sobre o projeto</h2>

Trata-se de um aplicativo de **previsão do tempo**, que oferece um layout simples, clean e minimalista, projetado para telas de desktops e dispositivos móveis. Este aplicativo foi desenvolvido usando *React* e *Node*.

O principal objetivo com este projeto era **lançar um aplicativo de previsão do tempo simples, mas completo**, que entregasse informações essenciais sem transmitir uma sensação de vazio.

<h2 id="features-br">🔎 Funcionalidades</h2>

Este aplicativo obtém a localização atual do usuário e retorna ao cliente o nome de sua cidade e bairro, condições climáticas atuais, previsão do tempo detalhada para a data atual e temperatura mínima e máxima para os próximos dias.

<h2 id="front-end-br">Front-end</h2>

O lado do cliente de **Weather Forecast** foi construído com React, resultando no seguinte layout:

<h3 id="layout-br">📐 Layout</h3>

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

<h3 id="technologies-front-br">🔨 Tecnologias</h3>

As seguintes tecnologias foram utilizadas para construir o front-end de Weather Forecast:
- [Axios](https://github.com/axios/axios)
- [Material UI](https://mui.com/)
- [React Loading Skeleton](https://www.npmjs.com/package/react-loading-skeleton)
- [React Router Dom](https://www.npmjs.com/package/react-router-dom)

<h2 id="back-end-br">Back-end</h2>

O back-end consiste em um servidor desenvolvido com Express Framework para Node, que escuta as solicitações acionadas pela camada front-end da aplicação.

Este servidor Node tem um único endpoint que retorna um conjunto de dados meteorológicos e a localização específica do usuário:

- /forecast: espera dois parâmetros por *query string*:
	- **lat:** latitude do usuário
	- **long:** longitude do usuário

- Retorna:
	- Cidade e bairro atuais do usuário por meio de *reverese geolocation*
	- Condições climáticas atuais, como temperatura, velocidade do vento e umidade
	- Previsão meteorológica detalhada para a data atual
	- Temperatura mínima e máxima para os próximos dias

Exmplo:
> /forecast?lat=-23.5549053&long=-46.4673641

<h3 id="external-apis-br">💱 APIs externas</h3>

As seguintes APIs de terceiros foram usadas para criar respostas da API de **Weather Forecast**:
- [Open Weather Map](https://openweathermap.org/) para dados climáticos
- [LocationIQ](https://locationiq.com/) para o *reverse geolocation*
 
<h3 id="technologies-back-br">🔨 Tecnologias</h3>

As seguintes tecnologias foram utilizadas para desenvolver o sevidor de **Weather Forecast**:
- [Cors](https://www.npmjs.com/package/cors)
- [Express](https://www.npmjs.com/package/express)
- [Axios](https://github.com/axios/axios)

<h2 id="database-br">Banco de Dados</h2>

O banco de dados escolhido para desenvolver MWG foi o [MySql](https://www.mysql.com). Veja a seguir uma breve descrição de suas tabelas:
- **tbexercise:** armazena uma vasta gama de exercícios;
- **tbgroup:** armazena as divisões musculares;
- **tblevel:** armazena os possíveis níveis atléticos do usuário;
- **tbstimulus:** armazena variantes avançadas para algum exercício;
- **tbworkout:** armazena informações básicas de um treinamento;
- **tbworkoutexercise:** armazena uma relação entre treinamento e exercício. É uma tabela muitos para muitos.

<h3 id="how-to-set-up-br">❓ Como configurar</h3>

Se você deseja fazer um *fork* deste projeto, você precisará configurar as seguintes variáveis de ambiente:

#### Client-side:
- **REACT_APP_BACK_URL** (URL do back-end para disparar requisições)

#### Server-side:
- **API_GEO** (Chave de API de LocationIQ)
- **API_WEATHER** (Chave de API de Open Weather Map)
- **PORT** (Porta desejada pra rodar o servidor)

<h3 id="inspirations-br">😁 Inspirações</h3>

Weather Forecast foi inspirado pelos seguintes projetos do Figma:
- [Weather Icons | Flat & Outline](https://www.figma.com/community/file/955978734883254712)
- [Weather Forecast App](https://www.figma.com/file/fXpD0piPYygazRk9mAXQH9/Weather-Forecast-App-(Community))

<h3 id="live-demo-br">🌐 Live demo</h3>

Veja este projeto rodando no [Netlify + Heroku](https://livramento-weather.netlify.app/)

Você também pode visualizar e editar este código no Code Sand Box:

#### Front-end:
[![Edit Weather Forecast (Front)](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/weather-forecast-front-465th?fontsize=14&hidenavigation=1&theme=dark)

#### Back-end:
[![Edit Weather Forecast (Back)](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/weather-forecast-back-z8nuo?fontsize=14&hidenavigation=1&theme=dark)

<h3 id="autor-br">👩‍🦲 Author</h3>

Full stack  desenvolvido por **Matheus do Livramento**.

[GitHub](https://github.com/livramatheus) | [LinkedIn](https://www.linkedin.com/in/livramatheus)
