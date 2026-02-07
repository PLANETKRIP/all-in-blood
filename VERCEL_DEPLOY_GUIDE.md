    # Vercel Deployment Guide (Step-by-step)

    1. Create a GitHub repository and push your project.
    2. Sign in to Vercel and import the repository (New Project → Import Git Repository).
    3. Configure Environment Variables in Vercel Dashboard:
       - OPENAI_API_KEY: sk-...
       - OPENAI_MODEL: gpt-4o-mini
    4. For Next.js API routes use the `next_api/pages/api` folder content. Move pages into your Next.js app root.
    5. Set Build & Output Settings if using Vite frontend:
       - Build command: `npm run build`
       - Output directory: `dist`
    6. Deploy and monitor logs. Use Vercel functions for API routes to keep keys safe.

    Notes:
- If using Express, prefer deploying on Railway/Render or container service.
- For serverless functions, adapt routes to Next.js API routes (already provided).
