## Global Currency Converter (MERN Stack)

A full-stack currency converter application built using React (Vite) and Node.js with Express. The application allows users to convert between more than 170 global currencies in real time using live exchange rates from a third-party API.

This project demonstrates frontend–backend communication, REST API design, and secure handling of environment variables in a MERN-style architecture.

---

### Features
- Real-time currency conversion using live exchange rates
- Supports over 170 international currencies
- User-friendly React interface with dropdown currency selection
- Express-based backend API
- Secure API key management using environment variables
- Rate limiting to prevent excessive API usage
- CORS configuration for safe client–server communication

---

### Tech Stack

**Frontend**
- React (Vite)
- Axios
- CSS

**Backend**
- Node.js
- Express.js
- Axios
- dotenv
- express-rate-limit
- cors

**External API**
- ExchangeRate-API (v6)

---

### Application Flow
1. The user selects the source currency, target currency, and amount.
2. The React frontend sends a POST request to the Express backend.
3. The backend fetches real-time exchange rates from ExchangeRate-API.
4. The converted amount and exchange rate are returned and displayed.

---

### Setup Instructions

```bash
# Backend
npm install
node app.js
```

```bash
# Frontend
npm install
npm run dev
```

Create a `.env` file in the backend directory:

```env
EXCHANGE_RATE_API_KEY=your_api_key_here
```

---

### Learning Outcomes
- Building a full-stack application with React and Express
- Working with third-party REST APIs
- Managing environment variables securely
- Implementing rate limiting and CORS
- Handling API errors gracefully

---

### Future Improvements
- Add loading indicators and better error messages
- Implement historical exchange rate data
- Improve UI responsiveness and accessibility
- Add currency search and filtering
- Deploy frontend and backend to production
