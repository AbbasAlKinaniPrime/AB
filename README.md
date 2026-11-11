# Samplify Kinani

**منصة العينات الإحصائية التفاعلية | Interactive Sampling Techniques Platform**

Prepared and supervised by **Dr. Abbas Al-Kinani (PhD), Community Medicine and Public Health**
Al-Ayn Iraqi University, College of Medicine, Department of Community Medicine

© 2026 Samplify Kinani. All rights reserved. No part of this platform may be copied, modified or redistributed without written permission from the author.

## Contents
Sample size calculation, eligibility criteria and participant flow, random number table, simple random, systematic, stratified (proportional and Neyman), cluster, multistage (PPS) and nonprobability sampling, and a sampling versus non-sampling error simulator. Arabic and English.

## Deployment (GitHub Pages)
1. Upload all files (including `_config.yml`) to the root of a **public** repository.
2. Settings → Pages → Source: *Deploy from a branch* → Branch: `main`, folder `/ (root)` → Save.
3. The site URL, canonical link, sharing image, sitemap and robots file fill in automatically from the repository address (`{{ site.github.url }}`); no manual editing is needed, including after adding a custom domain.

## Visitor counter (optional)
The strip under the header shows: online now, visits today, total visits and unique visitors. It stays hidden until it is set up.

1. Go to console.firebase.google.com, create a project (Google Analytics not needed).
2. Build → Realtime Database → Create database → choose a location → start in **locked mode**.
3. Open the **Rules** tab, replace everything with the contents of `database.rules.json`, then **Publish**.
4. Project settings → Your apps → **Web (</>)** → register the app → copy the `firebaseConfig` object.
5. In `counter-config.js`, replace `null` with that object (it must include `databaseURL`), then commit.

Definitions: *visits* = browser sessions (reloads in the same session are not recounted); *visitors* = distinct browsers/devices; *online now* = devices with the page open and visible during the last minute; *today* uses Baghdad time.
Connections open for about a second once a minute and then close, so a full lecture hall stays within the free plan's 100 simultaneous connections.

## Maintenance note
`index.html` is processed by Jekyll. Do not add `{{` or `{%` to its code; if ever needed, wrap that code between `{% raw %}` and `{% endraw %}`.
