# quote-generator

This is a simple web application that generates random quotes from a JSON file obtained from an external API. The quotes are displayed on the webpage, and users have the option to tweet the quote as well.

The application was built with HTML, CSS, and JavaScript. It also uses the Fetch API to retrieve data from the external API.

## Features

- Generate a random quote from an external API
- Display the quote and author on the webpage
- Style the quote differently based on its length
- Allow users to tweet the quote

## How to Use

To use the Random Quote Generator, follow these steps:

1. Clone or download the repository
2. Open the `index.html` file in a web browser
3. Click the "New Quote" button to generate a new quote
4. Click the "Tweet" button to tweet the current quote

## Code Overview

Here are the main components of the code:

- `quoteContainer`: The HTML element that displays the quote and author
- `apiQuotes`: An array that stores the quotes retrieved from the external API
- `loading()`: A function that shows a loading spinner while the data is being fetched
- `complete()`: A function that hides the loading spinner once the data has been fetched
- `newQuote()`: A function that generates a new quote by selecting a random quote from `apiQuotes`
- `getQuotes()`: An asynchronous function that retrieves the quotes from the external API
- `tweetQuote()`: A function that opens Twitter and populates the tweet with the current quote and author
- `newQuoteBtn` and `twitterBtn`: The buttons that trigger `newQuote()` and `tweetQuote()` when clicked

## Credits

The quotes used in this application were obtained from the [Quotes API](https://jacintodesign.github.io/quotes-api/), created by [Jacinto Design](https://github.com/jacintodesign).
