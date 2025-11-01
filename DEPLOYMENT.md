# Deployment Guide

This application can be deployed on various platforms with minimal configuration.

## Prerequisites

1. Push your code to a Git repository (GitHub, GitLab, or Bitbucket)
2. Obtain a Google AI API key for the Genkit integration (optional but recommended)

## Environment Variables

Before deploying, set the following environment variable:

```
GOOGLE_GENAI_API_KEY=your_google_ai_api_key_here
```

You can get your Google AI API key from the [Google AI Studio](https://aistudio.google.com/).

## Free Hosting Options

### 1. Vercel (Recommended)
- Free tier includes 100GB bandwidth/month
- Automatic SSL certificates
- Global CDN
- [Sign up for free](https://vercel.com)

### 2. GitHub Pages
- Completely free
- Integrates with GitHub repositories
- Custom domain support
- May require additional configuration for Next.js

### 3. Render
- Free tier with some limitations
- Custom domains
- Automatic SSL
- [Sign up for free](https://render.com)

### 4. Railway
- Free tier with $5 credit/month
- Easy deployment from GitHub
- [Sign up for free](https://railway.app)

## Configuration Files

This project includes the following deployment configuration files:

- `vercel.json` - Configuration for Vercel deployments
- `.env.example` - Example environment variables file

## Notes

- The application uses Next.js 15.3.3 with Turbopack
- All dependencies are properly configured for deployment
- The Calendly integration will work in production
- The Genkit AI integration requires the Google AI API key to function