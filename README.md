# brickburst.github.io

The public website for Brick Burst: a landing page, the privacy policy, and `app-ads.txt` for AdMob.

## Before publishing

Fill in the placeholders: `grep -rn "CONTACT_EMAIL\|DEVELOPER_NAME\|EFFECTIVE_DATE" .`

- `CONTACT_EMAIL`: an address you'll answer. Google Play requires a contact email, and it appears on your store listing too. A dedicated address is a good idea.
- `DEVELOPER_NAME`: your name or the developer name you use in Play Console.
- `EFFECTIVE_DATE`: the day you publish the policy.
- `app-ads.txt`: replace its contents with the line AdMob gives you.

## Publishing

1. On GitHub, signed in as `brickburst`, create a public repository named exactly `brickburst.github.io`.
2. Push the contents of this folder to it:
   ```bash
   cd site
   git init -b main && git add . && git commit -m "Brick Burst site"
   git remote add origin https://github.com/brickburst/brickburst.github.io.git
   git push -u origin main
   ```
3. In the repository, go to *Settings → Pages*, set the source to *Deploy from a branch*, `main`, `/ (root)`.
4. After a minute, check `https://brickburst.github.io/privacy.html` and `https://brickburst.github.io/app-ads.txt`.
5. In Play Console, set the website to `https://brickburst.github.io` and the privacy policy to `https://brickburst.github.io/privacy.html`.
