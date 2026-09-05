# viiv-portal-proxy

Tiny Vercel project that reverse-proxies `portal.viivindia.com` to the VIIV
student webinar app hosted on Cloudflare Workers
(`https://sites-project.raghurram83.workers.dev`).

## Deploy
1. Import this repo as a new Vercel project (Framework preset: Other, no build).
2. Project → Settings → Domains → add `portal.viivindia.com`.
   Vercel manages the DNS record automatically.

The app, database (Cloudflare D1) and WhatsApp OTP all stay on Cloudflare; this
project only forwards traffic so the branded domain works.
