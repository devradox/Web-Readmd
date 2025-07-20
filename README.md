# Personal Web Admin Panel

A modern admin panel for your personal website, built with Next.js, TypeScript, and Tailwind CSS. 

## ✨ Features

- **Authentication**: Simple Admin login with username/password
- **Contact Management**: View, mark as read, and delete real contact form submissions
- **Project Management**: Add, edit, and remove real portfolio projects
- **Content Management**: Edit About, Skills, and Experience sections
- **Settings Management**: Update website and contact settings
- **Analytics**: See real contact stats (ready for future analytics integration)
- **Persistent Storage**: All data saved in `/data/*.json` files
- **No mock/fake data**: Everything shown is real and up-to-date
- **Radix UI & Lucide Icons**: Clean, modern interface

## 🚀 Getting Started

1. **Install dependencies**
   ```bash
   npm install
   ```

2. **Run the development server**
   ```bash
   npm run dev
   ```
   The app will be available at [http://localhost:3000](http://localhost:3000) (or another port if 3000 is in use).

3. **Login to Admin Panel**
   - Go to `/admin`
   - Default credentials: `admin` / `admin123`

## 🗂️ Data Storage

All data is stored in the `/data` directory as JSON files:
- `contacts.json` — Contact form submissions
- `projects.json` — Portfolio projects
- `settings.json` — Website and contact settings
- `content.json` — About, skills, and experience content

## 🛠️ API Endpoints

- `GET /api/admin/contacts` — List all contacts
- `PATCH /api/admin/contacts/[id]` — Mark contact as read/unread
- `DELETE /api/admin/contacts/[id]` — Delete a contact
- `GET /api/admin/projects` — List all projects
- `POST /api/admin/projects` — Add a new project
- `PUT /api/admin/projects` — Update a project
- `DELETE /api/admin/projects?id=ID` — Delete a project
- `GET/POST /api/admin/settings` — Get/update settings
- `GET/POST /api/admin/content` — Get/update content

## 🧑‍💻 Customization
- Update credentials in the login logic for production use
- Add your own projects, content, and settings via the admin panel
- Extend analytics with Google Analytics or similar

## 📦 Tech Stack
- [Next.js](https://nextjs.org/) (App Router)
- [TypeScript](https://www.typescriptlang.org/)
- [Tailwind CSS](https://tailwindcss.com/)
- [Radix UI](https://www.radix-ui.com/)
- [Lucide React](https://lucide.dev/)

## 📄 License
MIT 
