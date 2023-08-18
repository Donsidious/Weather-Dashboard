
# Weather Dashboard
## Unit 06 Homework Assignment

Explore the live app here:
[Weather Dashboard](https://ryanellingson.github.io/Weather-Dashboard/)

## Project Overview


The Weather Dashboard is a convenient tool that lets users search for real-time weather conditions in any city. Enter a city name (either the city alone or "city, state") and hit search to see current weather details, including temperature, humidity, UV index, and an illustrative icon representing the weather (e.g., clear, cloudy, rainy). The app also displays a 5-day forecast at 12:00 PM for the selected city.

### Features:

- **Search History:** A button with previous search details is saved under the search field, allowing for quick access to past searches.
- **Persistent History:** Closing or refreshing the browser won't lose your history; the app will launch with the last city's weather data.
- **Clear History Option:** With a single click, users can erase their search history from local storage and remove the history buttons.

## Challenges & Areas for Enhancement

Built using the Open Weather Map data API, the app required intricate handling of the API responses. Information from one request, such as latitude and longitude, was used to generate subsequent requests, like the UV Index query.

The app also leverages JavaScript's Date object to manipulate timestamps from the Open Weather Map response. Methods like `getDate`, `getMonth`, and `getFullYear` were essential in crafting the date strings displayed on the page.

### Potential Improvement:

A notable issue arises when the Open Weather Map can't locate the user's requested city. Currently, the app doesn't notify the user, and the error is only evident in the browser's console. Addressing this by implementing a user-friendly error message would significantly enhance the user experience.
