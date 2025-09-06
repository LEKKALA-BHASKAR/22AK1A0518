# URL Shortener 

This project is a backend microservice developed 
It implements a simple HTTP service with URL shortening and related functionalities.

---

## 🚀 Getting Started

### 1. Install Dependencies
Use your preferred package manager. For npm:

```bash
npm install
2. Run the Server
npm run dev
If you have a PORT environment variable set, the service will run on that port.

Otherwise, it defaults to 3006.

Server will be available at:

http://localhost:3006
📡 Endpoints
The available endpoints are:
#POST
http://localhost:3000/shorturls
   {
  "url": "https://example.com/very/long/path",
  "validity": 5,
  "shortcode": "test123"
}

##RESPONE:
{
    "shortLink": "http://localhost:3000/test123",
    "expiry": "2025-09-06T10:07:35.728Z"
}

#GET
http://localhost:3000/shorturls/test123

##RESPONSE
{
    "originalUrl": "https://example.com/very/long/path",
    "createdAt": "2025-09-06T10:02:35.728Z",
    "expiry": "2025-09-06T10:07:35.728Z",
    "clicks": 0,
    "clickData": []
}

🛠 Tech Stack
Node.js
Express.js

