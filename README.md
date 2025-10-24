# Quarry Point  
**Where creators and builders connect.**

<p align="center">
<!--
INSTRUCTION:

Save the logo image I'm generating for you.

Create an img folder in your repo.

Add the logo to that folder and uncomment the line below.
===================================================================
-->
<!-- <img src="img/quarry-point-logo.png" alt="Quarry Point Logo" width="600" /> -->
</p>

<p align="center">
<strong>
A full-stack portfolio platform for architects, designers, and tradespeople.
</strong>
<br /><br />
<a href="#core-features">Key Features</a> •
<a href="#tech-stack">Tech Stack</a> •
<a href="#getting-started">Getting Started</a> •
<a href="#screenshots">Screenshots</a>
</p>

---

### The Concept

Quarry Point is a full-stack web application built to serve a niche community: architects/designers ("Creators") and the tradespeople ("Builders") they collaborate with.

It functions as a hybrid of a professional portfolio platform (like Behance) and a social network (like Instagram), solving a key problem:

**For Creators (Architects):**  
A beautiful, modern platform to showcase project portfolios, get discovered, and find verified builders.

**For Builders (Tradespeople):**  
A way to build a real, verifiable portfolio. Instead of just listing "I did X," they can be tagged in actual projects by architects, proving their contribution and skill.

This project is a complete full-stack solution built with a modern React and FastAPI stack.

---

### Core Features

- **User Roles** — Separate registration and profiles for Creators and Builders  
- **Project Uploads** — Multi-image upload with titles, descriptions, and categories  
- **Builder Tagging** — Creators can tag registered builders on a project  
- **Verified Portfolios** — Builder profiles show “Tagged In” projects  
- **Social Feed** — Instagram-style discovery feed  
- **Likes & Comments** — Interaction layer for community  
- **JWT Authentication** — Secure login with hashed passwords  
- **Responsive UI** — Modern mobile-first layout

---

### Tech Stack

#### Frontend
- React (Vite)
- React Router
- TanStack Query
- Tailwind CSS
- Axios
- Vercel (Deployment)

#### Backend
- FastAPI
- Python 3.11+
- SQLAlchemy ORM
- Pydantic
- python-multipart (Uploads)
- passlib + python-jose (Auth)
- Uvicorn

#### Database & Hosting
- PostgreSQL
- Render (Backend Deploy)

---

### Getting Started

#### 1) Clone the Repository
```bash
git clone https://github.com/yantr-manav/quarry-point.git
cd quarry-point
```

#### 2) Backend Setup (`/backend`)
```bash
cd backend
python -m venv venv
source venv/bin/activate   # On Windows: .\venv\Scripts\activate
pip install -r requirements.txt
```

Create a `.env` file:
```env
DATABASE_URL=postgresql://user:password@host:port/dbname
JWT_SECRET_KEY=your-super-strong-secret-key
ALGORITHM=HS256
ACCESS_TOKEN_EXPIRE_MINUTES=60
```

Run backend:
```bash
uvicorn main:app --reload
```
Backend runs at: `http://127.0.0.1:8000`

---

#### 3) Frontend Setup (`/frontend`)
```bash
cd ../frontend
npm install
```

Create `.env.local`:
```env
VITE_API_URL=http://127.0.0.1:8000
```

Run frontend:
```bash
npm run dev
```
Frontend runs at: `http://localhost:5173`

---

### Screenshots

<!--
Add screenshots into /img folder and uncomment below

### Home Feed
<img src="img/screenshot-home.png" alt="Home Feed">

### Project Detail
<img src="img/screenshot-detail.png" alt="Project Detail">

### Architect Profile
<img src="img/screenshot-profile-creator.png" alt="Creator Profile">

### Builder Profile
<img src="img/screenshot-profile-builder.png" alt="Builder Profile">
-->

---

### License

This project is licensed under the MIT License.  
See the `LICENSE` file for more details.
