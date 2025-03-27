# Netlify Reverse Proxy

A simple reverse proxy that works on Netlify, adapted from [ytanck/vercel-reverse-proxy](https://github.com/ytanck/vercel-reverse-proxy).

This proxy can be used to access various APIs and websites, including:
- OpenAI/ChatGPT
- GitHub
- Google
- And more!

## Features

- Proxy any HTTP or HTTPS endpoint
- Simple URL pattern: `/proxy/domain.com/path` or `/httpproxy/domain.com/path`
- Special routes for common services
- Works with Netlify's free tier

## Deployment

### Option 1: One-click Deploy

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/YOUR_USERNAME/netlify-reverse-proxy)

(Note: Fork this repository first, then update the link with your GitHub username)

### Option 2: Manual Deployment

1. Fork this repository
2. Sign up for a Netlify account if you don't have one
3. Create a new site from Git in the Netlify dashboard
4. Connect your GitHub account and select your forked repository
5. Deploy your site

## Usage

Once your site is deployed, you can use it like this:

### For HTTPS resources:
```
https://YOUR-NETLIFY-SITE.netlify.app/proxy/api.openai.com/v1/chat/completions
```

### For HTTP resources:
```
https://YOUR-NETLIFY-SITE.netlify.app/httpproxy/example.com/some/path
```

### Special Routes:
```
https://YOUR-NETLIFY-SITE.netlify.app/chat
https://YOUR-NETLIFY-SITE.netlify.app/openai
```

## Example Use Cases

- Access OpenAI API without CORS issues
- GitHub downloads acceleration
- Access to restricted content
- Content delivery optimization

## Notes

This proxy is provided as-is for educational purposes. Please use responsibly and comply with the terms of service of all websites and APIs you access through this proxy.

## License

MIT 