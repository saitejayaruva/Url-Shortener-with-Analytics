# 🔗 Full Stack URL Shortener

A modern **Full Stack URL Shortening Platform** built with  
**React (Vite) + Spring Boot + JWT Security + PostgreSQL (Neon Cloud)**.  
Users can shorten URLs, manage links, track analytics, and securely authenticate.

---

## 🌐 Live Demo

### ✅ Frontend (Netlify)
🔗 https://urshrtly.netlify.app/

### ✅ Backend (Render)
🔗 https://url-shortener-sb-6x0h.onrender.com

✅ **Database:** PostgreSQL hosted on **Neon Cloud**

---

## 🚀 Tech Stack

### 🖥 Frontend
- React 19 + Vite
- Tailwind CSS
- Material UI (MUI)
- Framer Motion
- React Router DOM
- React Hook Form
- React Query
- Axios
- Chart.js + React ChartJS 2
- Copy to Clipboard
- Day.js
- React Hot Toast
- React Icons
- React Loader Spinner

### ⚙ Backend
- Spring Boot 3.4
- Spring Security (JWT Authentication)
- Spring Data JPA
- Lombok
- PostgreSQL (Neon Cloud Hosted)
- Maven

---

## ✨ Features

✅ URL Shortening  
✅ JWT Authentication & Authorization  
✅ Secure APIs with Spring Security  
✅ Dashboard with Click Analytics  
✅ Copy to Clipboard  
✅ Charts for Link Performance  
✅ Fully Responsive UI  
✅ API Integration using Axios  
✅ Role-Based Security  
✅ Cloud-hosted PostgreSQL Database (Neon)  

---

## 📁 Project Structure

```
url-shortener/
├── url-shortener-react/   → Frontend
└── url-shortener-sb/      → Backend
```

---

## ⚡ How to Use (Important Order)

### ✅ Step 1: Start Backend First

If running locally:

```bash
cd url-shortener-sb
mvn clean install
mvn spring-boot:run
```

Backend runs at:

```
http://localhost:8080
```

✅ **For Live App:**  
Render backend is already running and connected to **Neon PostgreSQL**:

```
https://url-shortener-sb-6x0h.onrender.com
```

---

### ✅ Step 2: Start Frontend After Backend

If running locally:

```bash
cd url-shortener-react
npm install
npm run dev
```

Frontend runs at:

```
http://localhost:5173
```

✅ **For Live App:**  
Netlify Frontend:

```
https://urshrtly.netlify.app/
```

---

## 🔐 JWT Authentication Flow

1. User registers or logs in  
2. Server generates JWT token  
3. Token stored in frontend (`localStorage`)  
4. Token sent in headers for secured APIs  

---

## 📊 Analytics Dashboard

- View total URL clicks  
- Track daily URL performance  
- Graph-based analytics using Chart.js  

---

## 🗄 Database Configuration

### ✅ Local PostgreSQL
```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/url_shortener
spring.datasource.username=postgres
spring.datasource.password=yourpassword
```

### ✅ Cloud PostgreSQL (Neon)
```properties
spring.datasource.url=jdbc:postgresql://<neon-host>/<db-name>?sslmode=require
spring.datasource.username=<neon-username>
spring.datasource.password=<neon-password>
```

---

## 📦 Build for Production

### Frontend
```bash
npm run build
```

### Backend
```bash
mvn clean package
```

---

## 🌍 Deployment Ready For

✅ Netlify (Frontend)  
✅ Render (Backend)  
✅ Neon (PostgreSQL Database)  
✅ Docker (Optional)  
✅ AWS / Railway  

---

## 🛠 API Endpoints (Sample)

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/auth/register` | User registration |
| POST | `/api/auth/login` | User login |
| POST | `/api/url/shorten` | Create short URL |
| GET | `/api/url/{code}` | Redirect |
| GET | `/api/url/analytics` | Dashboard analytics |

---

## 🔐 Security

- Spring Security 6+  
- JWT Token Authentication  
- Password Encryption  
- Secured API Routes  

---

## 👨‍💻 Author

**Saiteja Yaruva**  
Full Stack Developer | Java | Spring Boot | React  
📍 India  

---

## ⭐ Support This Project

If you found this useful, please **give it a ⭐ on GitHub** — it motivates me to build more open-source projects!

---

## 📝 License

This project is licensed under the **MIT License**.
