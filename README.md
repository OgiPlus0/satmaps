# SatMaps
![WhatsApp Görsel 2023-07-27 saat 17 20 08](https://github.com/OgiPlus0/satmaps/assets/108802411/d4577a06-3162-4bbd-ba0b-cc7748a4cd64)

 Empowering Sustainable Investments! At SatMaps, we understand the increasing expectation from stakeholders for corporate commitment to biodiversity preservation. Our AI-based website offers predictions and suggestions for your future investments, while our chatbots alert you about potential side effects on local biodiversity. With our satellite-image-based map, you can confidently select environmentally responsible locations. Say goodbye to scattered and contradictory data; SatMaps brings all the information you need in one user-friendly platform. Make a positive impact on the environment while ensuring business success. Join us now and shape a greener future!

 ## Technical Demo of Our Project

 [![Our Video](https://github.com/OgiPlus0/satmaps/assets/108802411/35142845-fc50-4a0c-8a63-15897f525850)]( https://www.youtube.com/watch?v=4vUPuomWYrc)


## How We Will Develop This Project 

Let me show you how we will do it.

We will basicly use HTML + CSS at the frontend side of this project, and we will use JS + PHP in the backend side. For storing the users datas, we will use SQL and for the implementing ai to our project, we will use pyhton

While we are using HTML + CSS + JS + PHP we will use VSCode. We will use phpMyAdmin for testing our SQL codes. And We would build up this website to a real server. For developing the ai side by pyhton we will use Google Colab

 In the chatbot side as you know the best solution is OpenAI API, so we will use gpt-3.5-turbo . And in the map side  we think the best solution is providing by Yandex Map, so we will use Yandex.Maps API in there.

 So for using the OpenAI API

 ```
import openai

completion = openai.ChatCompletion.create(
  model="gpt-3.5-turbo", 
  messages=[{"role": "user", "content": "What is the OpenAI mission?"}]
)

print(completion)
```

We will use this code block. And Here is a introduction to using OpenAI API "https://openai.com/blog/introducing-chatgpt-and-whisper-apis" You can reach it very easily.

And for using the Yandex.Maps API we will use JS 

```
<html>
<head>
    <title>Examples. Setting a custom placemark image</title>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
    <!--
        Set your own API-key. Testing key is not valid for other web-sites and services.
        Get your API-key on the Developer Dashboard: https://developer.tech.yandex.ru/keys/
    -->
    <script src="https://api-maps.yandex.ru/2.1/?lang=en_RU&amp;apikey=<your API-key>" type="text/javascript"></script>
    <script src="icon_customImage.js" type="text/javascript"></script>
	<style>
        html, body, #map {
            width: 100%; height: 100%; padding: 0; margin: 0;
        }
    </style>
</head>
<body>
<div id="map"></div>
</body>
</html>
```

This code block is the easist way of using Yandex.Maps API at our project. You can reach more thing from here "https://yandex.com.tr/dev/maps/jsbox/2.1/" 
