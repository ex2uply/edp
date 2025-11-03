# EDP

A Next.js (App Router) client located in `client/` with Firebase integration, Tailwind CSS, and a small set of analytics/chatbot UI components.

## Tech Stack
- Next.js 15 (App Router) + React 19 + TypeScript
- Tailwind CSS
- Firebase (Auth, Firestore)

## Prerequisites
- Node.js 18+ (recommended LTS)
- pnpm or npm

## Getting Started
1) Install dependencies:
```bash
cd client
pnpm install   # or: npm install
```

2) Create environment file `client/.env.local` with your Firebase credentials:
```bash
NEXT_PUBLIC_FIREBASE_API_KEY=your_api_key
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your_auth_domain
NEXT_PUBLIC_FIREBASE_PROJECT_ID=your_project_id
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=your_storage_bucket
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
NEXT_PUBLIC_FIREBASE_APP_ID=your_app_id
```

3) Run the dev server:
```bash
pnpm dev   # or: npm run dev
```
Then open http://localhost:3000

## Common Scripts
Run these from the `client/` directory:
- `pnpm dev` / `npm run dev`: start local dev server
- `pnpm build` / `npm run build`: build production assets
- `pnpm start` / `npm run start`: run production build
- `pnpm lint` / `npm run lint`: lint code

## Project Structure (high level)
```
EDP/
  client/
    app/                # Next.js app router pages
    components/         # UI and app components
    hooks/              # React hooks
    lib/                # utilities, providers (e.g., Firebase)
    public/             # static assets
    styles/             # global styles
    package.json        # scripts and dependencies
```

## Notes
- Build artifacts (`client/.next`), `node_modules`, and env files are ignored via `.gitignore`.
- Line endings are normalized by Git on Windows; warnings about LF/CRLF are safe to ignore.

## License
This project is for learning/demo purposes. Add a license if you plan to distribute.


