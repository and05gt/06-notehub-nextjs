# 📝 NoteHub App

A multi-page note-taking app built with Next.js (App Router). Browse, search,
create, delete, and view the details of your notes.

- **Live Demo:**
  [https://06-notehub-nextjs-nine-gray.vercel.app/](https://06-notehub-nextjs-nine-gray.vercel.app/)
- **Repository:**
  [https://github.com/and05gt/06-notehub-nextjs](https://github.com/and05gt/06-notehub-nextjs)

---

## 🛠 Tech Stack

- **Framework:** [Next.js](https://nextjs.org) (App Router)
- **Language:** [TypeScript](https://www.typescriptlang.org)
- **Data Fetching & State:** [TanStack Query](https://tanstack.com/query) (React
  Query)
- **HTTP Client:** [Axios](https://axios-http.com)
- **Forms & Validation:** [Formik](https://formik.org) +
  [Yup](https://github.com/jquense/yup)
- **UI & Pagination:**
  [React Paginate](https://www.npmjs.com/package/react-paginate)
- **Styling:** CSS Modules

---

## 🗺 Routes

| Route         | Description                                                                                     |
| :------------ | :---------------------------------------------------------------------------------------------- |
| `/`           | Home page with general information about the application.                                       |
| `/notes`      | Note list with search, pagination, and note creation modal/form (SSR prefetch + CSR hydration). |
| `/notes/[id]` | Detailed view of a single note (SSR prefetch + CSR hydration).                                  |

---

## 📁 Project Structure

```text
├── app/          # App Router routes, layouts, pages, loading & error boundaries
├── components/   # UI components (each with its own .tsx and .module.css)
├── lib/          # API client (Axios instance) and data fetching functions
└── types/        # Shared TypeScript interfaces and type definitions
```

---

## 🚀 Getting Started

1. Clone the repository:

   ```bash
   git clone https://github.com/and05gt/06-notehub-nextjs
   cd 06-notehub-nextjs
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Environment variables: Create a `.env` file in the root directory and set
   your NoteHub API token:

   ```env
   NEXT_PUBLIC_NOTEHUB_TOKEN=your_token_here
   ```

4. Run the development server:

   ```bash
   npm run dev
   ```

5. Open [http://localhost:3000](http://localhost:3000) in your browser to view
   the app.

## 📜 Available Scripts

- `npm run dev`: Starts the development server.
- `npm run build`: Builds the application for production.
- `npm run start`: Starts the production server.
- `npm run lint`: Runs ESLint to check for code quality issues.
