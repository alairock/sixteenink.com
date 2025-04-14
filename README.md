# Sixteen Ink Website

This is the official repository for the Sixteen Ink website, featuring information about our mobile applications.

## Website Structure

- `index.html` - Main landing page
- `privacy.html` - Privacy policy page
- `styles.css` - Stylesheet for the website

## Setting up GitHub Pages with a Custom Domain

### 1. Create a GitHub Repository

1. Create a new GitHub repository named `sixteenink.com`
2. Push this code to your repository

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/yourusername/sixteenink.com.git
git push -u origin main
```

### 2. Set up GitHub Pages

1. Go to your repository settings
2. Scroll down to the "GitHub Pages" section
3. Under "Source", select the branch you want to publish (usually `main`)
4. Click "Save"

### 3. Configure Custom Domain

1. In your GitHub repository, create a file named `CNAME` with your domain name:
   ```
   www.sixteenink.com
   ```

2. In your domain registrar's settings:
   - Add an `A` record pointing to GitHub Pages IP addresses:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```
   - Add a `CNAME` record for `www` pointing to `yourusername.github.io`

3. Back in GitHub repository settings, enter your custom domain in the "Custom domain" field and save
4. Enable HTTPS for your custom domain by checking "Enforce HTTPS"

Your site will be available at both `https://sixteenink.com` and `https://www.sixteenink.com` with automatic redirection to the www version.