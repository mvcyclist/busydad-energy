# BusyDad Energy Static Host

This directory contains a minimal static site used to host the Tesla Fleet API public key for the BusyDad (Rai Home) integrations. Deploy the contents of `public/` to a static host (Vercel, Netlify, etc.) and point your domain (for example `busydad.ai`) at it.

- The public key must be served at `/.well-known/appspecific/com.tesla.3p.public-key.pem`.
- `index.html` is optional but provides a friendly landing page.
- Remember to keep `private-key.pem` secret; only the public key is deployed.

## Deployment Steps

1. Create a new Git repository and push this folder.
2. Import it into your static hosting provider (e.g. Vercel).
3. Add the custom domain, such as `busydad.ai`, in the host dashboard.
4. Update DNS records so the domain points to the static host.
5. Verify the public key URL responds over HTTPS before completing Tesla partner registration.
