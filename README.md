# TPM Trail Co. — Website & CMS Setup Guide

## Your website files

| File | Purpose |
|------|---------|
| `index.html` | Your entire website (main site + blog journal) |
| `admin/index.html` | Decap CMS dashboard — accessed at yoursite.com/admin |
| `admin/config.yml` | CMS configuration — defines blog fields and settings |
| `netlify.toml` | Netlify routing and build settings |

---

## How to deploy on Netlify + connect the CMS

### Step 1 — Create a GitHub account
1. Go to https://github.com and sign up free
2. Click **New repository**
3. Name it `tpm-trail-co`
4. Set to **Public**
5. Click **Create repository**
6. Upload ALL files from this folder (index.html, netlify.toml, and the admin/ folder)

### Step 2 — Connect Netlify to GitHub
1. Go to https://netlify.com and log in with your Gmail
2. Click **Add new site** → **Import an existing project**
3. Choose **GitHub** → select your `tpm-trail-co` repo
4. Leave all build settings as default
5. Click **Deploy site**
6. Your site is now live at a URL like `tpm-trail-co.netlify.app`

### Step 3 — Enable Netlify Identity
1. In your Netlify dashboard, click your site
2. Go to **Identity** tab → click **Enable Identity**
3. Under **Registration preferences** → select **Invite only**
4. Scroll down to **Services** → **Git Gateway** → click **Enable Git Gateway**
5. Go back to **Identity** → click **Invite users**
6. Enter `james.companyy@gmail.com` and send the invite
7. Check your Gmail and accept the invite — set your password

### Step 4 — Log into your CMS
1. Go to `yoursite.netlify.app/admin`
2. Log in with james.companyy@gmail.com
3. You'll see the Decap CMS dashboard with your blog posts

---

## How to write a new blog post

1. Go to `yoursite.netlify.app/admin`
2. Click **Blog Posts** → **New Blog Post**
3. Fill in the fields:
   - **Title** — your headline
   - **Category** — Trail Stories, Ecology, or Gear
   - **Date** — publish date
   - **Excerpt** — 2-3 sentence preview
   - **Body** — write your full article (rich text editor)
4. Click **Publish** when ready
5. Netlify automatically rebuilds and deploys your site

---

## How to connect a custom domain (optional)

1. Buy a domain at https://namecheap.com (e.g. tpmtrailco.com — ~$12/year)
2. In Netlify → **Domain settings** → **Add custom domain**
3. Follow Netlify's instructions to point your domain's DNS to Netlify
4. Netlify provides free SSL (https) automatically

---

## Questions?
Contact james.companyy@gmail.com or return to Claude for help updating the site.
