# Arsene Portfolio

Responsive static portfolio for Nshimiyimana Arsene.

## Build

Requires Node.js 20 or newer.

```bash
npm ci
npm run build
```

The deployable website is generated in `dist/`. The build includes the HTML page,
compiled local CSS, and `image.jpeg`.

## Deploy to Vercel

Import this repository in Vercel and deploy. `vercel.json` configures the build
command and output directory. Alternatively, run `npx vercel --prod` from the
project directory.

## Deploy to Render

For a Render Static Site, set:

- **Build Command:** `npm ci && npm run build`
- **Publish Directory:** `dist`

These settings are also recorded in `render.yaml` for Render Blueprint deploys.
If the existing Render service was created manually, update its Build Command
and Publish Directory in **Settings**, save the changes, and trigger a new
deploy. The build creates `dist/` and copies the HTML, CSS, and profile image
into it.

For another static hosting provider, build the project and publish the contents
of `dist/`.
