# Stop Typing App website

The landing page for [Stop Typing App](https://github.com/kevintraver/stop-typing-app), a macOS menu bar app that nudges you to dictate instead of typing out paragraphs.

It's a single static page with no build step: `index.html` plus its icons. Vercel serves it as is.

To preview locally:

```sh
python3 -m http.server 8000
```

## Analytics

The page loads [Vercel Web Analytics](https://vercel.com/docs/analytics) from `/_vercel/insights/script.js`. It only works on a Vercel deployment with Analytics turned on for the project, so the request 404s when previewing locally.
