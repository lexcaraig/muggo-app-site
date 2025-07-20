# MugGo App Website

This is the website for muggo.app, hosting authentication callbacks and landing pages for the MugGo iOS app.

## Structure

- `/` - Main landing page
- `/auth/email-confirmed/` - Email verification confirmation page
- `/auth/callback/` - OAuth callback handler
- `/download/` - App download page

## Setup

1. Push this repository to GitHub
2. Enable GitHub Pages
3. Set custom domain to `muggo.app`
4. Configure DNS records at your domain registrar

## DNS Configuration

Add these records at your domain registrar:

```
Type: A Record
Name: @
Value: 76.76.19.61
TTL: 300

Type: CNAME  
Name: www
Value: muggo.app
TTL: 300
```

## Deep Link Scheme

The site uses `muggo://` deep links to redirect back to the iOS app.
