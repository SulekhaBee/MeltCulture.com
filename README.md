# Melt Culture storefront

## Publish on GitHub Pages

1. Extract `Melt-Culture-GitHub-Pages.zip`.
2. Upload the **contents** of the extracted folder to the root of your GitHub
   repository's `main` branch. Keep `index.html` at the repository root.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**, then choose
   `main` and the `/ (root)` folder.
5. Wait for the Pages deployment to finish. The site URL is shown on the Pages
   settings screen.

The archive contains a prebuilt static site; Node.js is not needed to publish
it. To rebuild from source, install Node.js and run `npm ci` followed by
`npm run build:github-pages`.

GitHub Pages is static hosting. Razorpay checkout, order verification, and
inquiry submissions require the serverless API routes in `api/` and their
configured environment variables; those routes are not included in this static
site archive.
