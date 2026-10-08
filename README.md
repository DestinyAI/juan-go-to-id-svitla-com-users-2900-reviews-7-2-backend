# performance-review-optimizer-1 — Backend

Custom backend for the [performance-review-optimizer-1](https://github.com/DestinyAI/juan-go-to-id-svitla-com-users-2900-reviews-7-2.git) app.

## Run locally

```bash
node server.js
```

## Expose to the app via cloudflared tunnel

```bash
brew install cloudflare/cloudflare/cloudflared
cloudflared tunnel --url http://localhost:3000
```

Copy the printed URL (e.g. `https://random-name.trycloudflare.com`) and paste it into the app's **Settings → Backend URL** field.

## Connect a self-hosted GitHub Actions runner (for automated tasks)

Go to your repo on GitHub → **Settings → Actions → Runners → New self-hosted runner** and follow the steps for macOS / ARM64.
