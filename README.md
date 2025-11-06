# InfoHub

InfoHub is a modern, responsive React application built with Vite that provides quick access to essential information tools: weather updates, currency conversion, and motivational quotes. Designed for simplicity and efficiency, it integrates real-time data from external APIs with fallback mechanisms for reliability.

## Features

- **Weather Module**: Fetch current weather conditions for any city using the WeatherAPI.com service. Includes temperature in Celsius and Fahrenheit, and weather descriptions. Features a fallback to mock data if the API is unavailable.
- **Currency Converter**: Convert Indian Rupees (INR) to US Dollars (USD) and Euros (EUR) using real-time exchange rates from exchangerate.host. Includes input validation and fallback to mock rates.
- **Quote Generator**: Generate random motivational quotes from a curated local collection. Perfect for daily inspiration.
- **Responsive Design**: Optimized for desktop and mobile devices with a clean, accessible UI.
- **Accessibility**: Includes ARIA labels, keyboard navigation, and screen reader support.

## Technologies Used

- **Frontend**: React 19, Vite
- **Styling**: CSS (custom styles)
- **Icons**: React Icons (FontAwesome)
- **HTTP Client**: Axios
- **Environment Management**: dotenv
- **Linting**: ESLint with React plugins
- **Build Tool**: Vite

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/InfoHub-Challenge.git
   cd InfoHub-Challenge
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables (see below).

4. Start the development server:
   ```bash
   npm run dev
   ```

5. Open your browser to `http://localhost:5173` (default Vite port).

## Usage

- Navigate between tabs: Weather, Currency, and Quotes.
- **Weather**: Enter a city name and click "Get Weather" to fetch data.
- **Currency**: Enter an amount in INR and click "Convert" to see USD and EUR equivalents.
- **Quotes**: Click "New Quote" to generate a random motivational quote.

## Environment Variables

Create a `.env` file in the root directory and add the following:

```
VITE_WEATHER_API_KEY=your_weatherapi_key_here
```

- Obtain a free API key from [WeatherAPI.com](https://www.weatherapi.com/).
- The currency converter and quote generator do not require API keys as they use public endpoints or local data with fallbacks.

## Scripts

- `npm run dev`: Start the development server.
- `npm run build`: Build the project for production.
- `npm run lint`: Run ESLint to check for code issues.
- `npm run preview`: Preview the production build locally.

## Project Structure

```
InfoHub-Challenge/
├── public/
│   └── vite.svg
├── src/
│   ├── assets/
│   │   └── react.svg
│   ├── components/
│   │   ├── CurrencyConverter.jsx
│   │   ├── QuoteGenerator.jsx
│   │   └── WeatherModule.jsx
│   ├── App.jsx
│   ├── App.css
│   ├── index.css
│   └── main.jsx
├── api/
│   └── utils.js
├── .env
├── package.json
├── vite.config.js
└── README.md
```

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes. Ensure code follows the existing ESLint rules.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments

- Weather data provided by [WeatherAPI.com](https://www.weatherapi.com/).
- Exchange rates from [exchangerate.host](https://exchangerate.host/).
- Quotes sourced from various public domains.
