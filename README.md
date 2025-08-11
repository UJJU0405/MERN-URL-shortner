# MERN-URL-shortner
# 📌 MERN URL Shortener

A simple **URL Shortener** built with the **MERN Stack**.  
Users can submit a long URL and get a shortened link. Visiting the short link redirects to the original URL.

---

## 🚀 Features
- **Shorten Long URLs** — Convert long URLs into short links.
- **Redirection** — Short links redirect to the original URL.
- **MERN Stack** — React (frontend), Node.js + Express (backend), MongoDB (database).
- **Single Command Run** — Backend & frontend run together via `npm run dev`.

---

## 🛠 Tech Stack
- **Frontend**: React.js, Axios
- **Backend**: Node.js, Express.js, ShortID
- **Database**: MongoDB + Mongoose
- **Other**: Concurrently, CORS, Dotenv

---

## 📂 Project Structure
url-shortener/
│
├── client/ # React frontend
├── server/ # Node.js + Express backend
├── package.json # Root package.json for running both
└── README.md

yaml
Copy
Edit

---

## ⚙️ Installation & Setup

### 1. Clone Repository
```bash
git clone https://github.com/your-username/url-shortener.git
cd url-shortener
2. Install Root Dev Dependencies
bash
Copy
Edit
npm install
3. Install Backend & Frontend Dependencies
bash
Copy
Edit
npm run install-all
4. Setup Environment Variables
Create a .env file inside the server folder:

ini
Copy
Edit
MONGO_URI=mongodb://127.0.0.1:27017/urlShortener
PORT=5000
BASE_URL=http://localhost:5000
5. Run the App
bash
Copy
Edit
npm run dev
Frontend → http://localhost:3000
Backend → http://localhost:5000

📌 API Endpoints
POST /api/shorten
Request Body:

json
Copy
Edit
{
  "longUrl": "https://www.example.com/some/very/long/path"
}
Response:

json
Copy
Edit
{
  "shortUrl": "http://localhost:5000/abc123"
}
GET /:shortCode
Redirects to the original long URL.

🖼 Screenshot
Homepage:

📄 License
This project is licensed under the MIT License.
