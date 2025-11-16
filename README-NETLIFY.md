# Deploying to Netlify
1. Push this project to a GitHub repo.
2. Create a free Netlify account and choose "New site from Git".
3. Connect your GitHub repo and select the branch (main).
4. Set the build command: `npm run build && npm run export` and publish directory `out`.
5. Deploy — Netlify will build and publish. You’ll get a `*.netlify.app` URL.

## Custom domain
1. In Netlify: Site settings → Domain management → Add custom domain.
2. Add your domain (e.g., `yourdomain.com`). Netlify will show DNS records.
3. At your domain registrar, create the DNS records Netlify requests (A/CNAME).
4. After DNS propagation, your site is live with HTTPS.

## Netlify Forms
- The contact form is wired to Netlify Forms via `data-netlify="true"` and a hidden `form-name` field.
- You can view submissions in the Netlify dashboard under Forms.
