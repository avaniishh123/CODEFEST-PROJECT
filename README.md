# 🌟 URL Shortener

The **URL Shortener** is a sleek, high-performance web application that transforms long, messy URLs into short, shareable links—instantly and securely.

With a clean UI, custom aliasing support, click tracking, expiration handling, and fast redirection, it's the perfect tool for modern web users and developers.

---

## ✨ Features

- 🔗 **Instant URL Shortening**: Convert any long URL into a short, clean link.
- 🛠️ **Custom Short Codes**: Create personalized short URLs.
- ⏳ **Expiration Handling**: Set optional expiration dates for links.
- 📈 **Click Tracking**: View the total number of times your short link has been accessed.
- ⚡ **Fast Redirection**: Ultra-quick URL redirects powered by Flask and SQLite.
- 🛡️ **Secure and Robust**: Handles errors gracefully and ensures unique short codes.
- 🎨 **Beautiful UI**: Smooth animations, responsive design, and a gradient-themed modern interface.

---

## 🛠️ Tech Stack

- **Frontend**: HTML5, CSS3 (with custom animations), JavaScript (Vanilla JS)
- **Backend**: Python, Flask
- **Database**: SQLite
- **Other Tools**: Fetch API for async communication, Responsive Design, Form and JSON handling

---

## 🚀 How to Run Locally

1. **Clone the repository**  
   ```bash
   git clone https://github.com/your-username/url-shortener.git
   cd url-shortener
   ```

2. **Install dependencies**  
   *(Only Flask is needed)*  
   ```bash
   pip install Flask
   ```

3. **Run the server**  
   ```bash
   python app.py
   ```

4. **Access the website**  
   Open your browser and visit:  
   ```
   http://127.0.0.1:5000/
   ```

---

## 📄 Project Structure

```
├── app.py           # Backend server using Flask
├── urls.db          # SQLite database (created automatically)
├── templates/
│   └── index.html   # Frontend (served by Flask)
│   └── error.html   # Error page template
├── static/          # (optional for future CSS/JS if separated)
└── README.md        # Project documentation
```

---

## 📊 API Endpoints

- `POST /shorten` → Shortens a URL  
  Request body:
  ```json
  {
    "url": "https://your-long-url.com",
    "custom_code": "optional-custom-code",
    "expiration_days": 30
  }
  ```

- `GET /<short_code>` → Redirects to the original URL

- `GET /analytics/<short_code>` → Returns click count and URL details

---

## 🖼️ Screenshots

![image](https://github.com/user-attachments/assets/088866ac-dfeb-40f6-be78-651cc8fc044e)
![image](https://github.com/user-attachments/assets/b436aba9-3f12-42bc-b465-a3faadfa77f7)


## 🧠 Future Enhancements

- Add QR code generation for short links.
- Add user authentication for personalized URL history.
- Add charts and graphs in analytics page.
- Support for password-protected URLs.


## 📜 License

This project is licensed under the [MIT License](LICENSE).



Demo Video Link :- https://drive.google.com/file/d/1NOwnkRKn8xb6nPkOtrrvLh3Uvau_rwcn/view?usp=sharing
