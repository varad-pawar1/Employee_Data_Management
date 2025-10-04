# 🧑‍💼 Employee Data Management

Employee Data Management is a **full-stack CRUD application** for managing employees.
It uses an **Express + SQLite (TypeScript)** backend and a **React + Vite (TypeScript)** frontend, following a clean monorepo structure.

---

## 🚀 Live Demo

- **Frontend:** [https://employee-data-management-frontend-yqpc.onrender.com](https://employee-data-management-frontend-yqpc.onrender.com)
- **Backend API:** [https://employee-data-management-frontend.onrender.com](https://employee-data-management-frontend.onrender.com)

---

## 🧠 Tech Stack

| Layer    | Technology                            |
| -------- | ------------------------------------- |
| Backend  | Node.js, Express, SQLite3, TypeScript |
| Frontend | React, Vite, TypeScript               |
| Database | SQLite                                |
| Hosting  | Render                                |

---

## 📦 Monorepo Structure

```
Employee Data Management/
├── employee-backend/       # Express + SQLite API (TypeScript)
└── employee-frontend/      # React + Vite App (TypeScript)
```

---

## ✅ Prerequisites

- Node.js **v18+**

---

## ⚙️ Setup Instructions

### 1. Install Dependencies

```bash
cd employee-backend && npm install
cd ../employee-frontend && npm install
```

---

### 2. Environment Variables (Backend)

Create `employee-backend/.env`:

```env
PORT=5000
FRONTEND_URL=http://localhost:5173
DB_PATH=Data_Base/employees.db
```

The database and table will be created automatically if they don’t exist.

---

### 3. Run Locally

#### Backend (Development - ESM with ts-node)

```bash
cd employee-backend
npm run dev
```

#### Backend (Production)

```bash
cd employee-backend
npm run build
npm start
```

---

### 🖥️ Frontend Setup (React + Vite + TypeScript)

#### 1. Install Dependencies

```bash
cd employee-frontend
npm install
```

---

#### 2. Environment Variables (Frontend)

Create a `.env` file inside **employee-frontend**:

```env
VITE_API_BASE_URL=http://localhost:5000/api
VITE_APP_TITLE=Employee Management System
```

> 💡 `VITE_API_BASE_URL` points to your backend API.
> In production, update it to your hosted backend URL, for example:
>

---

#### 3. Run Locally

```bash
cd employee-frontend
npm run dev
```

Then open the app in your browser at:

👉 [http://localhost:5173](http://localhost:5173)

---

#### 4. Production Build

To build for production:

```bash
cd employee-frontend
npm run build
```

To preview the production build locally:

```bash
npm run preview
```

---

## 🌐 Environment Configuration

| File              | Variable            | Description                  |
| ----------------- | ------------------- | ---------------------------- |
| `.env` (backend)  | `PORT`              | Server port (e.g., 5000)     |
|                   | `FRONTEND_URL`      | Allowed CORS origin          |
|                   | `DB_PATH`           | Path to SQLite database file |
| `.env` (frontend) | `VITE_API_BASE_URL` | Backend API base URL         |


---

## 🧪 Tests

Once configured, you can run tests as:

```bash
cd employee-backend && npm test
cd employee-frontend && npm test
```

- Prefer `jest` + `supertest` for backend
- Prefer `vitest` for frontend

---

## 📡 API Endpoints

| Method | Endpoint             | Description     |
| ------ | -------------------- | --------------- |
| GET    | `/api/employees`     | List employees  |
| POST   | `/api/employees`     | Create employee |
| GET    | `/api/employees/:id` | Get employee    |
| PUT    | `/api/employees/:id` | Update employee |
| DELETE | `/api/employees/:id` | Delete employee |

---

## 📝 Assumptions & Design Choices

- ✅ Uses **SQLite** for simplicity and portability
- ✅ Auto-creates database and `employees` table on startup
- ✅ Uses `.env` to configure CORS via `FRONTEND_URL`
- ✅ Backend uses TypeScript with **NodeNext** + **ESM imports**
- ✅ Dev uses `ts-node` loader; production uses compiled JS in `dist/`
- ✅ Axios is used for API calls with `VITE_API_BASE_URL`

---

## ✨ Bonus Features

- 🔍 Search / filter bar on frontend with **debounce**
- ✅ Form validation before submission
- 🧠 Modular hooks and components for cleaner code structure
- 🌈 Professional folder organization (frontend + backend)

---

## ⚠️ Common Issues

- ❌ **ESM Import Errors** — Run backend with `npm run dev` (uses ts-node ESM) or use the build+start flow.
- ❌ **Database Path Issues** — The app auto-creates `Data_Base/`. Ensure the directory is writable.

---

## 📜 License

This project is licensed under the **MIT License**.

---

## 👤 Author

**Varad Pawar**
🎓 BCA Graduate | 💻 Full Stack Developer
🌐 [GitHub](https://github.com/varad-pawar1)


#### Employee Data Management
[View Project](https://github.com/varad-pawar1/Employee_Data_Management)

#### Employee Data Management Screenshot

<img width="835" height="821" alt="Screenshot 2025-10-04 161354" src="https://github.com/user-attachments/assets/b010d406-7391-4647-aa8d-7d7d61d799ba" />
<img width="469" height="1359" alt="screencapture-employee-data-management-frontend-yqpc-onrender-2025-10-04-16_20_57" src="https://github.com/user-attachments/assets/bdb298aa-4716-43b0-869b-865065f82cfa" />
<img width="513" height="801" alt="screencapture-employee-data-management-frontend-yqpc-onrender-2025-10-04-16_21_22" src="https://github.com/user-attachments/assets/35dc36c6-9de1-46d8-8f95-c068c6b3c477" />
<img width="960" height="1400" alt="screencapture-employee-data-management-frontend-yqpc-onrender-2025-10-04-16_21_37" src="https://github.com/user-attachments/assets/f6467172-73e5-4ed5-a7f4-204280f913ae" />

<img width="789" height="838" alt="Screenshot 2025-10-04 161420" src="https://github.com/user-attachments/assets/0bbb306d-c40e-4c8f-953f-f1e84a06fc51" />
<img width="791" height="810" alt="Screenshot 2025-10-04 161443" src="https://github.com/user-attachments/assets/bd22615f-01fd-4fb3-89f7-f1f4e7ade0bf" />
<img width="812" height="815" alt="Screenshot 2025-10-04 161511" src="https://github.com/user-attachments/assets/87851f53-86b7-425d-afec-eceed2713d56" />
<img width="1571" height="875" alt="Screenshot 2025-10-04 161605" src="https://github.com/user-attachments/assets/9ca0acbc-6e56-4f1e-b9b5-89b7c4c7ce75" />
<img width="1525" height="768" alt="Screenshot 2025-10-04 161654" src="https://github.com/user-attachments/assets/8513518c-3ede-4c6a-92b4-96584bbe2559" />
<img width="1590" height="897" alt="Screenshot 2025-10-04 161716" src="https://github.com/user-attachments/assets/bb75fc59-eb60-4c7b-803a-9a813e8623a7" />


```

