# Cloudflare Pages Deployment Guide

This guide will help you deploy the Evergreen Consistency website to Cloudflare Pages.

## Prerequisites

- A Cloudflare account
- The GitHub repository connected to Cloudflare Pages

## Deployment Steps

### 1. Connect to Cloudflare Pages

1. Log in to your Cloudflare dashboard
2. Navigate to **Pages** in the sidebar
3. Click **Create a project**
4. Select **Connect to Git**
5. Choose your GitHub account and select the `Evergreen-Consistency-Web` repository

### 2. Configure Build Settings

Set the following build configuration:

- **Project name**: `evergreen-consistency-web` (or your preferred name)
- **Production branch**: `main`
- **Framework preset**: `Next.js`
- **Build command**: `npm run build`
- **Build output directory**: `out`
- **Root directory**: `/` (leave empty for root)

### 3. Environment Variables (Optional)

If you need any environment variables, add them in the **Environment variables** section:

- `NODE_VERSION`: `18` (or your preferred Node.js version)

### 4. Deploy

1. Click **Save and Deploy**
2. Cloudflare will automatically build and deploy your site
3. The first deployment may take 5-10 minutes

### 5. Custom Domain (Optional)

1. After deployment, go to your project settings
2. Navigate to **Custom domains**
3. Add your domain (e.g., `evergreenconsistency.com`)
4. Follow the DNS configuration instructions

## Build Process

The build process will:

1. Install dependencies (`npm install`)
2. Build the Next.js application (`npm run build`)
3. Generate static files in the `out/` directory
4. Deploy the static files to Cloudflare's global network

## Troubleshooting

### Build Failures

If the build fails, check:

1. **Node.js version**: Ensure you're using Node.js 18 or higher
2. **Dependencies**: All dependencies are properly listed in `package.json`
3. **Build output**: The `out/` directory is being generated correctly

### Common Issues

- **Build timeout**: Increase the build timeout in project settings
- **Memory issues**: The build process should complete within standard limits
- **File size**: All files are under GitHub's 100MB limit

## Performance

Your site will be served from Cloudflare's global network with:

- **Automatic CDN**: Content delivered from the nearest edge location
- **Image optimization**: Automatic image compression and format optimization
- **Minification**: CSS and JavaScript are automatically minified
- **Caching**: Aggressive caching for optimal performance

## Monitoring

Monitor your deployment in the Cloudflare Pages dashboard:

- **Deployments**: View all deployment history
- **Analytics**: Track page views and performance
- **Functions**: Serverless functions (if needed)
- **Logs**: View build and runtime logs

## Updates

To update your site:

1. Make changes to your code
2. Commit and push to the `main` branch
3. Cloudflare Pages will automatically trigger a new deployment
4. The new version will be live within minutes

## Support

For issues with Cloudflare Pages deployment, refer to:
- [Cloudflare Pages Documentation](https://developers.cloudflare.com/pages/)
- [Next.js Static Export Guide](https://nextjs.org/docs/app/building-your-application/deploying/static-exports)

---

Your website is now ready for production deployment on Cloudflare Pages! 