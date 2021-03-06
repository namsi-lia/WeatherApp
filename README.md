<h1 align="center">Angular Weather App</h1>

Angular Weather App is a Progressive Web Application (PWA) to get weather forecast.
> **[Progressive Web Apps](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps)** are web apps that use emerging web browser APIs and features along with traditional progressive enhancement strategy to bring a > native app-like user experience to cross-platform web applications.

> **[Progressive Web Apps](https://web.dev/what-are-pwas/)** are built and enhanced with modern APIs to deliver enhanced capabilities, reliability, and installability while reaching anyone, anywhere, on any device with a single codebase.

## Features 🚀
- Get weather forecast by user location.
- Get the weather forecast by searching for a place.
- Can be installed on your mobile phone, tablet and computer.
- Displays the following information:
  - Temperature
  - Weather description
  - Feels like temperature
  - Humidity
  - Wind speed
  - Pollution
  - UV index
  - Hourly and weekly forecast
  - Sunrise and sunset times
  - Visibility
  - Air quality
- The temperature units can be switched between Celsius and Fahrenheit.
- Notify Internet connection status.
- Works offline after first use.
- Notify when an app update is available.


## Built with 🛠️
![Tech stack](https://res.cloudinary.com/comparte/image/upload/v1626424543/weather-app-tech-stack.png)
- [Angular](https://angular.io/) - An Application Design Framework and Development Platform for creating efficient and sophisticated single-page apps.
- [Angular Material](https://material.angular.io/) - Material Design components for Angular.
- [OpenWeather API](https://openweathermap.org/) - Fast and easy-to-work weather APIs.
- [Places API](https://developers.google.com/maps/documentation/places/web-service/overview?hl=en_US) - Get detailed information about 100 million places.
- [Geocoding API](https://developers.google.com/maps/documentation/geocoding/overview?hl=en_US) - Convert between addresses and geographic coordinates.
- [Web APIs for Angular](https://ng-web-apis.github.io/) - High quality lightweight wrappers for native Web APIs for idiomatic use with Angular.
- [RxJS](https://rxjs.dev/) - A javascript library for reactive programming using Observables, to make it easier to compose asynchronous or callback-based code.
- [TypeScript](https://www.typescriptlang.org/) - TypeScript is an open-source language which builds on JavaScript, one of the world’s most used tools, by adding static type definitions.
- [ng-connection-service](https://github.com/ultrasonicsoft/ng-connection-service) - Detects whether browser has an active internet connection or not in Angular application.
- [PWACompat](https://github.com/GoogleChromeLabs/pwacompat) - A library for creating splash screens and icons for Mobile Safari, as well as supporting IE/Edge's Pinned Sites feature.


## Getting started 🏁
To clone and run this application, you'll need [Git](https://git-scm.com) and [Node.js](https://nodejs.org/en/download/) (which comes with [npm](http://npmjs.com)) installed on your computer.

From your command line:
-  `git clone https://github.com/sldiaz04us/angular-weather-app.git`
-  `cd angular-weather-app/`
-  `npm install` to install all dependencies.

Before you run the application, you'll also need:
- Create a [Google API Key](https://developers.google.com/maps/documentation/javascript/get-api-key) to use Google Maps Platform products.
- Enable [Places and Geocoding APIs](https://console.cloud.google.com/apis/library).
- Add in the index.html file the below script with your Google API Key.
```html
<!-- index.html -->
<!DOCTYPE html>
<html lang="en">
  <head>
    ...
    <script defer src="https://maps.googleapis.com/maps/api/js?key={YOUR_API_KEY}&libraries=places"></script>
    ...
  </head>
  <body>
   ...
  </body>
</html>
```
- Create an [OpenWeather API Key](https://openweathermap.org/api).
- Add your OpenWeather API Key to the `environment.ts` and `environment.prod.ts` files.
```typescript
// environment.ts
export const environment = {
  production: true,
  openWeatherApiKey: '{YOUR_API_KEY}'
};
```
-  Run `ng serve`, this command runs the application.
-  Navigate to `http://localhost:4200/`


## What's missing❓
### Favorite locations
A location module where the users can add their favorite places and be able to see a detail of the weather forecast for each place on the same page.

### Radar map
A map module where the users can see a snapshot of the radar map showing information such as rain, snow, storm, etc.

### Settings
A settings module where the users can store their preferred location, temperature unit, etc.

### Unit/Integration tests 🧪
I skipped writing test for this project.

### Accessibility ♿
Not all components have properly defined [aria attributes](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA), visual focus indicators, etc.


## Credits
Design inspired by [Diana Malewicz - Weather App UI illustrations](https://uxdesign.cc/create-a-weather-app-ui-with-3d-like-illustrations-4a6a5686c5ea)

