# Fix 500 Errors on API Endpoints

- [ ] Update client/api/utils.js: Change module.exports to export { QUOTES, getRandomQuote };
- [ ] Update client/api/quote.js: Change require('./utils') to import { QUOTES, getRandomQuote } from './utils.js';
- [ ] Update client/api/currency.js: Change require('axios') to import axios from 'axios';
- [ ] Update client/api/weather.js: Change require('axios') and require('dotenv').config() to import axios from 'axios'; import 'dotenv/config';
- [ ] Start dev server with npm run dev in client directory
- [ ] Test /api/quote endpoint with curl
- [ ] Test /api/currency?amount=100 endpoint with curl
- [ ] Test /api/weather?city=London endpoint with curl
- [ ] Verify all endpoints return 200 with valid JSON
