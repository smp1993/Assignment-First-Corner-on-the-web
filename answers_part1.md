# Part 1 — Short Answers 

**Q1) What is a hosting provider for web hosting? Give some other ways to host your websites.**

To me, a hosting provider is a service that puts my website’s files on internet-connected servers and delivers them over HTTP/HTTPS so anyone can open my site in a browser. Good hosting also handles things like uptime, bandwidth/CDN, HTTPS certificates, and simple deploys.

Other ways to host a site:
- Static hosts: **GitHub Pages**, **Netlify**, **Vercel**, **Cloudflare Pages**
- Managed platforms: **Firebase Hosting**, **Render**
- Cloud DIY: **AWS S3 + CloudFront**, **Google Cloud Storage + CDN**
- VPS (do-it-yourself server): **DigitalOcean** or **Linode** with Nginx/Apache

---

**Q2) Does GitHub Pages support custom domain names?**

Yes. GitHub Pages supports custom domains (e.g., `myname.com` or `www.myname.com`).

Basic setup (project pages):
1. In the repo go to **Settings → Pages** and add your custom domain.
2. In your DNS provider, create a **CNAME** record for `www.yourdomain.com` pointing to `your-username.github.io`.
3. (Optional) GitHub will create a `CNAME` file in the repo; keep it committed.
4. Turn on **Enforce HTTPS** once the certificate is issued.

Official docs with all options and DNS details:  
https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site
