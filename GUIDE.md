# Echo Vault – Publish & AdSense Guide

## Files in this project (put ALL of them in the root of your repo)
index.html, style.css, game.js, about.html, privacy.html, contact.html, ads.txt

## Step 1 – Fix the placeholders
- contact.html: replace YOUR-EMAIL@example.com with your real email.
- Open index.html in your browser (double-click) and test the game first.

## Step 2 – Put it on GitHub
1. Create a free account at github.com.
2. New repository -> name it e.g. `echo-vault` -> Public -> Create.
3. Click "uploading an existing file", drag all 7 files in, then Commit.
   (Files must be in the repo root, not inside a folder.)

## Step 3 – Turn on GitHub Pages
Repo -> Settings -> Pages -> Source: "Deploy from a branch" -> Branch: main, folder: / (root) -> Save.
After ~1 minute your game is live at https://YOUR-USERNAME.github.io/echo-vault/

## Step 4 – Get a custom domain (important for AdSense)
- AdSense generally does not accept free subdomains like github.io, and it looks for
  ads.txt at the ROOT of your domain (yourdomain.com/ads.txt).
- Buy a cheap domain (e.g. echovault.games / playechovault.com) from Namecheap, GoDaddy, Cloudflare, etc.
- In the repo, create a file named `CNAME` containing only your domain, e.g. `playechovault.com`
- At your domain registrar add DNS records:
  - A records for the apex domain -> 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
  - CNAME record: www -> YOUR-USERNAME.github.io
- Repo -> Settings -> Pages -> Custom domain -> enter it -> tick "Enforce HTTPS".
- Check https://yourdomain.com/ads.txt opens and shows your publisher line.

## Step 5 – Add the site in AdSense
- AdSense -> Sites -> Add site -> enter your custom domain.
- The AdSense code is already in the <head> of every page, so just click "Verify".
- Wait for review (days to a few weeks). Ads will start showing after approval.

## Tips to get approved
- Have real content: the game page includes a how-to-play/strategy guide; keep adding pages
  (tips articles, level strategy, update log). Thin one-page sites are often rejected.
- Keep the About, Privacy Policy, Contact pages (already included).
- Don't click your own ads, ever.
- Get some real traffic: share on Reddit (r/WebGames, r/IndieGaming), itch.io, Twitter/X, Discord.

## Ideas to grow
- Add more levels/guard types, a daily challenge, and a leaderboard.
- Write blog-style pages: "Echo Vault beginner tips", "How the maze is generated".
