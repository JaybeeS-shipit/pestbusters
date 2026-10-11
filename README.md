# PestBusters

Digital pest control inspection logs, built for HACCP and food safety audits.

## Run it

```bash
npm install
npm run dev
```

Open the URL Vite prints (http://localhost:5173).

### In GitHub Codespaces
Code → Codespaces → Create codespace, then `npm install && npm run dev`.
Open the forwarded port 5173 (works on your phone too).

### Deploy to Vercel
Import this repo at vercel.com/new. Framework preset: Vite. Click Deploy.

## What is here

- `src/components/InspectionForm.jsx`: technician entry form
- `src/components/AuditDashboard.jsx`: search, filters, CSV and PDF export (demo data)
- `src/App.jsx`: temporary view switcher in place of real login
- `database/schema.sql`: Supabase/Postgres schema with role-based RLS

## Next steps

1. Create a Supabase project and run `database/schema.sql` in the SQL editor.
2. `npm install @supabase/supabase-js`, add `.env.local` with `VITE_SUPABASE_URL` and `VITE_SUPABASE_ANON_KEY`.
3. Replace the `onSubmit` stub in the form with real inserts and photo uploads.
4. Replace the demo `records` in the dashboard with a joined query.
5. Add login and route users by `profiles.role`.
