# novvicki.pl

Static business-card site. One file: `index.html`, no build step.

## Deploy (OVH Web Hosting, Git)

1. OVH Control Panel > Web Cloud > Hosting > your plan > **Multisite** tab.
2. On the `novvicki.pl` entry (and `www.novvicki.pl`): `...` > **Configure Git**.
3. Repository: `https://github.com/nowickit/novvicki.pl.git`, branch `main`.
4. Copy the webhook URL OVH shows and add it in GitHub: repo Settings > Webhooks
   (content type `application/json`, push events). Every push to `main` redeploys.

The target folder of the multisite entry must be empty before OVH attaches Git.
