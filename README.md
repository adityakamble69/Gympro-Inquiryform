# Gym Management System - Standalone Inquiry Form

This is the public-facing, standalone **Membership Inquiry Form** for the Gym Management System. It is built as a lightweight, independent project with **Vite** and **React**. 

Because it is fully separated from the main admin panel, you can deploy it to a public URL (like Vercel or Netlify) for your customers to access, while keeping your main admin panel private and secure.

---

## 📂 Project Structure

```text
inquiry-form/
├── src/
│   ├── App.jsx           # Self-contained inquiry form layout, states, and camera logic
│   └── main.jsx          # React app entry point
├── index.html            # Main HTML template containing styling fonts
├── vite.config.js        # Vite compilation configuration
├── .gitignore            # Git exclusion rules
└── .env                  # Target API endpoint variables (Git-ignored)
```

---

## ⚙️ Environment Configuration (`.env`)

Create a `.env` file in the root of the `inquiry-form/` directory:

```env
# Target API URL (point to your local backend or live backend server)
VITE_API_URL=http://localhost:8080/api
```

---

## 🚀 How to Run Local Form

### 1. Install Dependencies
Make sure you are inside the `inquiry-form` folder, then run:
```bash
npm install
```

### 2. Start Dev Server
To start the React development server:
```bash
npm run dev
```
*(Vite will spin up the server, typically on `http://localhost:5174` or another port displayed in the console).*

### 3. Build for Production
To generate a static build bundle for Vercel/Netlify hosting:
```bash
npm run build
```
*(The optimized compiled build will be generated in the `dist/` directory).*
