# PromoHive

## Getting Started

1. Clone the repository
```bash
git clone <repository-url>
cd promohive
```

2. Install dependencies
```bash
npm install
```

3. Set up environment variables
- Copy `.env.example` to `.env`
- Update the environment variables with your values

4. Set up the database
```bash
npx prisma generate
npx prisma db push
```

5. Start the development server
```bash
npm run dev
```

## Deployment

The project is configured for deployment on Netlify. Simply connect your repository to Netlify and it will automatically deploy your changes.

### Environment Variables on Netlify

Make sure to set the following environment variables in your Netlify project settings:

- `DATABASE_URL`
- `VITE_API_URL`
- `VITE_SUPABASE_URL`
- `VITE_SUPABASE_ANON_KEY`

## Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run linter

Note: small edit to trigger Netlify redeploy.